# Council Meeting Notes May 24, 2022

Community Council (CC) meeting held @ 15 UTC in grincoin#general channel on Keybase. Meeting lasted 60  min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendence:_

* anynomous
* yeastplume
* cekickafa
* defistaker
* phyro
* dtavarez

<br/>

# Short Summary

-  Mining decentralization and exchanges Grin implementation has been discussed.
-  Make sure current Asic vendors are not scammers
-  Grin Mining documentation and tutorial should be prepared.
-  Adding telegram link to community web site instead of main site has been discussed. 

<br/>

# Agenda Points & Actions

<br/>

* Last meeting notes here: https://github.com/grincc/agenda/tree/main/notes

* Current meeting [agenda](https://github.com/grincc/agenda/issues/56)
  1)  Adding the telegram link (https://t.me/grinprivacy) to the bottom of grin.mw
  2)  Discuss ideas about mining decentralization and how to promote it & how to engage with Chinese miners and users
  3)  Small bounties (Grin Tipping bot for Telegram & Changes to Grin Nodes).

 
## 1) Adding the telegram link to the bottom of grin.mw
<br/>

__anynomous__ : I will save you some typing @dtavarez by copying your input from before here:

Regarding "Add the telegram link (https://t.me/grinprivacy) to the bottom of grin.mw", my opinion is that grin.mw should stay the focus on Grin technology. We already have https://grincc.mw/hub which includes many links. Perhaps what we need is to update this page: https://grin.mw/community and in that case, anyone could just open a Pull Request including the desired changes. My suggestion would be to add a link to grincc.mw and remove the old links that are not working anymore.
I do not have much else to add. I personally think we should add a link to the grincc.mw, possibly another to grincc.hub.mw

     👍 anynomous,phyro,dtavarez,defistaker  

  

__anynomous__ :  So, regarding the initial request. Personally I feel no need to add the telegram link, if anyone does think it needs to be there, speak up now.
I think we all agree on this one. We do not directly link to social media, but we link to the grincc website which links to all kind of media, including telegram.
Next agenda item:

## 2) Discuss ideas about mining decentralization and how to promote it & how to engage with Chinese miners and users.
Again, I start with quoting the all wise @dtavarez :
"
David
- Try to reach out current miners. I think it's worth a try.
- Keep reaching out to the Exchanges.
   - Push Gate.io on the right implementation.
- Make sure current vendors are not scammers.
   - Promote current vendors.
- Write well written and comprehensive documentation on mining. I think the forum might be a good place.
"
Great job at making a tutorial on how to use the G1/G1 Mini and posting it on the forum. I already linked to it on GrinHub @cekickafa

__cekickafa__ : 👍

__phyro__ : what's meant as the right implementation?

__defistaker__ : I guess without memo
Those are Davids words, he is quite fundamentally against memo, and in favor of slatepacks.
I think most of us are, however, memo's are there to stay unless Gate.io decides to change it.
Has anyone in the past contacted gate.io, to ask/try to convince them to adopt slatepacks?
__cekickafa__ : Gate io is the only exchange upgrades constantly with Tradeogre. They find this method to combat with tickets i think. Deposit/Withdrawal problem.
Other ZB,and BKex implemented same MEMO method.
TOR adresses g1..

__phyro__ : I think they may be using memo as user identifier. Does anyone know the exact reason and can confirm?


__cekickafa__ : yes,a sort of KYC.

__anynomous__ : I cannot confirm, but yes, I think they use it to link to users. Probably so they do not need to have to make separate software to manage accounts, simply a single wallet.

__phyro__ : I didn't really have KYC in mind, they just need to know which user sent the money


__cekickafa__ : KYC means identify user.

__anynomous__ : We should ask them for their reasons. I think it them having a single wallet, and a need to link outputs to users

__cekickafa__ : But you dont need memo while withdrawing.

__dtavarez__ : they are doing that to link deposits to users

    👍phyro


__cekickafa__ : Only deposit

__anynomous__ :But, yes, this also can be used as KYC. 


__phyro__ :
> __cekickafa__ : KYC means identify user.

this is KYC https://www.investopedia.com/terms/k/knowyourclient.asp

__dtavarez__ : they kind of refused to change it because grin flow is unique

__cekickafa__ : 
>__phyro__  this is KYC https://www.investopedia.com/terms/k/knowyourclient.asp

MEMO proves that you sent the deposit.

__phyro__ : alright, didn't want to hijack and move in this direction, dtavarez confirmed my question

__anynomous__ : Ok, so it is about them being able to have outputs per user. And yes, also as sort of a payment proof.
Basically it is about dispute settlement.

__cekickafa__ : The point is, gate.io is the only one upgrades Grin wallet regularly and there is no alternative than tradeogre.

__dtavarez__ :  They reject the idea of creating an unique flow just for grin

__anynomous__:  We should ask them how much each of these weigh. E.g. if it is all about dispute settlement, then payment proofs are the solution.

__dtavarez__ : 
> __dtavarez__ :  They reject the idea of creating an unique flow just for grin

  in summary that is the main reason

__anynomous__:  Probably, and they are not alone, meaning it is a problem for many exchanges.

__dtavarez__ :  Kucoin problem was a bug that was reported but not fixed.

__cekickafa__ : Only More exchanges and competition will solve the problem.

__dtavarez__ :  Now the built is fixed, they could just upgrade their nodes.

__anynomous__ : I think we covered the exchange part of Decentralisation.
Next would be to discuss miner decentralisation.
Do we have any active Chinese community members? Not sure if @xiaojay is still active. I would not even know where to contact Chinese miners to convince them that more decentralisation is good for the project, and as such also for the price they might get for their Grin.
EDITED
I will interpret silence as, no one knows any active Chinese community members, or how to best get in contact with them.

              
<br/> 

## 2) Small bounties (Grin Tipping bot for Telegram & Changes to Grin Nodes).

<br/>

__defistaker__ : We are talking about bounties, do we have a procedure to decide for amount etc?

__anynomous__ :Not really, it is open to discuss. @dtavarez made some sugestions:


* A Grin Tipping bot for Telegram for 10,000 ツ

 * nodes.grincc.mw improvements:

      * Making UI responsive for 100 ツ

     * Serve external javascript libraries from localhost for 100 ツ

     *   Implement multithreading to get nodes information for 5,000 ツ

It is hard to estimate if these are the right amount per bounty. David can best estimate them since he know the code. The website is in Javascript and CSS, the node contacting software is written in GO, but the multithreading part can also be done by an overarching script, e.g. bash parallel.

__defistaker__ :I support the suggestion

__anynomous__ : So to me, these bounties look 'about right' as far as I can estimate them. Not to high, but enough to be interesting 


👍 (cekickafa)

Same here. Is anyone against these bounties, or things they are to low or high?


__defistaker__ : Yes, it should be easy for someone with go knowledge to make it responsive and load external js
No idea about, multithreading, I trust @dtavarez on that :)

__anynomous__ : Not sure either, but I think it is also managable.

__dtavarez__ : The process to the nodes information happens in one single thread.

 __cekickafa__ : Lets start,then we can do fine tuning about bounty quantity.

__dtavarez__ :  The idea is to use multithreading to have more uptodate information about the nodes
example https://nodes.grincc.mw/publicnodes?ip=107.174.93.160
grincc.mw
Grin Nodes
the actual height is >1757209
but in the website says 1756968
also it would nice to have a more accurate number for Public Reachable

__defistaker__ : https://github.com/davidtavarez/grinnodes/blob/master/p2p/connect.go

__anynomous__ :  Sounds like a plan. How and where will we make these bounties public?

__defistaker__ : I don't know about go, but it seems it updates every 10 minute for peer. If the update interval reduced,  would not it get more accurate numbers, without multithreading ?

__dtavarez__ :  Not exactly.

__anynomous__ :  I see, it works like a queue, so multithreading should speed it up.

__dtavarez__ :  The idea of the 10 minutes is to avoid banning your ip to get the geo ip information

__anynomous__ : What do you mean avoid banning? If you do too many request to a peer, they auto ban you?

__dtavarez__ :  Not from peers.
From the services required to get the geo info of the IPs

__anynomous__ :  Ok, well, you can also check peers every 1 minute, and GEO location only once every 10 minutes, hour or day.
Anyhow. It sounds like a good plan. Lets put out the bounties, but where?

__dtavarez__ :  Forum?

__anynomous__ : Sure, mabye we should also make a separate bounty page at the grincc github page.
Both

__cekickafa__ : Excuse me but locating ip ,geo doesnt hinders privacy?

__anynomous__ : I have to go now.
Thank you all for the meeting, and hope to see you soon.

👋 cekickafa, defistaker, dtavarez, phyro, yeastplume

Maybe you can still ask @yeastplume if there have been any recent developments.

__defistaker__ : 
> __anynomous__ : Sure, mabye we should also make a seperate bounty page at the grincc github page.
Both

 I think github should be primary place, we can post to forum, and give link to github repo.


 __dtavarez__ : 
 >__cekickafa__ : Excuse me but locating ip ,geo doesnt hinders privacy?

 that is a good discussion
but right now the geo location is only used to display the heatmap
it is possible to unlink the geo information of the ip
there is no need to save it
but again, I think it would be nice to have a bounty for that too.

 👍 (cekickafa)

 __cekickafa__ : ok maybe @yeastplume has word ?

 __defistaker__ : Maybe he is afk


__yeastplume__ :  Not too much, hope everyone has seen the seed checker at https://grintools.revcore.net/seedcheck/

🚀 anynomous, defistaker

 __anynomous__ : Yes, i saw it.

__yeastplume__ : And the forum post asking for more seed nodes (don't have the link just now). That is just the first of a few tools to come.
but at the moment I'm stopping to review and catch up on mwmixnet and the code and I want to get some docs done on PIBD

🎉cekickafa 👍 dtavarez, defistaker, anynomous

if any of those testnet nodes that aren't working are yours... please let me know!

__anynomous__ : I will check

__dtavarez__ :
 >  __yeastplume__ : And the forum post asking for more seed nodes (don't have the link just now). That is just the first of a few tools to come.

 The CC will also offer one seed node for each network
nodes were deployed
we just need to setup the DNS.

🚀 anynomous, defistaker, cekickafa

__yeastplume__ : Yes and we'll have 2 up on behalf of the core team.

__dtavarez__ : Excellent

__anynomous__ : For note keeping, this meeting is now at an end 😉



   ## *Action points*
 - Crosscheck and make sure  Grin ASIC vendors legit. 
 - Grin  Telegram Bounty announcement.
 - Small bounties for nodes.grincc.mw improvements.
 - Forum post about  seed nodes.




**Meeting adjourned.**


















