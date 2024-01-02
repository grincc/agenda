
# Community Meeting Notes November 07, 2023

Community Council (CC) meeting held @ 18:30 UTC in grincoin#general channel on Keybase. Meeting lasted 72 min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.




### _Community attendance:_

* future3000
* grinreaper
* ardocrat
* anonymous
* cekickafa
* phyro


# Short Summary
 
 
 -  Grin 2020 wishlist items and possible developments are being discussed.
 - Atomicswap development has been discussed; @Grinreaper volunteered for development. Topic is to be discussed at #dev channel by core developers.
  
 - The lack of manpower for Grin repository development and bug fixes has been mentioned.

# Agenda Points & Actions
 

* Last meeting notes here: https://github.com/grincc/agenda/tree/main/notes

* Current meeting [agenda](https://github.com/grincc/agenda/issues/115)



__anynomous__ : I was hoping on some more CC members joining...
We will see, they might join in later, for some of them it is early morning.
I just pinged them on Telegram..

__cekickafa__ : Well, on forum posted also 2 days ago. it stays on top.


__anynomous__ :  Yep, anyhow, giving the opportunity to join is all we can do.
Regarding last meetings;

## TODO



Regarding last meetings #TO DO's, we had to update the status of the various items on the wishlist. I updated them and let yeastplume gave it a quick review. I will post his feedback here:


_*Payment proofs are in the contracts branch of the wallet code. They're being created by the GUI wallet at the moment during a transaction, but there's just no way to view them at the moment (coming soon). The relevant PR is here https://github.com/mimblewimble/grin-wallet/pull/681

*tor support for nodes, I'm not sure where that came from, I personally wouldn't rate it as being highly important (detrimental even because you want changes to propagate as fast as possible). Light node I have no idea, it still looks very theoretical. Binaries for older systems/low ram machines isn't something I'd be likely to be focusing on.

*flyclient's always been a theory, don't think much work has been done on it since by anyone
*rest I think is more or less okay, on radar at varying distances_

Here is a link to the updated wishlist with the status of the various features:
https://github.com/grincc/hub/blob/main/wishlist.md

Update since the last meeting, thanks to @johndavies24, is that bulletproofs+ were audited on Tari. That is a good step forward in creating more trust.. The reason not to implement them in grin yet was that they needed more time testing. If there would be an exploit, that would have been very bad for Grin (inflation bug), hence the need to be conservative and first wait for the tech to be audited, tested and proven safe..

👍cekickafa


__cekickafa__ : #TODO one item was Mwixnet testing, but we are unable to operate here, becuz of lack of some instruction and engagement.

__ardocrat__ :

>@scilio:
i was just waiting to see if there were any more comments on the code. if there's not, I will get reorg out for review this week


we are waiting for reorg to test :)

__anynomous__ : I also did not get far yet. I asked @johndavies24 for Testnet coins, he has them in abundance, but my virtual machine got corrupted, tried new Ubuntu version which got some problems with some dependencies for Grin. I am still sorting that out.


__ardocrat__ : will be interesting to reproduce reorg.


__anynomous__ : Definetely..
Also wonder what happens if you cancel, or spend the outputs before they arrive on chain, how that is handled.

👍ardocrat

@ardocrat you did the most testing for now, can you summarize what kind of tests you did?

__ardocrat__ : yeah, had problems with cancelling, when funds were already sent, wallet repair required after

__anynomous__ : A, damn, that bug again.


__ardocrat__ :

>__anynomous__ :
@ardocrat you did the most testing for now, can you summarize what kind of tests you did?

nothing special, just debugged at code how it works with wallet API

__anynomous__ : Did you run in any errors/unexpected behaviour?

__ardocrat__ : not yet :D
I stopped testing when got response @scilio will add changes

__anynomous__ : Good. Well it is great you have some experience at least, then you can provide tips and tricks on getting it to run.
What is needed is a normal node running testnet and a wallet right? or is the mwmixnet itself already a testnet node?

👍ardocrat

__ardocrat__ : At least now I understand how it works :)

👍 anonymous

__anynomous__ : That is more than us.

__ardocrat__ : wallet and mwixnet server

__anynomous__ : on which flavor of linux did you test?

__ardocrat__ : node of course, as we need testnet

__phyro__ : a forum post via a clean gui on how to test mwixnet would be welcome :)
guide*

__anynomous__ : I agree, to me at first glance it still looked vague, like what steps do I actually do for testing.
Can figure it our of course, but a forum post with some example tests might be illustrative and usefull.

__phyro__ : regarding bp+ audit, I suspect that if bp++ were possible on Grin, we'd likely just skip to bp++ variant to avoid adding bp+ and another potential risk
bp++ is an improvement over bp+ which is an improvement over bp that we use

__anynomous__ :  A, great to hear. Because I was even unsure on whether we were waiting for bulleproof+ or bulletproof++.

__phyro__ : but it seems unlikely that we touch this soon. Lots of other things to prioritize probably

__anynomous__ :  I agree, it is just nice for the long run but not of any practical relevance for now.

__ardocrat__ : 

>__anynomous__ : on which flavor of linux did you test?

distro? I am using last Arch, after updating had problems with building for last gcc, we merged croaring changes to grin node repo, but grin-wallet is still using old crates with 0.4.6, I guess we can do it at next release with @yeastplume

👍 anonymous

__anynomous__ : Do you now why running a node on tor was a priority 1 on the Wishlist? @yeastplume criticized it.
I am not sure of the history of it being there although I personally would like to run a node via tor.

__ardocrat__ : some deps need to be updated for mwixnet as well.

>__anynomous__ : Do you now why running a node on tor was a priority 1 on the Wishlist?

it was suggestion by @dtavarez

__anynomous__ : Ok, I have issues on Ubuntu 22..04 with libncursesw.so.5. There is a fix with creating a link to libncursesw.so.6, but it does not work on 22.04

__cekickafa__ : So multisig is far and away?


__anynomous__ : a updated snap package would solve that, but unfortunately the last release is a two years old
As I understand it, yes.

__ardocrat__ : 

>__cekickafa__ : So multisig is far and away?

new bulletproofs are needed as I understand.

__anynomous__ : "multi-sig* -Not happening any time soon if I understand correctly, since there is no solution yet to generate threshold range proofs:

"This is based on what I found on keybase, do you know if the above is correct @phyro?
Multisig is one of the things I would like to see in the comming 2 years.

 For one simple reason, I think it might be usefull for a lot of ecosystem projects, e.g. an open (source) HW that is used in a 2 out of 2 multisig, using a single mnemonic as output for example.


👍ardocrat 

If that is reaslistic at all, no idea 🤷


__cekickafa__ : Which ones on wishlist needed Hardfork ?
bidirectional payment channels?

__phyro__ : I don't think I've heard of a threshold rangeproof solution for bps. I think I've heard a n-of-n one, but I never dove into that. The thing is also that MW signs twice, on outputs via rangeproofs and on kernels via schnorr sigs. I guess you could do musig2 on kernels, but I've no idea about this on rangeproofs

__ardocrat__ : Yeah, I read this https://tlu.tarilabs.com/protocols/mimblewimble-mb-bp-utxo#mimblewimble--ntext-of-n--multiparty-bulletproof-utxo

👍 anonymous, phyro

__anynomous__ : I agree, it would be for me the next thing after that. Nice if it is possible, but probably it would require a lot of discussions and a lot of work... which I am unable to do 😆
Ok, I think with that we are leaving the first topic on our agenda, and already discussing the next one:

## 2) Grin Ecosystem wishlist, were are we now and where do we want to be in 2-4 years.

__cekickafa__ : Gui wallet and tx without problems maybe in  2-4 years?

__anynomous__ : For me, if we get contracts, GUI, biderectional-payment proofs and Coin-Swap working in the coming years 🙌 , if we get more working, e.g.  multisig, or atomic-swap 🚀 🙌 even better, but only a bonus since it enables some extra ecosystem projects

👍 phyro

Ya, I do would like to have the basics working, you know cancelling transactions, or hanging transactions in both grin-wallet or grin++ should be a thing of the past.

__phyro__ :  most importantly, we need people to read and contribute code

👍 anonymous,  %100 ardocrat

__anynomous__ : Yes, that would be something to put on our wishlist 😉  Maybe priority 0
I can't make any promises, but at least I am learning rust, which might mean I can actually handle a bug in the future, nothing too ambitous though, I can only work on Grin in hobby time.

__cekickafa__ : 

>__phyro__ :  most importantly, we need people to read and contribute code

that is a problem since 2020, how can we solve this ?

__future3000__ : Hi guys!

👋 👍 anonymous, phyro, cekickafa

__anynomous__ : I guess crypto wizards who know rust and are in it for the project itself are just extremely rare

__phyro__ : yeah. Hopefully as software matures and gets simpler to use, it also gets easier to test and see why Grin is interesting

__anynomous__ : I do think we have a chance of getting some people who are now on the periphery to get a bit deeper into the code and as such able to help a little at least.
O and great thing to have you with us nowedays @ardocrat 🙏  You already took on some bugs.

💗ardocrat 👍 phyro

__phyro__ : non-core contributions are also a great way to keep the community engaged. It can be blogs, paintings, merch or whatever else

ardocrat 👍 

__ardocrat__ :

>__anynomous__ : I do think we have a chance of getting some people who are now on the periphery to get a bit deeper into the code and as such able to help a little at least.
O and great thing to have you with us nowedays @ardocrat 🙏  You already took on some bugs.

I am happy to contribute when I have time, I am building GUI too, just fixing all bugs on my way to have better experience with it to not have a lot negative when I will publish it at all stores :D

👍 anonymous

__anynomous__ : I agree, I mean I love lovely grins work as well as Nirgs wallpapers for example, these kind of things to help us all keep up motivation. I think to many people forget that they can actually contribute in whatever way they want

__phyro__ : yeah, exactly

__anynomous__ : Any ideas on how we can get our average community members to engage more? I mean we tried subgroups.... quite a few times... did not work unfortunately.

__phyro__ : people just have to stop waiting for others to do it and become proactive

__anynomous__ : Fully agree there, perhaps we should use Telegram more actively to encourage people to come to the forum. I think a part of the problem is that they just stay on Telegram. I mean I did see a lot of great memes and Gifs there that never made it to the forum.

__ardocrat__ : just do it, testing helps a lot, learning Rust too :D

👍 anonymous

__phyro__ : it's really that simple :) lovelygrin is a great example of this. If you can paint, paint a picture 🤷

__cekickafa__ : 

>__phyro__ : people just have to stop waiting for others to do it and become proactive

what people ?

__ardocrat__ : grinpixel by @future3000 is great idea too

👍future3ooo

__anynomous__ : Exactly, ... it is so simple that I feel like we should not even have to encourage it at all, somehow those people came in in the early years and now are just not active anymore, not sure why.
Yes, I love that idea as well.

__phyro__ :

>__cekickafa__ : what people ?

whoever has time and wants something to happen I guess

ardocrat 👍 

__ardocrat__ :

>__cekickafa__ : what people ?

from forum I guess, some of them I met at Telegram


__cekickafa__ : 

## 3) About Atomicswap:
 We have a volunteer @grinreaper, i contacted him and asked if he can join the meeting, he said he will try to join later time hopefully. He wanted to engage about atomicswap last year feb 2023. Forum post to remember.
 [forum](https://forum.grin.mw/t/questions-about-the-state-of-the-atomic-swap-pr-and-introduction/10332/6)


__anynomous__ : I think we somehow have to get more people in from Telegram to forum, perhaps an Arts contest?

__cekickafa__ : nobody replied that guy on forum even ? What are we talking here ?

__anynomous__ : With some fun bounties, just to get people over the treshold. If they see their works are appreciated, some will just keep contributing.

__ardocrat__ : I feel like forum has more unique people

👎🏻 cekickafa

__anynomous__ : It does, or at least more techy people, but I think for every 10 Telegrammers, there is at least one potential great forum contributer.

__ardocrat__ : @cekickafa seriously, look who is writing at Telegram and forum, last time I see more new people at forum, reporting bugs and so on

__cekickafa__ : i think Grin prisoned into forum, and you expect a large community people, engage, test and code. That is exact opposite.

__phyro__ : it might be good to avoid bounties for things that can be done out of fun

__ardocrat__ : I am sitting at Telegram a lot time
@nonia is about to build bridges

__anynomous__ : The thing is many on Telegram just want to monitor or think they cannot contribute, those who already joined the forum mostly are already one step further in wanting to know and contribute to the project. It is nothing against Telegrammers, it is just one more step of commitment to make a forum account. Same for KeyBase, it is an extra step, so only those who are serious do it.

__grinreaper__ : 

>__cekickafa__ :  About Atomicswap:
 We have a volunteer @grinreaper, i contacted him and asked if he can join the meeting, he said he will try to join later time hopefully. He wanted to engage about atomicswap last year feb 2023. Forum post to remember.

 Hi, I have been working a good amount on implementing the swap on some other chains that I am already very familiar with in terms of scripting. For grin I am not super comfortable with it yet and am not sure about best practices and expectations for how it should be implemented. Any ideas as to where I should begin would really help. Should I write up a RFC first?

 __ardocrat__ : We have some problems with Multisig..
Its requirement for swaps/dexs

__cekickafa__ : 

>__grinreaper__ : Hi, I have been working a good amount on implementing the swap on some other chains that I am already very familiar with in terms of scripting. For grin I am not super comfortable with it yet and am not sure about best practices and expectations for how it should be implemented. Any ideas as to where I should begin would really help. Should I write up a RFC first?

thank you passing by, you asked last year those questions on forum. And we were talking why we dont have enough people.

__anynomous__ : Yes, at the moment the workaround that Bisq uses is to use a public API for payment proofs, to verify a payment and using a collet oral of BTC for the Grin holder, which is returned ones the transaction is confirmed.

__ardocrat__ : Bisq is more like P2P, not true DEX

__grinreaper__ : one side of the implementation of the atomic swap only requires a scalar pre image, is that do-able?

 
__anynomous__ : I do not know what a 'scalar pre image'  is, so I would have to look into it.

__grinreaper__ : Basically like a ephemoral private key

👍 anonymous

__anynomous__ : Perhaps better discuss this on the forum, or in the #dev channel.

__grinreaper__ : ok

__anynomous__ : I think ephemoral keys should be possible, basically it is sharing the key directly, the problem is there would be no payment proof, so how to avoid the sender from getting scammed.

__ardocrat__ : 


>__anynomous__ : Perhaps better discuss this on the forum, or in the #dev channel.


#dev channel is good place

__anynomous__ : In any case, it is good way of thinking to just share the key, it simplify things on the swap side, but complicates a bit on the wallet level, need to send the keys to a seperate account with ephemoral keys for swapping for example.
Best to move this discussion to the #dev channel.
Anything else we need for the comming 4 years? I would like to see the Testnet faucet/Telegram bot from @renzokuken working. But that would require a new bounty. Old bounty is in Grin and... well we all know what happened to the price 😜

💯 cekicafa

__grinreaper__ : responding in the dev channel


❤️cekicafa ,anonymous

__anynomous__ : I think we can close the agenda, but feel free to brainstorm and contributes ideas on what we would need for the coming 2-4 years.
Also ideas to bring in more people, or train more devs, bring back motivators such as artists etc. All ideas are welcome.

__phyro__ : 

>__cekickafa__ : thank you passing by, you asked last year those questions on forum. And we were talking why we dont have enough people.

I had in mind people contributing to grin-wallet or grin repositories.

thanks 👋

__anynomous__ :
@phyro Any idea on how to pull people over the treshold? I think a part of the problem is that in the beginning a group of people started to evolve/develop to keep up with the projects. Those who did not do so yet, have hard time making that jump (also there are not many that can make that jump).


__phyro__ : it's much easier to dive into things when the community is more active and many other people do so as well

__anynomous__ : I do not know if you get what I mean, what I mean is that eh core devs kept developing at a great pace, making them even greater wizards which might seem unattainable by the rest of the community, and especially those who join new.
Exactly, like in the early years, the forum was and keybase was like a continuous learning platform.

ardocrat,  phyro👍

__cekickafa__ : 

>__phyro__ : I had in mind people contributing to grin-wallet or grin repositories.

Noted.

__phyro__ :
oh, I don't think the project is much more complex. Grin core has, for the most part, stayed the same. There's things like PIBD and other improvements, but the core is mostly the same

__anynomous__ :
I know it got me startled at times, but it was great since you could learn at a fast pace. I feel like I unlearned as much as I have learned about crypto in the last years, especially since becoming a CC member.
It is not the project that I mean got more complex, what I mean is that the majority of peope did not keep up or forgot. It is like I said, I forgot a lot of the essentials because of working on governance for example instead of looking at the rather great documentation the project has.
Perhaps we need something like a technical newsletter or nesflash
But I see the problem already, who is gone make it.

__phyro__ :
hmm, if people have questions, ask them here or on the forum. It can serve as a spaced repetition for many

__anynomous__ :

Ya, I should get the habit again of asking. Answers are not only usefull to me but also to others.

__phyro__ :
there's lots of docs on the grin repo that can be used to learn. And when people get stuck, ask on keybase or forum :)

__anynomous__ :
it takes time to learn, but a motivated individual can definitely push through
On that note, do you know what the rewind command does, last time I tried it gave an error, so no idea what it actually supposed to do. Rewind a couple of blocks or something?

__phyro__ :
is that on wallet or node?

__anynomous__ :
I think node
Have to check. Sorry, got to go

__phyro__ :
on the wallet side, we have

  - rewind_hash:
      about: Return the hash of the wallet root public key.
  - scan_rewind_hash:
      about: Scan the UTXO set and return the outputs and the total of grin owned by a view wallet rewind hash.

which is kind of like a viewkey. You can scan which outputs you own, but can't spend them with this rewind_hash afaik

ardocrat, anonymous👍

__ardocrat__ : 
When we will fixs bugs and optimize some things, we can integrate Grin everywhere and make tools for this by wrapping native rust modules for different frameworks/languages, Like @renzokuken did for Python.

I remember he had idea for custom slatepacks format to use them for 2fa, can not find this info, tried at search.. maybe he will come back, it will be great to have him here again.
>__anynomous__ :
I think we can close the agenda, but feel free to brainstorm and contributes ideas on what we would need for the coming 2-4 years. Also ideas to bring in more people, or train more devs, bring back motivators such as artists etc. All ideas are welcome.

👆

>__phyro__ :
oh, I don't think the project is much more complex. Grin core has, for the most part, stayed the same. There's things like PIBD and other improvements, but the core is mostly the same

Debug is helping a lot to understand how things work, especially if it needs to reproduce a bug/problem, unconfirmed txs made me to go deeper into tx flow to watch every step, so I can say problems are motivating to learn things inside not just on API level :D



## *TO DO List*

* Grin unconfirmed tx and users cancel problems topic not discussed.
* Mwixnet community testing








**Meeting adjourned.**
