 # Council Meeting Notes February 01, 2022

 Community Council (CC) meeting held @ 15 UTC in grincoin#general channel on Keybase. Meeting lasted 60 min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

<br/>

### _Community attendance:_

* __dtavarez__
* __yeastplume__
* __phyro__
* __cekickafa__
* __vegycslol__ 
* __defistaker__
* __jankie1800__ 

</br>

# Agenda Points & Decisions

* __Decision__: Request for funding @dtavarez Feb-Apr 2022 **PENDING** 
* Last meeting notes [here](https://github.com/grincc/agenda/blob/main/notes/18-01-2022-council-meeting-notes.md)
* Current meeting [agenda](https://github.com/grincc/agenda/issues/36)


</br>

## 1) Update on community miners purchase order and mining operation cost and profit.

__defistaker__ : Well, both of today's topic need input from CC members :)

__phyro__ : should we start going through the agenda anyway or is this skipped because no one from CC is around?

__jankie1800__ : I can raise the questions and perhaps they can respond a bit later and I can add an edit if there are any decisions made

__defistaker__ : Sure, go ahead please

__jankie1800__ : I think the plan was to point miners to a donation pool. I'm thinking to further transparency; maybe an income_log with where miners can account for energy use and be compensated for the cost of running the machine- Also I'm wondering how/if the delivery was processed to everyone housing the machines/ are situated accordingly. Really just checking in for an update.

__dtavarez__ : ASIC miners are in one place right now; we are ready to deliver them starting this month. We tried to find a co-location place for at least the G1 but it has been an almost impossible task.

__jankie1800__ : thanks @__dtavarez__; I think we can revisit and work out how to build transparency as in process- I have access to low cost electricity + a mining friendly jurisdiction. Something I may consider moving forward if there continues to be an issue

__dtavarez__ : We will have more news on this in the near future, in the meantime, we can proceed with the delivery of ASIC miners that were intended for distribution. Any other question before moving into the next topic?

</br>

## 2) Request for funding @dtavarez Feb-Apr 2022 
- [Request Forum-Post](https://forum.grin.mw/t/request-for-funding-davidtavarez-feb-apr-2022/9518)


__defistaker__ : I think we can't officially hold a voting but can talk about the request. I think all the proposed items are needed including bug fixes. Any comments?

__jankie1800__ : Like @__defistaker__ said I don't think we will reach a quorum regarding the vote, but this may serve as a placeholder for the decision and I will update as the council reaches their decision
 * __defistaker__ : Officially, only CC member's vote is counted, is it correct @__dtavarez__ ?
 * __dtavarez__ : it looks like, yes

__dtavarez__ : A small summary- @__mcmmike__ me and __@Mokhtar__ are running Grin++ public nodes; they helped to find things that need to be fixed asap- what I will do now is to focus mostly on the node code for the next months

__cekickafa__ : Payment proof and one time slatepack adress? Does 2 include soft hard fork? sorry for not knowing- I think these 2 things are very important
* __dtavarez__ : no, only new endpoints should be added to the grin++ api- new" for grin++ 
 
__defistaker__ : According to grinnode.live stats, an important portion of running nodes are grin++ 

<p align="center">
  <img width="460" height="300" src="https://u.teknik.io/OJzsx.png">
</p>

* __dtavarez__ : the issues started since v1.2.6 after a rewriting almost code related to P2P; I now need to fix things that I am now aware of since I am receiving feedback from Community members
  *  :+1: (__defistaker__) 
 
__jankie1800__ : do you have any thoughts on the coming PIBD update and if it will affect your work?
* __dtavarez__ : I'll work on PIBD after the things I added to my forum post
    
__phyro__ : Is there going to be any work on payment proofs? I may have missed something on the forum, I did notice one-time addresses but maybe I missed these.
* __dtavarez__ : only to add the same behavior like the Rust implementation
* __phyro__ : oh I see :+1: 
    
__dtavarez__ : the thing is that I am receiving too many support request lately specially from gate.io users, I need to simplify my life and save some hours on support; also the same with tor
too many: "I sent X amount to Gate.io, they are requesting proof" and the typical: "my address is orange", which is solved 99% of the time by using tor bridges. And address reuse is something we should not encourage but, since I am now receiving also feedback from people running public grin++ nodes, now my backlog increased and some issues should be addressed asap from the grin++ perspective
* __defistaker__ : Security issues take priority :+1: 
* __cekickafa__ : too many: ***"I sent X amount to Gate.io, they are requesting proof"*** this torture is since 2019!

__vegycslol__ : Is address reuse bad if u only reuse with the same user? I feel like it shouldn't be. I personally think address reuse is great when you're transacting with the same person. We should not follow btc's each tx new address since addresses on btc and on grin are completely different
* __phyro__ : there are two different concepts really which we (mostly) bulk into one. Grin address is both the destination and the identity. An identity is like a phone number, the destination is the physical location at which you meet. You may want to hide the latter but keep the former intact to be able to call people any time you want. But that's probably a topic that's larger than this meeting
* __dtavarez__ : but you don't want people using grinchck.uber.space to check confirm whether or not your wallet is running in terms of privacy
     
__dtavarez__ : Special thanks to __@Mokhtar__ and __@Mike__, again they are actively testing and running public nodes; I am also running some grin++ public nodes, I think it would be nice if more people deploy more public nodes

__dtavarez__ : I wrote a python script to download and extract the node binary from the GrinPlusPlus repo; now it is easier to do it; but the node should work smoothly, so it is my priority to solve the problems encountered

__jankie1800__ : I appreciate your attention to detail for the end user experience. Instead of counting out those who are blocked or being frustrated by poor exchange experiences it seems like you are being creative and solving their problems through the wallet. I'm excited to see where you take things
* __dtavarez__ : I'm just saving time on support 😂 some (a lot of) people DM me directly instead of using the telegram group, I hate it, but from time to time, I discover new things to help users achieve what they need while using grin++
* __defistaker__ : Thanks for all the hardwork
  * 👆 (__phyro__, __vegysclol__) 👍 (__cekickafa__, __dtavarez__)  
        
__cekickafa__ : yes after Burkett, DTavarez official customer support is perfect. it is not easy to deal people just like me 😂  Burkett was dealing the same i mean. guy was so patient
* __dtavarez__ : Talking directly to users helps Grin++ to be better
    
__dtavarez__ : All topics were discussed, right?
* __defistaker__ : Yes, we have discussed both topics 
* __cekickafa__ : well discussed.if you say so. I took my answers.thnx
    
__dtavarez__ : If the CC woud like to proceed with the decision and update on the forum post __@jankie1800__ can add it to the meeting notes here to account on record. Can we finalize today's CC meeting then? @__defistaker__ 
* 👍 (__jankie1800__)
__defistaker__ : Yes, I think we can close. Thanks all 

</br>

## *Action Points*
</br>

* Update meeting notes with CC decision on funding request for @__dtavarez__



