# Council Meeting Notes July 06, 2021

Third (CC) meeting held @ 3PM UTC in grincoin#general channel on Keybase. Meeting lasted 60 min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendence:_ 

* __anynomous__
* __mark_hollis__
* __mo5itoo__
* __dtavarez__
* __cekickafa__
* __defistaker__
* __joltz__
* __dburkett__  
* __phyro__
* __vegycslol__


<br/><br/>
## Agenda Points & Actions
<br/>

### 1)  Funds transfer from core to cc
<br/>

* __anynomous__ : We did not yet receive any news from the OC when we can expect the funding in our wallet.
So I guess we should make this an action point now the CC for the next CC meeting.
No OC members present here by any chance who can update us 😉


<br/><br/>

###  2)  Status of PR#606
<br/>
 

* __dtavarez__ : PR#606 https://github.com/mimblewimble/grin-wallet/pull/606
was an issue or request made by an exchange
here's the issue https://github.com/mimblewimble/grin-wallet/issues/595
* __cekickafa__ : made by an exchange i think
* __dtavarez__ : correct
* __mo5itoo__ : Hotbit exchange
* __cekickafa__ : it was talked about lehnberg time at 2021 february somewhere
* __anynomous__ : Great. In the end this is how we get better software, simply by listening to users.
* __dtavarez__ : the PR is open, all tests are green, but the PR is not merged yet
deevope worked on that
* __cekickafa__ : who can merge it?   __phyro__?
* __dtavarez__ : he commented this: "I suggest to fix before the #607 issue before merging this PR. If this issue is fixed, this PR would need some more code, if not it can be merged."
this is the issue https://github.com/mimblewimble/grin-wallet/issues/607
* __anynomous__ : I see, that is a bit dangerous issue.
 
* __dtavarez__ : I think the PR can not be merged before working on issue #607: Inconsistent wallet transactions state
 
* __anynomous__ : I agree, the 607 issue sounds also rather important to exchanges to me. Nice if they can retrieve transaction by block height, but if that transaction became invalid because of a reorg... well I guess they would like to know 😅

* __dtavarez__ : probably someone could let them know that the fix is not merged yet.
@ __mo5itoo__ do you think you could let them know?
* __mo5itoo__ : Yes i will do that on telegram
* __anynomous__ : Is anyone working on solving the 607 issue?
* __dtavarez__ : I don't think so
* __anynomous__ : Would be nice if we can let them know if this might be solved and as such merged in the near future.
Ok 😅 We need more Devs, that is for sure.
* __cekickafa__ : i think this is egg chicken problem
 


* __anynomous__ : Anyone else wants to comment something on this topic, otherwise I suggest we move on to agenda point 3)
 
* __dtavarez__ : I think we can continue with Community pool

<br/><br/>

###  3) Community Pool
<br/>

* __dtavarez__ : I added to the agenda, but I can't remember who suggested, my bad
* __defistaker__ : I asked if we will continue discussion following last meeting
* __anynomous__ : Ok, well I think we can just give an update.
 
* __anynomous__ : As most people have noticed, Grinmint and  grinnode.live both have a banner saying that Grinmint will change ownership.
@mcmmike had contact with @quentinlesceller to take over grinmint, and apparently they have a deal!

* __cekickafa__ : nice for decentralization.👏
 
* __defistaker__ : ownership will be transferred in october 2021

* __anynomous__ : Which is great news for the community, no need to switch pools. Instead we suggest to beev up grinmint with more hashing power from the community to counter the big pools.
In addition to that, we could also discuss the miners we want to buy as CC. Which we plan to use to mine via grinmint.
 
    We discussed internally among CC members, and although we like decentralisation, having a huge number of G1 minis is also challenging. Therefore, we propose that if we want to invest considerably, we also get a G1.
    E.g. these two options:

    1) 12 G1 mini's +  1 G1, total of 66 chips, equalling 70.02 G/s (estimate cost, around 50.000$)
    2) 12 G1 minis (total of 12 chips, equalling 15.6 G/s (estimate cost, around 11 thousand dollar)

    @mcmmike contacted Nhash

    "Miner availability should be no Problem Just price difference Not Sure If they sell us at the same rate."

    This means that the hypothetical problem we had last time, "who manages all the G1 mini's" is a becoming a real question now.
    I honestly think the community, especially just the CC cannot handle e.g. 42 G1 Minis, but we can handle 10-12

* __dtavarez__ : what I like about this is that we then could count with actually Grins to partially fund community efforts
* __anynomous__ : Fully agree there!
 
* __dtavarez__ : I'm not sure about the other benefits mentioned before

* __cekickafa__ : yes at last Grin will be used

* __anynomous__ : So to explain the motives of the CC a bit more, we want to have 1) a stable income of Grin to use for bounties, community activities etc. 2) We want to help secure the network
The best way to do so is by mining ourself.

<br/> <br/>
### Back to topics (1) Funds transfer from core to cc topic and (2) Status of PR#606 
<br/>

* __dburkett__ : """ quoting   __anynomous__  No OC members present here by any chance who can update us 😉  """ 
@__quentinlesceller__ @__tromp__ @ __joltz__

* __dburkett__ : Oh and @ __phyro__

* __anynomous__ : @ __dburkett__ it would be great if they can update us on this, since without funding, there is not much to manage as CC 😛

* __dburkett__ : Yes, ideally this would not take long. If it takes months to transfer funds to the CC, then I'm not sure how we expect the OC to ever fund any initiatives :/

* __joltz__ : I think folks are preparing/testing hardware wallets etc for the new multisig. Is the CC ready to receive funds? Where can that information be found and verified?
(apologies if already answered, just saw I got tagged)

* __anynomous__ : https://github.com/grincc/finance/blob/main/addresses.md

    I think in addition it would be good to verify with one or two CC members, but what is on the page right now is correct. Wallet as well as disaster checks were made in full so we are certain we all have managed our keys correctly,.

* __joltz__ : Great, will pass it along and help nudge it forward 👍 Are there any CC funding guidelines posted anywhere yet as well?
* __dtavarez__ : Yes,  https://github.com/grincc/docs/blob/main/spending-guidelines.md
* __dtavarez__ : what it will required to prove that the CC is ready?
* __joltz__ : Perfect, thanks. Seems like CC has everything completed and is now just waiting on OC?
* __anynomous__ : Correct.

* __joltz__ : Sounds good, will share these docs and hope we can all complete the required actions as soon as possible 👍

* __dtavarez__ : that's good

* __anynomous__ : Great, than soon we can start funding requests 😁

* __joltz__ : Will update us here once there is a concrete time for xfer so everyone is prepared
 
* __anynomous__ : Great, we will be ready to verify.

* __joltz__ : Hopefully we can have it done before/during next meeting we have here

* __dtavarez__ : @ __joltz__ any thoughts on issue #607 of grin-wallet?

* __joltz__: (assuming regular cadence is still going. have been lurking a bit but obviously not active in the meetings)

* __dtavarez__ : is deev still active?

* __joltz__ : would need to spend some time to step through how it is handled in the code 
last I heard deev was traveling or something

* __dtavarez__ : cool

* __phyro__ : grin-wallet is in need of devs basically. That's all there is, need people familiar with the code to check the changes. Unfortunately we lack here quite a bit

* __anynomous__ : Ok, if anyone knows some rust-devs who might fit the profile, please please please, send them our way 🙏

* __dtavarez__ : just to confirm, we do have enough owners in the github repo to merge any change, right?
* __dburkett__ : Yes, but for some reason @  __joltz__ was missed. He's still just a member, not an owner of the repo

* __phyro__ : We do have owners so merge isn't a problem. The requirement for merge, review from a person that actually knows the code, is the issue
* __cekickafa__ : if owners dont review why they have privilege to merge?
* __phyro__ : I'm ok with merging things I'm confident in, but the wallet code isn't something we should just merge without a careful review (imo)
 
* __anynomous__ : Quick questions, who are actively working right now on grin-wallet? 
Antioch is still active right?, More Devs?

* __dburkett__ : Antioch does not appear to be active anymore. At least not the past few months

* __anynomous__ : Ok, then we are in a tight spot

* __dtavarez__ : it is good to know that the ownership is not an issue, we could try few things to bring more manpower, probably get involved in local communities might help

* __joltz__ : Does CC have a strategy for showing proof of ownership of their multisig published anywhere?

* __anynomous__ : Just a quarterly proof that we have access, and we have all validated the wallet and its addresses.

* __phyro__ : We have a 100% success rate, the last person that posted something on rust subreddit brought us trevyn (though not for long unfortunately)

* __dtavarez__ : probably we could work on this before the next meeting

* __joltz__ : It would be great to have the first proof published before initial xfer from both CC and OC

* __anynomous__ :  We need to update: https://github.com/grincc/security
It is empty now

* __dtavarez__ : I agree


<br/><br/> 

### 3) Community Pool topic (continued)

<br/>

* __anynomous__ : Alright back to topic -> Community pool -> miners

* __anynomous__ : But time to get to topic now. So back to community pool and mining
    1) 12 G1 mini's +  1 G1, total of 66 chips, equalling 70.02 G/s (estimate cost, around 50.000$)
    2) 12 G1 minis (total of 12 chips, equalling 15.6 G/s (estimate cost, around 11 thousand dollar)
    Which of the above options are prefered here, vote by number
    Prices might change, we still need to contact Nhahs for a deal.
    Any thoughts, votes, or is everyone in limbo on which option would be the best 😅
  

* __cekickafa__ : 1
* __mo5itoo__ : I vote for the second option.start small and see how it go
 

* __anynomous__ : There is also an option 3) Meaning we buy 12 G1 minis now, and possible a G1 later
 
* __defistaker__ : The more the merrier, 1

* __cekickafa__ : it has no end. just make it 2 option pls
 
* __dtavarez__ : what if we open a post in the forum? and let people think and express their ideas?

* __anynomous__ : Maybe that is best, there are limited amount of people here.
Good, lets do so and move on.

* __dtavarez__ : cool


<br/><br/>

###  4)  Funding request : https://forum.grin.mw/t/request-for-funding-mwgrin-fr/8888/15
<br/>


* __anynomous__ : So Mohito has requested funding for a range of videos some time ago.

* __mo5itoo__ : Yes i want to provide New ressources for beginners to start with
We Can add the videos to the Doc as an example to see how things works
 
* __dtavarez__ : I see Dog was doing something like this https://forum.grin.mw/t/grin-video-docs-2021/9022

* __anynomous__ : Yes, so there are more people who are interested in making videos.
 
* __dtavarez__ : true

* __anynomous__ : In that spirit, I think we also need a solution or system to accommodate more community members.

* __mo5itoo__ : Yes since i made my request, dog already started doing it hah
 
* __anynomous__ : Yes since i made my request, dog already started doing it hah

* __dtavarez__ : I like the Grin Documentation, maybe it makes sense to attach a video of each topic: Quickstart, CLI Hanbook, Build and Wallets

maybe the use cases can be listed
 
* __anynomous__ : I think the request does really make sense.

    I think that would be step 1) to list the user cases and videos.
    Then step 2) would be to create bounties for these videos.

* __dtavarez__ : if we list the use cases and put the bounty, anyone could join and it could be more open
 
* __mo5itoo__ : I like the ideally

* __cekickafa__ : bounties looks good. best video series win the prize
so we have many videos😂
 
* __anynomous__ : We can create additional bounties for extra prizes, or best effort prizes.
 
* __dtavarez__ : do you agree on list the uses cases and suggest a bounty? maybe we could reach Dog too
it is just a suggestion

* __anynomous__ : Yes, the more the better actually. Same thing with docs. Took me a few explanations of how Grin works before I got it.

* __mo5itoo__ : We Can make a post on the forum announcing the bounty

* __mo5itoo__ : Who will write the post ?
 
* __dtavarez__ ; You could start

* __anynomous__ : And we can add to it.

* __mo5itoo__ : by a suggestion, yes

* __vegycslol__ : Are enough people from cc fund for this bounty? Just so that it doesn't happen that you create a post and then it's denied

* __defistaker__ : I think CC members discussed this internally and tend to make it a bounty, If I recall correctly,  __anynomous__ mentioned this.


* __anynomous__ : Great, then we are exactly on time

    This was the last topic to discuss today, so I thank you all for your wittiness and opinions.
    Till next meeting, unless someone wants to add something.

* __cekickafa__ : @paouky isnt joining meetings. Anybody has idea? or you contact them internally?
There is something about those counsels,when you are in it . You become GHOST

* __phyro__ : Are there any issues with the activity of some members in CC?

* __anynomous__ : So far non. Pauky is not been at some meetings, I can ask if there is a specific reason. With Mac, he lives in new zeeland, therefore we have the next meeting earlier, so he can join.

<br/>

**Meeting adjourned.**