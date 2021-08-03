# Council Meeting Notes August 03, 2021

4th Community Council (CC) meeting held @ 10AM UTC in grincoin#general channel on Keybase. Meeting lasted 95  min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendence:_ 

* __mcmmike__
* __anynomous__
* __future3000__
* __mark_hollis__
* __dtavarez__
* __cekickafa__
* __defistaker__
* __hendi__
* __phyro__
* __paouky__
* __tromp__ 

 
<br/><br/>
# Agenda Points & Actions
<br/>

* __mcmmike__ : Before we start I would take the time to thank @* __defistaker__ and @jankie1800 or taking meeting notes and for the last meeeting notes which can be found here https://github.com/grincc/agenda/tree/main/notes 👍

## 1)  Funds transfer from core to cc
<br/>

* __mcmmike__ :  We have received a test transaction from OC to the CC BTC multi-sig address
and we did send a test amount back to the OC using all CC members to sign this transaction. 
CC BTC address can be found here : https://github.com/grincc/finance/blob/main/addresses.md

* __mcmmike__ : __@joltz__ we are still working on an automated process for the verification of the CC keyholders to proof it publicly. 
Is there anything else we need to do to receive the funds ?
I think from a CC point of view , except the proof of the keyholders, we have done what we where asked?
anyone else wants to add something?

* __phyro__ : I'm glad this is finally moving. I hope __@joltz__ corrects me if I'm wrong, but after the proof of keyholders, I think you will check all the required boxes 👍

* __anynomous__ : We have some idea about how we can proof active keys for the keyholders, but if the OC has already a sheme set-up for this, it would be nice to have a look at it.

    Unfortunately signing a transaction with all keys does not work as security proof since the additional keys are thrown out of the transaction, so in our case of a 4/6 wallet, only 4 signatures end up on the chain.

* __phyro__ : I see. I'll poke people regarding this question if they don't answer later on

* __paouky__ : The council do it with PGP. 
I'm not sure of the exact scheme tho

* __mcmmike__ : We wanted to proof it on the BTC blockchain showin the witnesses in the transaction, but this is a bit tricky but not impossible I guess.

* __anynomous__ : Ok, not sure how exactly.
We were also thinking about signing a message with latest block hash and making a verification script to check the six messages signatures against the public keys in the GCC transaction. In this way we have proof the keys for signing are different, used for the GCC address and proof of time of signing due to the block hash.

* __mcmmike__ : I think at the next CC meeting we should have a solution. 
And if not we can always do PGP (GPG) at any point in time.

* __anynomous__ : Anyhow, would be nice to check out the PGP method of the OC.

<br/> 

## 2)  Community Pool

<br/>

* __mcmmike__ : Not sure who added this point to the agenda, but I think you refereing to the Grinmint pool after October 2021?

* __defistaker__ : yes

* __anynomous__ : I did notice a spike in hash/graph rate 😉

* __mcmmike__ : As you perhaps noticed I negotiated a agreement with Grinmint and BlockCypher to cover the costs until October and then we move the pool to a new code base but keep the name. 
As the name Grinmint is well known and we can use is after October 2021.
Working with a CC member on a new GRIN mining pool code base and running it legally out of Europe provides us with a good start of the community pool.
We will dedicate a percentage of the earnings towards GRIN project or GRIN council(s).
Also nHash added Grinmint to their default configuration in G1 mini and G1 (2nd mining slot).

* __anynomous__ : This will make a huge difference.

* __mcmmike__ : well, yes and no only if the Chinese pool is down :)
but its a good start and trust relationship

* __phyro__ : that's a good move!

* __anynomous__ : It makes a big difference if miners can quickly switch to it, we are all beasts of convenience.

* __mcmmike__ : if you solo-mining think about joining.



<br/> 

## 3)  Advancement of the CoinSwap Proposal 
(https://forum.grin.mw/t/mimblewimble-coinswap-proposal/8322 )

<br/>

* __mcmmike__ : I personally want to have GRIN coinswap and see it happen but we need to agree on how and who.

* __dtavarez__ : îs __@scilio__ around?

* __future3000__ : Ironically, after I added this to the agenda there was a funding proposal on the forum  : https://forum.grin.mw/t/request-for-funding-scilio-coinswap-implementation/9149

    -I'm not sure how we proceed with funding this...i.e before anyone works on an implementation does the high level design need to be scrutinized more ?

    -How does everyone feel about the request amount/ and milestone payments? 

    -__@scilio__  is there anything you can show us at all in terms of previous work you have done? Even if it's in private.

* __anynomous__ : I think we might need to first have a cryptographer have a look at it.
Regarding the milestones, since we do not know __@scilio__ , I am a bit in favour of having a single bounty, so payment only upon delivery of a working product.

* __defistaker__ : I agree

* __future3000__ : would be good to hear @tromp's thoughts on this.

* __phyro__ : If the solution is open source and they code a milestone from which someone else can pickup and continue, I think that's still some progress towards the goal of having this thing working. But I also see the other side, it might be staying at milestone 1 for a long time.

* __mcmmike__ : Generally speaking,  I am in favor of supporting such requests (CoinSwap) from the CC council not only from the OC. We could even share the responsibilites in terms of verifying the output of the milestones, etc - once we agree to proceed with a request.

* __anynomous__ : In general I am also in favor of supporting the request, it has been requested for a long time, so lets not look a gift horse in the mouth... but at the same time, I am afraid the project might risks being stuck at milestone 1 or 2 in which case it would not be a good deal for the money.

* __cekickafa__ : it is better starting than doing nothing about it. proceed.

* __anynomous__ : If a reputation of good deliveries can be shown, I think having the milestones is fine, since we can trust there is a good chance the final product will be reached.

* __dtavarez__ : I will say this:
    - Open sourced the project since day 0, maybe we could create a repository on grincc github account.
    - Milestone 1 includes the definition and documentation of all public APIs, I would like to suggest to do only that in a Milestone 0, including a architecture design before starting. Why? to have a better idea of how a deliverable will looks like.
    - I found the the proposal too much for a single developer, I'm wondering if I'm the only one with that concern. I found 6 months too optimistic.

* __mcmmike__ : thank you @__dtavarez__ for your oppinion on this. 

    I am a bit concearned, as we need someone to verify the code output of a milestone and when accepting the proposal we need to appoint one or two persons who would verify it for us to proceed with another milestone.

* __phyro__ : whatever happens, the code produced will be verified by the community so that whatever we pay for, we believe it is worth having around

* __anynomous__ : Lets also offer @scilio the option to show proof of competence/trust privately, maybe he does have products or reputation but would like to keep his anonymity, which I respect. In such a case, a few of us could vet for him/her.

* __future3000__ : Personally I want to make CoinSwap a priority, hence why I added it to the agenda. It seems like too good of an idea not be worked on and was concerned OC were not going to progress it, thus CC could push it along.  Do we need to first get more eyes on it and create a public bounty to try and break the design?  

* __anynomous__ : I agree with this option, regarding milestone 0, first check out more what needs to be done.

* __phyro__ : I could point some things that are annoying and fragile in the design, but these could also be detected in the future and are not needed in the first implementation

    it wouldn't hurt to get an opinion from a cryptographer, but I'm not sure paying them to do it is the solution. The thing has a fairly simple design

* __defistaker__ : +1 to milestone 0. And if 6 months is optimistic, it carries more weight to show previous work/experience on similar projects.

* __mcmmike__ : I would suggest on how to proceed:

    1) We proceed as __@dtavarez__  mentioned .
    2) __@anynomous__  is the CC contact person for Scilio 
    3) __@dtavarez__  helps stucture the milestones on our CC github organizations. 
    4) For API usage I can be a contact person as I am providing public API via Grinnode.live ?

    (cekickafa, anynomous, defistaker :thumbup: )

* __dtavarez__ : A CoinSwap Implementation is a ton of work, and I think we all agree on bringing this to life; I would like to see a more detailed planning; perhaps, it is better for @scilio to adopt a scheme like Burkett is doing with MWEB, I found that scheme a better fit when it is hard to estimate due to the big amount of work. I have no authority to say how much anyone's time costs, I'm just trying to find a more fair way to bring @scilio aboard.

* __phyro__ : I would suggest we continue the conversation about the milestones on the forum post to avoid having information in two places (makes it easier to search for people that join the community later)

* __dtavarez__ : I will post my comments on the forum post.

* __mcmmike__ : Ok, then we move to the Forum for further discussion. 
But please take some responsibility if you really think its a good start otherwise it ends in something which we didnt want. 

* __tromp__ : the coinswap is simple enough that we can forego an official audit. a bounty on breaking it would be fine, but i'm pretty confident it's sound

* __future3000__ : ...Just quickly. Before we move on.  Let's move to the forum for further discussion as suggested, then providing CC has funds transferred by our next meeting, we could then vote on funding the first milestone.
( __mcmmike__, __anynomous__ :thumbup:)

<br/> 

## 4)  Manual confirmation of an incoming transaction RFC 
<br/>

* __mcmmike__ : Can you David take over here please?

* __dtavarez__ : :thinking_face:

* __mcmmike__ : If we dont have a clear idea we can pospone this agenda point?

* __defistaker__ : I repeated issue title in the github issue, apologies

* __anynomous__ : Yes, can also postpone. In general I think the idea is to add manual confirmation (and all options/benefits that come with it) as an opt-in feaure in Grin++ and grin-wallet. not sure what needs to be discussed though.
For now, who is interested can share his or her view on github:
https://github.com/mimblewimble/grin-rfcs/pull/84

    Or the forum as part of the ultimate grin wallet experience discussoin:
 https://forum.grin.mw/t/lets-create-the-ultimate-grin-wallet-experience-grin-ux-ui/9092/25

    Lets move on?

* __dtavarez__ : I don't know what we need to discus about this here. 

* __mcmmike__ : yes I think its best to pospone it (  __@defistaker__ take not of this please)

<br/><br/>

## 5) Community minining equipment purchase
<br/>

* __mcmmike__ :   __@anynomous__ can you take over here please?
just a short side note, I got contacted by nHash, the G1 miners a nearly sold out but they have plenty of G1 minis (iChicken's)

* __anynomous__ : Ok, We have discussed the purchase of G1 and G1 min miners in the last three Grin Community Council meetings.
As a result of these discussion we proposed two options and we let community members vote on these options via the forum:

    With around 10 days of voting and the following count

    Vote results:
    12 G1 Mini’s (1 Vote)
    12 G1 Mini’s + 1 G1 miner (9 votes)

    The community council will proceed with option 1), the ordering of 12 G1 Mini’s and 1 G1 miner, we will contact NHash to reserve the order.

    As a side not, NHash notified us that their supply of G1 miners is running low, so we will take some haste in contacting them and reserving our miners.

    There are still however some things to consider and take care of, e.g. how to arrange accountability, compensation for electricity usage, and especially how to get the lowest electricity price for the G1 miner since most CC members live in Europe where electricity prices are around three times as high compared to for example the US.

* __future3000__ : I support this, however, before we proceed we need a more concrete plan:
As you've allured to: 
    1) Who exactly from CC is going to hold the G1 & G1 minis. 
    2) What is their $/kWh
    3) Who will control the wallet/ or wallets 

    I also think we need a formal vote in a CC meeting, once we have funds from OC. 

* __mcmmike__ : on a side note, for Grinmint we are providing some base-hashrate using a G1 and some G1-minis in a datacenter as you perhaps have seen in the hash-rates. But I dont know if the electricity cost are this beneficial here for the CC miners. 
 
* __mcmmike__ : `1) Who will control the wallet/ or wallets`
 
    I would suggest setting up a account on Grinmint and share the password with a few CC members and withdraws only to our public donation GRIN address. 

* __dtavarez__ : `1) Who will control the wallet/ or wallets`  I think withdrawals can go to the CC wallet.
(* __mcmmike__, * __anynomous__ :thumbup:)

* __mcmmike__ : `2) What is their $/kWh `
We are payin 0,30€/kwh at the moment in the datacenter

* __anynomous__ :
    1) I think we discussed this internally a bit, most of us can host 1-2 G1 mini miners or more, so the G1 Minis are not much of an issue 
        although the electricity price might be high.    
    2) We have to index our electricity prices, I think mine is around 0.27 euro/kWH, so 2.5-3 times the price as in the US.
    3) What David said, we can use the CC grin wallet.

* __mcmmike__ : and btw, you can NOT run a G1 in your home ! 
Its like 100 GPUs at full 100% fan speed, literally. 

* __anynomous__ : Since the G1 is the biggest hash rate, I think this is the one we have to focus on, find good housing with cheap electricity, the G1 mini miners are ok with somewhat higher electricity price, it is still small compared to what they generate.

* __cekickafa__ : 0.08 here +/kwh

* __future3000__ : Yes we have discussed internally. But not exact details.  I feel the community needs to see a concrete plan for accountability sake. 

* __dtavarez__ : I agree, just a note: it is good to say that internal conversations are just random conversations, no decision is made; decisions will be taken publicly during these meetings 

    (quoting  __future3000__) maybe the next step then should be to write a concrete plan (?) present this plan and ask for public feedback

* __mcmmike__ : as suggested lets use the forum

* __dtavarez__ : cool

* __mcmmike__ : but I am not sure if nHash can reserve miners for us to be honest.

* __anynomous__ : We can use the forum discussion on voting for the miner options, already some good discussions are going on there.

* __mcmmike__ : **To summarize:**
    - Once we receive the funds we  do a formal vote here.
    - We document the process on GRIN forum publicly as well as in the CC meetings and ask the community for feedback. 
    - we should give out 3-5 G1-minis to the community anyhow even if a CC member hosts all miners for this purposes. 

    (__dtavarez__ :thumbup:)

* __anynomous__ :  __@mcmmike__ That is why I think we need to formalise the decisions, so they now we will pay soon.
We can also vote in allocating money for it, the vote does not depend on us having the Bitcoin in the wallet. I do wonder about a batch discount though...

* __mcmmike__ : but if we have not formally voted yet, we should not reserve it (if even possible)

* __dtavarez__ :  __@anynomous__, do you think we could have a meeting next Tuesday then?
one week to write the formal plan, and receive feedback

* __mcmmike__ : sure same time is fine with me.

* __dtavarez__ : the meeting will be just for having the formal decision 

* __anynomous__ : Yes, I think that might be best. We nee to keep things moving, since the G1 is a major factor in the mining, we cannot manage  64 G1 Mini's

* __mcmmike__ : __@dtavarez__  __@defistaker__ should we create an CC agenda issue for this? I would say yes to have everything public and reference to it on the forum post.

* __dtavarez__ : I say yes

* __mcmmike__ : next Tuesday at 12 CEST if  __@future3000__ also wants to join.

    before we conclude any other topics we should be discussing here? 

* __anynomous__ : __@mcmmike__ can you ask Nhash for a price/ with batch discount, so we also have the price set before the official vote.

* __mcmmike__ : sure , send me the amount of miners and I do it directly after the meeting

* __anynomous__ : 12 G1 Mini +  1 G1, with preaty please batch discount and possibly extra discount for supporting the Grin Community.

* __mcmmike__ : done: 
    ```
    Hello Helen,
    we had a community council meeting today and wanted to ask about a price for:
    12 G1 Mini +  1 G1 miners
    For the GRIN community can you please make us a fair community price on it ?

    We will make the order process public and I will send you a link soon. 
    This is for supporting the Grin Community. 

    Thank you from the GRIN community,
    Michael
    ```

    __@defistaker__ please create a new issue on the CC https://github.com/grincc/agenda for the next CC meeting in two weeks. 
    Please make sure the time is set correctly for the next meeting.

    If you dont mind, include the GRIN discord invite link https://discord.gg/5p4vCQY9km  to the issue. And perhaps a link to the GRIN Keybase server.
 
    This was a productive GRIN CC meeting, thank you all and I wish you all a lovely day .

* __defistaker__ :
    - https://github.com/grincc/agenda/issues/8  (Mining equipment meeting) 
    - https://github.com/grincc/agenda/issues/9  (Next regular CC meeting)
                
<br/>

**Meeting adjourned.**