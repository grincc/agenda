# Community Meeting Notes February 13, 2024

Community Council (CC) meeting held @ 14:30 UTC in grincoin#general channel on Keybase. Meeting lasted 45 min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.




### _Community attendance:_

* anonymous
* cekickafa
* renzokuen 
* waynegeorge

# Short Summary
 
 
- Open discussion about ironbelly mobile wallet. New design ideas from @waynegoerge has been talked.
- Grinvention/mimblewimble.py implementation funding alternatives has been discussed.



# Agenda Points & Actions
 

* Last meeting notes here: https://github.com/grincc/agenda/tree/main/notes

* Current meeting [agenda](https://github.com/grincc/agenda/issues/125)



## Ironbelly wallet status


__anonymous__ : It has been rather quit from the community in the last couple of months, perhaps because the price is going up, so suddenly there are less complains 🤔 .
Would be nice though if the community brings in topics for discussion ones in a while. I assume there are still tools they need or would like to see in the project.


__Cekickafa__ :   Well it is the quitest despite Gui wallet
I dont know if it is good or not.


__anonymous__ : Yes, perhaps that satisfies all their needs... in any case it is a good development even though it is only alpha release for now.
Not sure either
Well, there are also some community initiatives, e.g. the betting app, even though that is just a thought for now.


__Cekickafa__ : It is a very good idea. It will certainly attract people.


__anonymous__ : It is good to play around with transactions, just for fun. As long as they use the blockchain to verify bets.


__Cekickafa__ : Anyway it is a real use case. Like it or not. People like gambling.

__anonymous__ : Would be even better if it is non-profit, but I am not sure if that is what God had intended, or that he wanted to accumulate a bit of Grin.

__Cekickafa__ : Non profit not really works imo:)

__anonymous__ : I am happy to know that at least the Open Source HW wallet idea I had has some merrit since it can be done safely:
keybase://chat/grincoin#general/62818

for me it strengthens the idea that we need to develop mimblewimble.py since it can be used for that HW implementation.
💯 cekickafa




__renzokuken__ :
Hey guys.

sorry for being late, I was actually on time but started to read something and missed the keybase activity

👋 cekickafa, anonymous

__anonymous__ : no problem, happens to me a lot as well.
🙏renzokuken


Did you already think a bit about the Funding Request, if and when you would like to make one?

__renzokuken__ : Yes... Unfortunately, I am having some second thoughts about it.

__anonymous__ : Or an alternative, funding format request.
That is alright, tell us your "second thoughts " 😉


__renzokuken__ :  I haven't really worked on ツ for a while and I almost forgot why I did not apply for funding and started grinventions instead. After our last discussion I started to research how to make funding request and draft it and I remembered why I never done that.

__anynomous__ :And what were the reasons you remembered?

__renzokuen__ : Most importantly, independence. Grinventions development is slow, extremely slow, because of lack of funding mainly. But grinventions is truly independent, has its own vision of ツ and own roadmap which aligns with what community wants (payment engines for ecommerce shops, multiple languages implementations, easy to read source code, betting software, Telegram bots etc).

Lack of funding is price to pay for being independent and a ticket to openly disagree with core development choices.

I checked previous funding requests, hourly rate is tempting and it would be nice to have that amount of ツ, but I don't want ツ to be bunch of leafs all coming out from same root, finance-wise. I think it is important for there to be an entity which is not funded from the core nor CC.

That was big reason.

Small reason is simpler - accounting. There is no entity to invoice, even if I apply for funding, that would be a traceable income which I cannot declare. If I fund grinventions from donations, payments are secret and government can't accuse me of having an undeclared income.

__anynomous__ : Ok. Make sense.
Sometimes the better road is the harder one. Same reason why I also always rejected any ideas of being funded, because it thought it would not be good for the project.
__renzokuken__ : Maybe if I haven't joined this community with my real name visible to the public, I could apply for funding and noone could trace this back to me, but it's too late for that.
There are ways to declare income from unknown sources, but it's expensive and most of that would be lost.

Any developer, who accepts crypto funding just so that most of that goes to government in form of taxes is acting against the ツ philosophy in my opinion. I openly disagree with that.
__anynomous__ : Perhaps the CC could consider making a donation on "good faith" to grinvention, it would be hard to put "deliverables" on such a donation, but perhaps some requests for functionalities can made. I am however not sure if others are open to that idea. 
I do not think this is retrospective funding, nor is strictly a funding request, it would be simply "a donation" with a message attached to it, like things CC and or community would like to see in the future.

__renzokuken__ :I will still deliver the milestones, I will accept donations, instead of 120K-140K ツ I will get maybe 5K ツ, but I will not hate myself for braking my own principles.

👍 anonymous, cekickafa, nicolasflamel

__renzokuken__: 

>__anynomous__ : Perhaps the CC could consider making a donation on "good faith" to grinvention

The donation addresses are public. Anyone can donate. There is no obligation to do so, but all donations are appreciated.


__anynomous__ indeed. I think the biggest hurdle here is seeing if both community and other CC members are onboard with such an idea. I think indeed it would be a smaller amount that any funding request would ever be, due to it being more risky/no-clear deliverables or output for community, but it would be a welcome contribution I assume.

__renzokuken__ :I joined this project because I believe in it, not for income.
__anynomous__TO DO for me to create forum topic to get feedback from community and other CC members. We will see if there is any support for it.

__renzokuken__ : No pressure.
__anynomous__: I think your past work at least provides a lot of merit to the idea. No worries, I feel no pressure, I just think it is worth as shot, because I believe as well mimblewimble.py would be in the best interest of Grin as a project.

💯  renzokuken , cekickafa 🤝  renzokuken

__cekickafa__ Well python implementation is important for adoption imo. Hope to see completed very much.
👍 renzokuken

By the way. This keybase crushes again for me. Sorry for delay.
__waynegeorge__ Hey guys,I wanted to bring up the topic of mobile apps. I'm aware that Ivan has limited ability if any to maintain Ironbelly so I think it's becoming more urgent
I guess user experience in general

__renzo__ This is a good point, have you tried to reach Ivan and discuss it with him? Do you know what are his thoughts on that and future of IronBelly?
__cekickafa__What you mean limited ability? I think limited time he said.

__waynegeorge__ : I did email him. I responded to my first email, but not my follow up


___cekickafa__ : Anonymous replied him at forum. He didnt respond yet

👍 renzokuken

__waynegeorge__ : It's hard to share ideas without them sounding like pipedreams but I have recently started SwiftUI development and am prepared to look at either refurbishing IronBelly or a complete remake. In reality it would be some time away still but I already have some ideas down

__anynomous__ : Ok, sounds interesting. Is there any specific reason you would want to remake or revamp IronBelly?

__waynegeorge__ : I think for iOS in particular, a native app would provide a better UX

__cekickafa__ : not android?

__waynegeorge__ I also wanted to experiment with P2P transacting with other means
such as multipeer
I guess yes, it would be better if there was a matching Android version
I thought it would be a great opportunity to look at the crypto user experience as a whole. I think one reason that grin is less well known is that the UX on CEXs is much better than native crypto apps
I know this is a big conversation

__renzokouken__ : @waynegeorge is it difficult to integrate javascript code into app written according to your design? I am asking because I would like someday to translate my python code into js to have something similar to what Nicolas Flamel did with his mimblewimble code.


__waynegeorge__: It is possible although I'm not yet aware of limitations, etc

👍 renzokuken

__cekickafa__ : So you want to upgrade ironbelly with contract style tx as in Gui wallet @waynegeorge ?
Sorry my lack of understanding.

__waynegeorge__ : I'm not sure what contract style is but my vision is for a process where a send amount is set, a nearby peer is found either using bluetooth, nfc, wifi, etc, then the interactive transaction takes place
iOS have a MultiPeerConnectivity framework. I'm sure it's even easier on Android
__cekickafa__ : Ok, that is about broadcasting. That is similar to grin++ node+wallet mobile?

__renzokuken__ :

>__waynegeorge__ : I'm not sure what contract style is but my vision is for a process where a send amount is set, a nearby peer is found either using bluetooth, nfc, wifi, etc, then the interactive transaction takes place

is your wallet also going to run a node? I though for a wallet you only need to reach your node, multi peer connectivity doesn't seem to be important for that (correct me if I'm wrong)

__waynegeorge__ : I like the idea of light app to start with
so remote node

__cekickafa__ : Ironbelly uses remote node now.

👍 waynegeorge

__waynegoerge__ :possibly a way to pair it with self hosted node with an easy deployment process
__cekickafa__ : Well, if you define and explain it on forum, there will be more engagement about your idea. Maybe under ivans forum post.https://forum.grin.mw/t/future-of-ironbelly/10859

👍 waynegeorge

__waynegeorge__ : I guess crypto is currently only used by geeks or normal folks with access to them via CEXs. I'd like to make it easier for normal folks to use

👍 renzokuken, cekickafa

__cekickafa__ well, we better take @i1skn thoughts about this also. You said you mailed him, continue with forum spotlight.

__waynegeorge__ One last thing that just came to mind for @renzokuken, perhaps you could do the work in your name via a company that you create? Then you could legally take out funds from it in the most tax efficient way for you

__renzokuken__ Thank you for reaching out about this. Unfortunately I can't, to accept payment I need to invoice to someone, but CC is not a company neither a person, cannot be invoiced.

__waynegeorge__ Could CC create an official organisation? would it even want to is the first question though lol

__anynomous__ the answer is no 😛

__cekickafa__ it would be risky

__wayngeorge__ I guess people can just become ghost devs 😉

__anynomous__ @waynegeorge If I understand it correctly, you want to remake or edit IronBelly to purely work without any online interaction. The question is if this is not already possible. I mean a QR code is offline right? So if you create a slatepack message and show the QR code to the other party, it should all be offline. Only part online is when broadcasted.


__waynegeorge__ The online part will need more thought but I do have some ideas, Yes the QR method already woks but I was just looking at ways to make the process smoother

👍 anynomous.












## *TO DO List*


* 




**Meeting adjourned.**