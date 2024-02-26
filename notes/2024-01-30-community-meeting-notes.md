# Community Meeting Notes January 30, 2024

Community Council (CC) meeting held @ 14:30 UTC in grincoin#general channel on Keybase. Meeting lasted 65 min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.




### _Community attendance:_

* anonymous
* cekickafa
* renzokuen 
* cyptsd
* aglkm
# Short Summary
 
 
- BIP39 passphrases functionality in grin-wallet has been mentioned
- Grinvention/mimblewimble.py implementation is being discussed, dev @renzokuken has shared his view and projections. Funding idea of _mimblewimble-py_ is welcomed.
- Mwixnet testing is not realised yet.



# Agenda Points & Actions
 

* Last meeting notes here: https://github.com/grincc/agenda/tree/main/notes

* Current meeting [agenda](https://github.com/grincc/agenda/issues/123)



## Ironbelly wallet status


__anonymous__ : Lets start with agenda point 1
## 1) Gui wallet testing
It looks like a decent amount of testing is going on. Quite some misteries needed to be solved with the compilation not working on some systems thansk to croaring, but Michael/yeast figured it out.

__Cekickafa__ :  Anybody had issues with linux?

__anonymous__ : I think we have now 21 open issues within a month of which 4 [bugs], not bad. All of these will help improving the wallet.

I have not tried it yet on Linux

__cekickafa__ : Linux works for me. Windows is problem as usual.

__anonymous__ :  Ok interesting that it does work properly on Linux.

__cekickafa__ :  Yes it works. Most issues opened for windows.

__anonymous__ : I still want to do more testing using day to day actions, but I see many things have been tested already, like cancelling a transaction (does not work/bug)

💯 cekickafa

I think most of these have to do with the dependencies
In a way that is a hassle since it hard to figure out bugs with dependencies, on the other hand it is good since it means the main Grin-wallet GUI code is working and not the issue.

__cekickafa__ :  yes it is also good, many people participated for testing.

__anonymous__ : On a side node, I have Grin-GUI running in the back for a week now on Windows, so no stability issues (compiled locally).
Yes, I was happy to see many who are not regulars on the forum or Keybase to join in. I think it shows how much interest is there from the community in a core wallet.
Unless someone wants to add more, I think we can move on to agenda topic 2)

👍 cekickafa,yeastplume



__renzokuken__ : hi all, sorry for being late for the meeting.

👋 cekickafa, anonymous

I'm representing @MCM Mike

__anonymous__ :  No problem, you are right in time for a topic that is most relevant to you.
Glad you are representing Mike, I know he is still supporting Grin in the back, but he busy and hard to get a hold off for day to day things like decisions for grin governance.

 👍   renzokuken


Good to have 3 CC representatives in on chat room at the same time 😛

renzokuken 🤝


__renzokuken__ : I agreed to represent him for the period of six months with a check in the middle (3 months), just in case if I don't manage it for some reasons.


__anonymous__ : It is nice try out, to see if you like governance. Same for @cekickafa but as groundkeeper it is less new to him since he was already involved in a lot of the discussions.

👍 cekickafa,renzokuken

Lets move on to the next topic

## 2) BIP39 passphrases functionality in grin-wallet.

👍 renzokuken


__anonymous__ : I discussed this with @renzokuken. At the moment we do not have support for BIP39 in either grin-wallet or in Grin++. I see BIP39 as an option for power users. Therefore I think grinvenntion/mimblwimble.py would be very suitable since I want it to be the Swiss army knife forGrin similar how bitcoinlib in python is the swiss army knife for Bitcoin.

💯 cekickafa

__renzokuken__ : I confirm, _the mimblewimble-py_ is using _bip_utils_ library which is compatible with various btc-related standards.

🚀cekickafa, anonymous

__anonymous__ : There is also another function requested by a power user long time ago to me, support for custom wordlists. I think this is another example of a function that could be implemented in _mimblewimble.py_, purely for power users.
bip_utils is a great library, I also love using it. The developer is also really easy to contact to help serve specific needs, which is quite unique.


__cekickafa__ : Very nice!


__renzokuken__ : Yes, I also confirm that wordlist customization is more than doable. However, I must add that it would be wiser to ensure some of the core functionalities in mimblewimble-py should be completed first:
1. slatepacks (in progress)
2. RSR flow
nice to have BIP39 passphrases and custom wordlist, but what's the point if you can't exchange slatepacks yet. I suggest that should be completed first.

__anonymous__ : I agree, also you brought to me the topic of retrospective funding, or the fact that a LOT OF WORK has been done, and there has been any funding by OC or CC. I think it would make sense to compile a list of tasks and make it into a sizable funding request, enough to move _mimblewimble-py_ into something like a stable release, which does require all the basics to work. So these all be made into objectives/deliverables of a funding request.

💯 cekickafa

__cyptsd__ : hi sorry i missed the start

👋 cekickafa, anonymous, renzokuken

__anonymous__ : There are more plans/wishes I have for mimblewible-py on the long run, such as using it as basis for a custom hardware wallet:
https://forum.grin.mw/t/funding-proposal-2-bounty-for-a-hardware-wallet-implementation-bounty/10600

All of these require  mimblewible-py to be fully functioning and as such requiring a significant push in work, both coding and documentation

__renzokuken__ : Sounds like something that could push this project further. There was an honest will to complete _mimblewimble-py_ project from my side but the funding principles were probably too idealistic and project became less of priority compared to other more lucrative projects in my agenda.

__anonymous__ : Indeed, the funding model did not work. I think for something like this a good old fashioned Funding Request with clear measurable deliverables and a proper amount of funding at least largely in BTC (denominated in euro or dollar), would be suited to minimize risk for @renzokuken.
I mean we all love grassroot principles, but we also all need to pay rent at the end of the month...

👍 cekickafa

__renzokuken__ : I am not entirely sure if _mimblewimble-py_ could be helpful for this particular case, I might be wrong but I don't think hardware wallets can run Python.


__anonymous__ : This is also why David T always used funding request, even though he hated asking for money,.
It can, in fact the Jade hardware wallet that runs on the same hardware I propose is purely Python based.

__renzokuken__ :  Noted.


__cekickafa__ : _Mimblewimble.py_ reached many miles already. Personally i see it very important for Grin ecosystem enlargement.


__renzokuken__ : It is not only meant as a library to use, but also to become the most easy to read mimblewimble implementation. Python has its disadvantages, but it makes it possible to implement pleasant to read code that can itself be a documentation of something.


👍 cekickafa, anonymous, aglkm

__anonymous__ : It does however leaves some risk in security since the chip is Chinese made, not with a secure element. Hence, I would prefer it to work as a sort of 2 factor authentication device, and possible as sort of a Multisig (2 signatures by HW owner, 1 by the other party). Normally this is not possible since more than 2 parties creates problems with payment proofs, but since the HW and the computer/phone wallet are the same user, this attack becomes irrelevant I think.

👍 renzokuken

I also agree on the importance of the educational part of mimblewible-py. For example, I simply wanted to check if it supported BIP39 passwords, it took me 10 minutes to browse the code and see that it did not but easily could with some modifications. That is just because the modules are kind of independently working and because Python is that easy to read.

🙏renzokuken

__cekickafa__ : _Mimblewimble python_ will bring more contributers to Grin for sure.

__anonymous__ : So what I would propose is to think a bit about what you want for mimblewible-py @renzokuken. Make a list of _functions/tasks/deliverables_ and time estimates for each as well as an expected time in work. Then think about if and when you will have time to dedicate time to this project, and make an appropriate funding request. Try not to be to minimal, coding, and especially properly documented coding and testing code, takes quite some time, even with Python.
I think it is more important to get everything working properly than being too cheapskate on yourself and ending up not having enough funding to get by.


__renzokuken__ : so, on behalf of Grinventions I would say:
1. I agree to prepare a funding request if CC would consider it.
2. The requested features (BIP39 passwords and custom wordlist) are doable, but I advise to complete the library first (finish slatepacks, persistence of state and RSR flow).

however, as a representative of MCM Mike I can't support my own funding request, I will leave the final decision to him and rest of CC members.

👍 cekickafa, anonymous

__anonymous__ : Exactly, just like David T abstained from any voting, I think you should to. I think you can pass it along to Mike in this case, see what his opinion is.

👍 renzokuken

__renzokuken__ : Would it be ok to include in that funding request previous work I've done? I have a detailed records on time spent on this project.

💯 cekickafa


__anonymous__ : Indeed, but BIP39 and custom wordlists on the bottom of the list of things that need to be done,
That is something I can say much about since I do not know the mind of the other CC members. I always find retrospective funding difficult since we do not want everyone to ask money for what has been done.
I see it more as something to take into consideration as well as reputation that allows a more generous Funding Request to be supported as well as possible upfront payments. Not as an exact compensation for the amount of work that has been done. 
@cekickafa what is your opinion on retrospective funding in this case as well as in general?

Also to @cyptsd, what is your opinion on this?

__renzokuken__ : The very reason why I did not want to ask for funding before and waited to deliver was to actually be fair to the community. A new mimblewimble implementation is an ambitious project, I was afraid I won't manage to deliver. I did not want to commit to something without being sure I can manage it.


__cyptsd__ :  

>__anonymous__ : Also to @cyptsd, what is your opinion on this?

I’m just taking a look at grinventions now as I’m not familiar with it
 
👍  anonymous

__anonymous__ : I know your motives are pure, it is just that as I said it creates a difficult dilema since there are also contributors that contribute without payment, we do not want to make retrospective payments for all contributions ever made the default.

__renzokuken__ : Understandable.

__cyptsd__ :  But in terms of BIP39, it seems that would be good in terms of consistency with bitcoin. I didn’t actually know that grin used a different standard

👍  anonymous


__cekickafa__ : 

>__anonymous__ : @cekickafa what is your opinion on retrospective funding in this case as well as in general?

Grinventions @renzokuken spent quite time for Grin so far, he is talented, also proven to be a loyal Grin fan. I am strongly in favor him keeping close to Grin with more time via supporting him.

👍 renzokuken 👍  anonymous

__anonymous__ : @cyptsd Grin is BIP39 compatible, however, it does not support extra passwords to be added to the seed phrase at the moment.
In time I think it can be added to main wallets, for now it is more for a few power users who ask for it. It has been asked to me though multiple times

👍 cyptsd

__renzokuken__ : I would also add that I am only interested in ツ payments. If I accept BTC I publicly declare it would be only to convert it to ツ on TradeOgre.
I know that there has been buzz in the community about people contributing and taking BTC and other kinds of payments.

🔥 aglkm da,datumplane 😎

__anonymous__ : Ok. We are short of Grin, miner debacle, still gives me a headache so for now BTC it is, you can convert to ツ

__renzokuken__ : I personally agree with that, accepting ツ (or willingness to convert the payment to ツ) is a proof of believing in this technology.

💯 cekickafa 👍  anonymous, datumplane


__anonymous__ : I agree there, it purely for practical reasons, I also prefer receiving  ツ for any contributions

🤝  renzokuken 👍  anonymous

__aglkm__ : 

>__cyptsd__ :  But in terms of BIP39, it seems that would be good in terms of consistency with bitcoin. I didn’t actually know that grin used a different standard

I don't think BIP39 padsphrases can be put into power users category only. It more like a standard in Bitcoin space to secure your funds properly.

__cekickafa__ : 

>__anonymous__ : I agree there, it purely for practical reasons, I also prefer receiving  ツ for any contributions.

Yes that should be default method. Pity still we cant pay with Grin, our own currency.

__cyptsd__ : I’ve just looked at grinventions. Sounds great and should be supported imo. Having different implementations and tools to bring more skills to grin

🙏renzokuken 👍  anonymous, cekickafa, defistaker


__anonymous__ : @aglkm You are right that it should become a main wallet option in due time, when @yeastplume has fixed all the more important issues. Custom wordlists though are really for power users and pose a significant risk of losing funds when making mistakes (think different encoding etc.). For now I think it suffice to implement them in mimblewimble-py.

👍 renzokuken

Ok, so that is a TO DO for you @renzokuken, to prepare a funding request. Take your time, there is no hurry, we need make a comprehensive list and you can ask CC for feedback at any time.

__renzokuken__ : i will prepare a draft.

🔥  anynomous, cyptsd, cekickafa, 🚀 anynomous, defistaker


I need some time to get back to this code base, I haven't looked at it since summer 2023. Need to remind myself where I left off and then I will be able to make reasonable eastimates.

__anonymous__ : quick feedback, at 2 factor authentication to the functions list. I am sure we will need this in the future and you had some great ideas there.

__renzokuken__ : is it about login using ツ address signature?


__anonymous__ : Just put it on the bottom, yes
or at least using wallet derived keys for 2FA, but yes, signatures is probably best

__renzokuken__ : I have draften an RFC for it https://github.com/mimblewimble/grin-rfcs/pull/90

 👍  anonymous

__anonymous__ : I think it has enough substance to it to see it as valuable, especially when combined with the HW/2FA device..
Bascially a Grin/Jade HW without the extra server key and instead extra key in a local wallet.
Lest move on to the last agenda topic.

## 4 ) Mwixnet testing status.

__anonymous__ :  I have to be honest, ... I did not do a thing lately, got very little time and prioritized playing with Grin GUI with that little time. But yaa, I should look at all the test cases written at the least, if not add some myself.

__cekickafa__ :  I was stuck it with  tesing on ubuntu linux. I didnt try after Gui but i will try it again. Adding TO DO my list.
I dont know if any other contributers tested it?

__anonymous__ : I do not know either, I think there are actually to few people testing it, but that is also because it is hard to test. Basically writing test cases in Rust is the bets way forward... not many who can manage that. For me it also takes more focus and time than I have.



__cekickafa__ :  well. İt is really mwixy:)

💯 renzokuken ,  anonymous

__anonymous__ : In Any case, I will ad it to my list of things I would like to do but probably will not get around to 🥲

__renzokuken__ : If it requires writing test cases in Rust unfortunately I can’t help much.
But if it is about installing something, collecting logs etc then I could help.

__aglkm__ : Is mimiblewimble-py is node + wallet software?

__anonymous__ :  I think a bit of both, we just need to try stuff, and in general test-cases are most efficient there, but in general people need to compile and play with it.

__renzokuken__ : Yes, but not completed. Part of the node p2p protocol is implemented.


__aglkm__ : Can it be divided into node and wallet modules, so you can use rust node with python wallet?

__anonymous__ : The wallet part has priority IMO.

👍 renzokuken

__renzokuken__ :

>__aglkm__ : Can it be divided into node and wallet modules, so you can use rust node with python wallet?


Yes, you would be able to use external node of your choice.

🔥  anynomous, aglkm, cekickafa

But essential node code is also being implemented, validating txs, handling blocks etc.

__anonymous__ : Ok, with that I want to close the official meeting. Feel free to continue the discussion though.
Thanks for being at the meeting, and hope to see you all next time again. Lets make Grin Great!👋

__renzokuken__ : Thank you, everyone. Happy I participated.

__cekickafa__ : Thank you all.

__cyptsd__ : bye all.









## *TO DO List*


* Grinventions forum post for feedback.




**Meeting adjourned.**