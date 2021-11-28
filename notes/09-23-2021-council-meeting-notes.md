 # Council Meeting Notes November 23, 2021

 Community Council (CC) meeting held @ 10 UTC in grincoin#general channel on Keybase. Meeting lasted 80 min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

<br/>

### _Community attendance:_

* __anynomous__
* __phyro__
* __yeastplume__
* __ordante__
* __cekickafa__
* __defistaker__
* __renzokuken__
* __hendi__
* __mcmmike__
* __dtavarez__
* __jankie1800__ 

<br/>

# Short Summary

- Miners transaction logs now available for review.
- Grin-Exchange progress is ongoing with updates pending.
- Discussion of proposal for GRN-BTC currency conversion was approved.
- Discussion of extending grin-wallet cmd line tool to parse recovery seed will continue on github. 
- Review of @Scilio's Coinswap Milestone #1 looks excellent and is approved. Milestone #2 will be up for next.

<br/>


# Voting Results
* Vote to allocate 0.5 BTC and flexibly buy grin when and if needed so we can fulfill our promise of paying Funding Requests at least 10% payment in Grin **VOTE PASSED (YES)**

* Vote accept the work of Scilio Coinswap Milestone #1 to release compensation and commence work on Milestone #2 **VOTE PASSED (YES)**

* Decision to fund hosting for slatepacks.com in amount is **accepted** 50ツ from GrinCC with the rest (50ツ) funded by personal Individual Contributors(IC's)

<br/>


# Agenda Points & Actions

* Last meeting notes [here](https://github.com/grincc/agenda/blob/main/notes/09-11-2021-council-meeting-notes.md)
* Current meeting [agenda](https://github.com/grincc/agenda/issues/25)



* __anynomous__ : Welcome everyone to today's Grin CC meeting.
Find the agenda [here](https://github.com/grincc/agenda/issues/25)
Lets take a few minutes to read it.


* __dtavarez__ : I want to start sharing the Transaction made for the miners: https://etherscan.io/tx/0xafebbcf478720ee950f6daf1c839be882b13da464ea187992afd540bc7a28a0f

* __defistaker__ : Before we begin,I  would like to inform community about grincc website. I have some health issues in the last few weeks, which prevented me from staring computer screen for long times. I am recovering now, and planning to finish website as soon as possible
 * __anynomous__ : Looking forward to see how the site will look like __@defistaker__

## 1) Bounty idea for adding Grin to THORchain

* __anynomous__ : It was suggested by Gorfish, but I think he has a different handle here on KeyBase. It would be best if he made a case for it however; THORchain describes itself as:https://www.thorchain.com/ A Cross-Chain Liquidity Network swap between blockchains directly from your wallet. The idea sounds nice, but there are multiple projects I think that offer similar functionalities, so not sure if and why THORchain. Does anyone has experience with the project? If not, I would suggest we or Gorfish first create a topic for it on the forum to discuss it in more detail. After discussing it on the forum and knowing more details, we can bring it up again in a Grin CC meeting to create a proper Funding Request or bounty.

</br>


## 2) Generation of transaction logs for public visibility 

* __dtavarez__ : this is about the transaction log of the miners, right?

* __anynomous__ : I think so, but I did not add the topic.

* __dtavarez__ : this is referred to here at the beginning of the meeting: 'Transaction made for the miners: https://etherscan.io/tx/0xafebbcf478720ee950f6daf1c839be882b13da464ea187992afd540bc7a28a0f' 

* __hendi__ : So far we've received about 3,034 Grin on the CC wallet. :rocket:

* __anynomous__ : In general I think we soon have to produce another security proof and have to update our transaction logs. So time for some administrative work.

* __phyro__ : I suggest github issues for wallet/node related changes because it's much easier to track things there. Perhaps there's already one for this

* __anynomous__ : __@phyro__ that sounds like a good plan. @ __@dtavarez__ Can you maybe make a page on github showing the transaction logs of the Grin CC Bitcoin wallet. __@hendi__ can you maybe add to it an overview of our donations to the Grin CC Grin wallet.
I will focus on generating a new security proof, for that we do need a transaction we all need to sign, maybe the payment to Scilio which we will discuss later in this meeting.

* __dtavarez__ : details of each transaction can be found in the grincc repo added my Mike. each task was tackle using cards. details are in each task

* __hendi__ : Unfortunately my node was off for a while / a secondary node handled the receive of the donations, so now my main node doesn't give correct receival dates on grin txs unfortunately

* __anynomous__ : No problem, we will sort that out. I can maybe help.

* __hendi__ : Ok, thanks. Let's add to the agenda that I'll give a bi-weekly update about the donations (if any), and update a public/permanent list on Github

</br>

## 3) Updates on Grin-Exchange progress

* __mcmmike__ : We are making progress with the mining pools, but I sadly can not report a due date when GRIN will be listed. Make sure you write each exchange, that you want GRIN listed, so we can generate a bit of a demand from the community side. I have to highlight, we did not hear back from KuCoin since a long time. BisQ is pro-active an will implement GRIN soon. Its a slow process but we making progress step-by-step. Also please be aware the upbit post could be fraud as we still in process of double-checking. 

* __anynomous__ : Yes, the security deposit for 1 month does not make sense. I think Defistaker contacted UpBit to verify if the post is legit, any response yet?

* __defistaker__ : upbit seems to be a scam after research 

* __anynomous__ : __@defistaker__ Great work, lets mark it as a scam on the forum.

* __dtavarez__ : Hotbit- one of the devs was having problems with TOR, there is no update if he managed to solve it </br> Gate.io- we shared with them enough documentation about grin transactions and the GRIN Integration Guide written by Marek. Also the suggestions of decreasing the confirmation number and also how annoying is the memo hack.

* __jankie1800__ : Bisq dao vote will release Dec 1
    * __anynomous__ :crossed_fingers:

* __mcmmike__ : I can comment on one important fact while we in contact with the exchanges.
We lack the problem of showing the exchanges how our wallets can handle hundreds of deposits and withdraws for the users. 
At the same time the wallet needs to be multi-tenent, which we also need to show them.
we came up with a short process:
https://github.com/grinventions/docs/blob/main/slatepack-integration-guide.md - We need some more help here from experienced users.

* __anynomous__ : I think the first step is to use the HD part of the wallet, e.g. account level, even without tor, it naturally separates customers.

* __yeastplume__ : right, we did have ideas about a more robust backend for the wallet, a refactor of some db code and sql db support but never had the priority. I agree this needs more focus.

* __anynomous__ : Sheldonth is working on allowing multiple wallets, which could also help.

* __cekickafa__ : So I want to ask something. Is it good strategy to rely on exchanges instead of a Ordante style metamsk wallet for real use cases? Does it needs a HF consensus breaking with payment proof or something?
 * __mcmmike__ : we also need to integrate the RFC from tromp, but this is not for this meeting I guess. More for github discussion this would help also with the process.

</br>

## 4) Proposal for GrinCC to buy around 0.5BTC-1.0BTC worth in Grin
see [proposal](https://forum.grin.mw/t/proposal-grin-cc-buy-around-0-5-1-btc-worth-of-grin/9371/8) on forum.grin.mw for more details
</br>

* __anynomous__ : We discussed it a bit on the forum, to be hones I expected more input there. The general idea is to buy allocate some BTC flexibility to buy Grin when needed to keep the Grin finances of the CC sufficient to pay Funding Requests at least 10% in Grin.
In a few months the miners will generate enough, but till then we need some funding to cover it. I think __@newjack__ gave a nice summary of which possible directions to go. 
> **A**)fulfill the proposal asap - begin 10% grin payouts on contributions (aka the keep it simple approach)</br>
**B**)hold off on fulfill proposal until miners are situated - pushes payment in ツ for contributions back.</br>
**C**)Hybrid-B: hold off on proposal until miners are situated + use this as inspiration to commit to running some sort of charity fundraiser. Doing this would serve as community building and keep strong the shaking cup side hand. Already this post has garnered financial support from inside the community so it may well serve as a case-study of reaching to outside established channels for support. After all we are a project that runs on donations. Though I can easily see us reach out for support only to receive more btc donations.</br>
**D**) Do nothing. imo not really an option as to prior agreement to pay out 10% to contributors- however the timeline may be negotiable depending on urgency"

* __anynomous__ : Just to emphasize, the purpose is not to buy on the spot in one time 0.5-1 BTC worth of Grin, but to have the funds available when opportunity and need coincide.

* __dtavarez__ : And that's why we will be running miners right?
 * __anynomous__ : Exactly, so on the long run we will not be dependent on exchanging BTC-Grin, which might be ill timed and provides additional work. It might even be, that the need and opportunity do not arrive, if the miners produce enough in time... What are your opinions on it?

* __dtavarez__ : my personal opinion is that, yes, we want to have enough coins, but I don't see the pressure to have them asap

* __anynomous__ : My opinion is similar, I think yes we should allocate the funds, but no need to rush into anything, it just means we can if it is needed.

* __defistaker__ : I am for the keep it simple approach. (A)

* __phyro__ : Grin funds are probably a bit riskier today because there's no multisig I assume.
 * __anynomous__ : I  agree, I would very much like it if there would be a solution to this. MultiSig, double password, something.

* __future3000__ : I'd rather we hold off for as long as possible doing any further conversions from BTC to Grin and only do it if necessary.

* __anynomous__ : Ok, to summarize what I hear:
> 1) There is an agreement that the funds can be allocated 

>2) It should be stressed that the funds should only be used if and when needed.
Do we agree on the amount 0.5-1 BTC? How much in that range? I personally think that 0.5 BTC would already be enough to cover the gap till the miners kick in. :+1:(hendi, future, anynomous)
</br></br>

* __anynomous__ I think __@mcmmike__ would prefer to have more available, what do the council members say?
>1) 1 BTC allocated
>2) 0.5 BTC allocated

* __hendi__ : the less the better IMHO

* __mcmmike__ : 0.5 BTC is enough. Also we are not quick in exchanging BTC for Grin as counci, so we should have at least a bit to distribute

* __anynomous__ : Ok, then we formally agree on allocating 0.5 BTC to flexibly buy grin when and if needed so we can fulfill our promise of  paying Funding Requests at least 10% payment in Grin.

</br> 

## 5) Funding slatepacks.com hosting costs.

* __dtavarez__ : I personally donated for hosting costs

* __anynomous__ : I also see this one as something that is more fitted for donation purposes, we could however also decide to "donate" some funds as Community using the CC funds if all here agree to do so, e.g. 50% of the hosting costs, the rest can come from community member donations.
 * __mcmmike__ : I am fine with it, but we need to think about future projects how to support them. Because I see a bit of a risk if we don't have a future support plan for community projects.

* __future3000__ : How much are the hosting costs? 

* __anynomous__ : I am not sure exactly why he failed to get enough donations, I did not see it mentioned at the forum, but he says: 
> "I have been unsuccessful in asking the community for the remaining 100ツ needed to run slatepacks.com for another 5 months -- Can I please bring this up to the CC and ask for your official input regarding funding the GRIN marketplace I made?"
</br>

* __dtavarez__ : "100ツ needed to run slatepacks.com for another 5 months"
    * __mcmmike__ : donation address? 
    * __dtavarez__ : grin1cq636ment795xn68knzu0ewp73f3zdlgv6dsqv8x7vf2v0j4ek5sk6nmk3

* __mcmmike__ : sent 100ツ from the grinnode.live donation wallet

* __future3000__ : I like the idea of us running CC funding campaigns to support things like this
    * __dtavarez__ : me too 

* __anynomous__ : Ok, so for now we can agree to make a donation of say 50ツ and anyone here can decide to donate or not. I think we should help facilitate indeed. </br>
thumbs up for donating 50ツ of community funds
    * :+1:(anynomous, ordante, dtavarez, future3000, jankie1800, hendi, cekickafa, hendi)
</br>

* __anynomous__ : Then we are agreed to:
> 1) Help this time with a donation of 50 ツ

> 2) To in the future help out facilitate fund raisers in general for similar purposes

* __anynomous__ :Just a thought, maybe even dedicate a page on the Grin CC website for it __@defistaker__
    * :+1: (defistaker)

</br>

## 6) Discussion of extending grin-wallet cmd line tool so that it can parse recovery seed from a file - w/ Security Perspectives 
see [proposal](https://forum.grin.mw/t/proposal-grin-cc-buy-around-0-5-1-btc-worth-of-grin/9371/8) on forum.grin.mw for more details
</br>

* __ordante__ : I'm hoping that a rust developer will cherry pick this

* __anynomous__ : I do think we really should facilitate more this kind of tinkering. It is the best way to create a healthy ecosystem. So yes, I hope indeed a Rust developer will pick this up. And for the future we need to look at standardizing API's between wallets, making it as easy as possible to build around them.
    * __cekickafa__ : standardizing api since 2019
    * __dtavarez__ : It is important yes, that's in my horizon. One step at a time 

* __anynomous__ : Are the API's of Grin++ and grin-wallet the same right now? I have not played with either in a long time.
 * __dtavarez__ : Not exactly the same. There are some differences

* __yeastplume__ : I don't think grin++ exposes API's for 3rd parties. (could be wrong..)

* __anynomous__ : I think there is not more we can discuss here than emphasize that this is something we all think is important for the future of Grin since it makes life so much easier for anyone who develops code on top of the node(s) or wallet(s). I hope to see a future with a myriad of programming languages used for different nodes, that can interchangeably use different GUI's and all link to ecosystem.

* __ordante__ : It's not just the recovery phrase, its also slate packs. There was one argument that if you pass the phrase via command line it will be logged in bash history but i think if you have bash history turned on that's what you want. The alternative is to | pipe in the data or pass as a file.
    * __dtavarez__ : would you mind to open a github issue for this?

    * __ordante__ : I will open 2 github issues now, I hope that somebody takes them and they don't sit in queue forever. They are really easy fixes. There is also the unpack crash I found.

* __yeastplume__ : We chose specifically not to allow the phrase on the command line, which is why it's parsed in-app only using an input parser.
 * __anynomous__ : It just needs to be an option, for developers, not default for normal users. Maybe make a developer mode in the wallet that you need to enable, a boolean.

* __ordante__ : So this needs discussing if it's a security issue but also if I can't use the Rustlang Grin implementation then what's the point? to expect a hack to require a gui terminal present.
    * __dtavarez__ : but you can use the API.

* __phyro__ : As tavarez suggested, the github issue is the place to discuss this imo 

* __ordante__ : where is the api documentation please. is it v1/v2/v3? Also, where can I recover wallet? https://github.com/mimblewimble/grin-rfcs/blob/master/text/0007-node-api-v2.md
    * __anynomous__ : please do add an issue so that we have a good place to discuss this further.

</br>

## 7) Review of Scilio's coinswap milestone 1 & discuss approval for milestone 2 start
[github PR](https://github.com/mimblewimble/mwixnet/pull/1)
[forum discussion](https://forum.grin.mw/t/request-for-funding-scilio-coinswap-implementation/9149/55)
</br>

* __anynomous__ : is the reviewing of the coinswap already done, or in a far advanced enough state to approve milestone #1? 
    * __yeastplume__ : A few of us reviewed it, we're happy with progress so far and happy to have Scilio contributing

* __dtavarez__ : Joltz has made a comment after review found [here](https://github.com/mimblewimble/mwixnet/pull/1#pullrequestreview-813030113)
> * __joltz__ (from github comment) : "This PR seems to implement the basics as described in the first milestone. Beyond that, I don't have much to add that hasn't already been brought up in these comments.I do have some comments about the specification itself but will keep them in the forum thread. It's nice to have you here Scilio, looking forward to seeing your next work.

* __anynomous__ : So that is a yes? 
    * __phyro__ : Yes, as yeastplume mentioned, we are happy and we merged the milestone #1. Could someone remind me which council was supposed to cover the coinswap?

* __jankie1800__ : I recall Scilio requested funding came through the GrinCC.
 * __anynomous__ : Indeed he did. So the Grin CC has to make the transfer, we can all sign it so we can use it as our second quarter security proof.
 * __phyro__ : Ok, great :grin: 

* __future3000__ : CC picked it up because we wanted some action
 * __yeastplume__ : I don't think it was clear from the funding requests who was to fund it (core fund has no problem funding quality work either, it just needs to be clear from the outset)
 * __anynomous__ :  think we can always later on discuss distributing funds in case the Grin CC runs out, for now that is not an issue.
The funding is not separate based on programming language, there are just different emphasis on what kind of projects to fund from the Grin OC and Grin CC.There most certainly will be overlap, we all work towards the same goals. The requests was made in general, the Grin CC honored/approved it, so I think this one we can fund from the Grin CC funds.

* __yeastplume__ : I think we may have to work this out a bit; we could have a case where the community funds somthing that needs core devs to review/merge, but if it's not up to snuff (according to OC) and we can't merge it we might have contention.In this case scilio's work is of good quality, so we're fine. But that won't always be the case. I just don't want a situation where OC starts being accused of being elitist or playing political games because a piece of work isn't of sufficient quality, or there isn't sufficient consensus to merge it.
 * __anynomous__ : I think we can always cross that bridge when we get there. I think in general as long as we all discuss things with respect for each-other, differences in opinion are never an issue, they are just part of a healthy eco-system with healthy discussions, which might indeed include disagreeing sometimes. Correct me if am wrong, but all these things are just procedural. Both councils have formal meetings, discuss things and vote on them. There might be times that the OC approves something (for funding or committing), that the CC has doubts about and vise versa. But that is not different from the situation with one council. In the end, the community decides (assuming there is proper argumentation).

* __phyro__ : It could still be an issue if the OC wants to invest time elsewhere and doesn't agree we have time to review a certain project. 
 * __anynomous__ : It is true, the CC is very much dependent on good reviewers, for which many are part of the OC. We cannot change that. But in this case I think it is about how to view these community members. I think we should see them all as community members, volunteers, no one is paid for reviewing. So there can be no contention, or blame if someone does not volunteer to work or review anything. For this reason I also do not foresee contention between OC and CC, since we simply ask community members, not members of the council. So lets make clear that we separate the role of OC and CC members which are just formal bodies to make decisions, and any activity that members of these governing bodies do as community member.

* __mcmmike__ : I think what __@yeastplume__ wanted to highlight, if there is something the OC is not agreeing on because of bad programming or possible future problems, they can still decline the PR into rust wallet.

* __anynomous__ : Regarding governance and overlap, possible contention between OC and CC, maybe we should simply have chat about that sometimes, preferably over a beer. I do not think the CC will have any wrong expectations or demand from OC members, we are all volunteer after all. Alternatively we could maybe discuss it one time in a joint OC CC meeting, I mean why not have such a meeting.
</br>
* __anynomous__ : Unless there is anything else we should discuss, I would like to wrap up the meeting for today and thank you all for attending. 
Lets press onwards:muscle:, many interesting developments with Grin lately:grin:

__Meeting adjourned__

</br>

## *Action Points*
</br>

* Follow up thank you to those in the community who made monetary donations today in addition to the ongoing contributions of time and energy
* Discuss potential meeting time between OC and CC
* Follow up with hotbit exchange for update and provide additional support
* Review THORchain protocol and revisit at a later date
* Follow up to refresh security proof and update transaction log
* Community donation campaign possible ideas and solutions for future funding models
