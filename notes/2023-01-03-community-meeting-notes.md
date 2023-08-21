
# Community Meeting Notes January 03, 2023

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact. Meeting lasted 40 min.

### _Community attendance:_

* satoshocrat
* nicolasflamel1
* anynomous
* dtavarez
* cekickafa
* defistaker




# Short Summary
 

- Cekickafa was asked if he contacted community member naive about the testminer, and he replied, "Yes, another community member funded his electricity costs"
- Python cffi secp256k1-zkp wrapper - bounty. The code has been cursorily reviewed and the tests are present, but have not yet been initiated. 
-The distribution of the Python Wrapper bounty has been unlocked and give to nicolasflamel1 due to inactivity and lack of response by @walkbackgod.
-Community Council will be sponsoring a meme contest to the amount of $5-$10 payable in Grin.
- Discussion regarding forum post https://forum.grin.mw/t/minimalism-in-spending-of-the-community-council/10228 regarding minimization of spending from the CC.
- Anynonmous will reach out to Renzokuken to ensure the code is complete, David Tavarez will review for completion as well.


# Agenda Points & Actions
 

* Last meeting notes here: https://github.com/cekickafa/agenda/blob/main/notes/2022-12-20-community-meeting-notes.md

* Current meeting [agenda](https://github.com/grincc/agenda/issues/77)



__anynomous__ : Lets take 1 minute to read todays agenda☝️, if anything needs to be added to the agenda, let us know.
@cekickafa, there was one TO DO I think from last meeting. Did you contact Navi about the testminer (or was it someone else who needed payment)?
EDITED
__cekickafa__ : Yes, contacted and request for funding @naive closed. A community member paid him for electricity costs.
__anynomous__ : Perfect, than that TO DO has been done.

Lets move on to the first topic of today:

## 1) Python cffi secp256k1-zkp wrapper - bounty.
https://forum.grin.mw/t/locked-python-cffi-secp256k1-zkp-wrapper-bounty/10030/5
Is Renzokuken here? I did have a look at the code and I saw a nice number of Tests and a decent amount of code, but I have not tried to run the code myself or test it.

__cekickafa__ : He is absent now i think but code is there, some contributions, nice to see👍

__anynomous__ think we need two formal reviews before paying out, but based on everything I have seen I do not think that will be any issue.
Regarding the distribution of the bounty, to me it looks logical 100% of the bounty will go to @nicolasflamel1. Walkback god has our thanks for initially taking this up, but since 1) he only contributed a little and 2) he disappeared without communication and 3) the nature of a bounty is all or nothing or a checkpoint, I think it is only fair that @nicolasflamel1 will claim the full bounty of 10k$ in BTC. Orriginally a 10% payment in Grin was proposed but since the CC is low on Grin funds, I propose the bounty will be paid in full in BTC.

Please upvote if you agree, if you think this is unfair to Walkback god, please let us know by downvoting or providing your arguments here in the comments.
👍 defistaker, nicolasflamel,tromp,jdavies, cekickafa 

__cekickafa__ : Well, i pinged  @walkbackgod twice. I would like to hear from him also but couldnt. Thats all i can say. He seemed interested with Grin, maybe he joins again.


__anynomous__ : I think so, probably life just happened, and not everyone checks every communication channel frequently. In any case, he has our thanks for taking on this bounty innitially, hopefully we will see more of him/her in the future, just like I hope we will see more from you in the future 


__@nicolasflamel1__ : I plan on sticking around for a while. It's been pretty fun so far.
👍 anonymous, trinitron, jdavies, cekickafa, defistaker




__dtavarez__: I think it can be paid. The pip package is already published.


I would like to propose to donate 100 Grin to this meme contest (something like 7 dollar in value currently)

@dtavarez Have you tested it? 

__anynomous__:    I only browsed the code, but did not run any tests.@dtavarez Have you tested it? The test cases are there I think, mostly we just need to run those.

__dtavarez__: 

>__anynomous__: @dtavarez Have you tested it? I’ll do it, I actually want to test it anyways
The test cases are there I think, mostly we just need to run those.

Not yet, I could dig more and write some test
I’ll do it, I actually want to test it anyways

## 2) CC sponsoring the 2023 meme contest (5-10$) in Grin https://forum.grin.mw/t/2023-meme-contest-anything-goes-just-have-fun-meming/10254



__cekickafa__: i already donated 500 grin to ipollo campaing for test miners, but i will donate also. :)


__anynomous__:  Please upvote or downvote this proposal:   keybase://chat/grincoin#general/56143
Any donation is welcome, in the end many small hands make lightwork and many small donations make a nice price pot.

__dtavarez__: 

> __anynomous__: Any donation is welcome, in the end many small hands make lightwork and many small donations make a nice price pot.

To the CC’s wallet
Right?

__anynomous__: @cekickafa @satoshocrat and others, feel free to share the contest in newsletters and on social media.
Nice thing is that we do not need to vote on this as whole CC since we decided to me more easy going with microfundings.
With that we can move on to the third and last topic for today:

## 3) 3) Call to action: collect feedback about CC spending.






__anynomous__:  I proposed on the forum to minimize Grin spending until Bitcoin has gained a bit in value, e.g. more than 30k.
Please provide your opinion on this topic, preferably on the forum for transparency.
The main idea is to only fund PIDB implementation in Grin++ and nothing else for now, maybe some minimal amount for Grin CC administration, but everything else may be dropped for the time being or taking up voluntarily.
Existing bounties are of course paid normally.



__dtavarez__: this is very simple, I would like to invite more people to join the discussion on the forum https://forum.grin.mw/t/minimalism-in-spending-of-the-community-council/10228

__cekickafa__: Well, this applies to all community. There is nothing wrong about taking conservative measures.

__anynomous__ : I agree, in the long run this will really benefit the project and the community while just being saving for a short while.

__dtavarez__:   my position is to keep the development train moving


__anynomous__ : I think we can make an exception for CoinSwap implementation as well. We can have that discussion when he finishes milestone 3. But in general, I do not think Bitcoin will stay long below 30k, so I do not think the project will have much time to spend in this maintenance mode.






__satoshocrat__: Post CoinSwap's 3 milestone completion and bounty fulfuillment/testing, would this also include a stipend for wallet integration? Could that be funded from the OC fund? I don't want to assume Scilio is going to be around and willing forever to see the full vision implemented, nor do I want CoinSwap to stall before integrated imo

 Why is it not being funded from the OC fund anyway?  at least partially?


__anynomous__ : But for @dtavarez it might be inconvenient, I think you might for 1 or 2 quarters to rely on you daytime job for income.
Luckily you have nearly 5 months to look for the right income source.

__cekickafa__: We must take into account the possibility of a prolonged bear market as well as any other possibilities

__dtavarez__ : what I've been trying is to boost the development as much as I can before taking it more slowly.

👍 anonymous

__defistaker__ : It is good that you have 5 months to boost 👍

__anynomous__ :  Same for our groundkeepers, @cekickafa @satoshocrat . I know this might be inconvenient, but you know it now while having 4-5 months of funding

__cekickafa__: Well, this applies to all community. There is nothing wrong about taking conservative measures.

__anynomous__ : I agree, in the long run this will really benefit the project and the community while just being saving for a short while.

👍 cekickafa

__cekickafa__: I am committed to Grin, and do my best as much as i can do.

🚀 anonymous

__dtavarez__ : but my position remains the same: the funds should be dedicated to the development of Grin, and we must keep it that way

__anynomous__ : We will, we will just be strategic about the timing and impact of the funds.
I think that is all for today. If there is anything more, please bring it to the discussion now.

__dtavarez__: I do not feel OK deciding what is important and what is not, that's why I keep bringing the Post 5.0 wish list
maybe we should review the list and add bounties
create bounties based on that list
and keep the funds open to long task like PIBD implementation

__anynomous__: And if not, I would like to thank you all for your input today. Do not forget to provide feedback on the forum and contribute memes:
https://forum.grin.mw/t/minimalism-in-spending-of-the-community-council/10228/21
https://forum.grin.mw/t/2023-meme-contest-anything-goes-just-have-fun-meming/10254/3

Community members can look at thie post  5.0 wishlist and use it as basis to provide their feedback on the minimal spending proposal, which features should we make exceptions for and fund right away?
Probably 90% of the community will say PIBD and CoinSwap should be exceptions, but I let everyone decide that for themselves and provide arguments on the forum
EDITED
Cya all in the next meeting in two weeks from now, till then have fun meming 😊


## *TO DO list*


 * Anynonmous will reach out to Renzokuken to ensure the Python Wrapper code is complete; David Tavarez will review for completion as well.


 

**Meeting adjourned.**