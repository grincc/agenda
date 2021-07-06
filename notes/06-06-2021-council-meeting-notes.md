
# Council Meeting Notes June 06, 2021 

First Community Council (CC) meeting held @ 3PM UTC in grincoin#general channel on Keybase. Meeting lasted ~90 min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

**Community attendence:**

* _mcmmike_
* _mark_hollis_ 
* _dburkett_
* _dtavarez_
* _jankie1800_
* _geneferneau_
* _tromp_
* _phyro_
* _defistaker_
* _anynomous_
* _cekickafa_
* _hendi_

## Agenda Points & Actions

### 1) Status of the multi-sig address

* _mcmmike_ : Currently we are in the process of testing the multi-sig address and each and everyone of the community council is getting familiar with the process. 
We scheduled a meeting with all members of the community council this Friday for setting up the multi-sig address and doing final desaster recovery test over the weekend.
it took us a while to get everyone together and getting time-zones and working schedules aligned with some time where we all are online at the same time.

* _jankie1800_ : I believe there will be proof of access done quarterly for the OC memebrs. Are we planning on setting up a similar safeguard with the CC?

* _cekickafa_: grin council members reachable? can it  take another 2 months to split  those funds:)

* _anynomous_: Yes, indeed we plan a quarterly proof.

* _mcmmike_ : I am not sure if everyone who needs to be reachable is reachable , but we do have contact to some of the OC members.
I think once we are done with our multi-sig address and spending rules, we let the OC know in advanced to be prepared.

* _anynomous_ : Good, in general for this council as well as the other it would be good to hand over keys when it is clear a member cannot provide the time anymore to manage funds/ is not reachable anymore.
Lets make that commitment here, since this council is fresh :)

To me it is also not yet clear if all funds will be made available directly or in portions. Both have their advantages and disadvantages since each council has the risk to lose funds

* _mcmmike_ : I do agree, but we all know the comitment of being part of the GRIN community council is a long-term comitment. 
We should do this check prior to signing date and communicate this publicly if we make changes to the CC members.

* _phyro_ : I'm interested if CC members have experience with managing private keys like these or is it something new to most of the members?

* _mcmmike_ : I can only speak for myself and its othing new to me.

* _anynomous_ : In my case, multisig is new, only know it from theory. I think this is the case for more people since single users do not need a multisig. Anyhow, it is not so complex.

* _phyro_ : the thing I'd want to avoid is checking in 3 months and finding out 2 keys were lost

* _anynomous_ : Lol, that will not happen. I do think everyone knows how to manage keys, only new is that it is used in a multisig setup

* _mcmmike_ : no, I have already a process worked out, where we also being forced to do a desaster recovery test.

* _hendi_ : Nothing new for me

### 2- New Github Organization links, etc

* _mcmmike_: We setup a new github organisation https://github.com/GRIN-Community-Fund where all the CC members are owners of the repository. 
We will build and structure the new organisation over the next few weeks and make everything CC related public there.
I would love to migrate your @_jankie1800_ meeting notes to the https://github.com/GRIN-Community-Fund/agenda repository, where we all (CC members) have PR rights.

* _jankie1800_: is thiis not possible to integrate into the existing github mw repos?

* _mcmmike_ : We dont have PR rights there at least I have no rights at the moment.

* _anynomous_ : O, and for who did not check Discord yet, this is the preliminary design for the logo of the Community Council. keybase://chat/grincoin#general/35465

* _mcmmike_ : we could at least have the CC meeting notes at https://github.com/GRIN-Community-Fund/agenda if you dont mind? @_defistaker_ can help you with it if you need more help.

* _jankie1800_ : my ocd want everything to be in the "correct" place but i understand that in order to move we may need to relocate some data

* _mcmmike_ : I would be fine if we switch at some point when you made your PR sucessfully  on the MW repository. 
please give us some time to stucture the repository(s) but we will make everything CC related public there, also the signing and verifying will be done there.
* _dburkett_ : I'm not sure you would want to. This is an opportunity to do away with the idea that github.com/mimblewimble is official.
	Would probably be good to go with a shorter org name though :)
	https://github.com/grincc is not taken

* _tromp_ : nor is https://github.com/grincoin

* _mcmmike_ : Can we just rename it now to grincc if we all agree ? ( @_hendi_ @_dtavarez_ @_anynomous_ )
Or should we think about it

* _dtavarez_ : I agree, either grincc or grincoin works for me


* _jankie1800_ : i personally like grincc better because its focus should be CC opposed to centralized name like grincoin
* _anynomous_ : In any case it would be best to claim grincoin as domain, to avoid it being missused
* _dburkett_ : I'll give the community council members a minute to snag the org name. If not, I'll grab it and reserve it
* _mcmmike_ :I could rename it, but if we can not agree on it? 
Please send some 👍 from at least 3-4 CC members for renaming the repository to grincc and I will do it right away. 
***_dtavarez_ and _mcmmike_ 👍 ***

 
* _dburkett_: I'm sure everyone is fine with it. We're in a race against time here. I don't want a scammer to grab it
 
* _mcmmike_ : ok I will rename it

* _dburkett_: Thank you :)
* _mcmmike_ :_anynomous_ can you proceed with (3) spending rules please while I rename it

### Topic 3 Spending Rules

* _jankie1800_: would a RFC be applicable here?
_anynomous_ : It would be, we can take inspiration from:
https://github.com/mimblewimble/grin-rfcs/pull/41/commits
In general I think the spending rules are not that dissimilar, however the objective of spending will be shifted somewhat to:

* _mcmmike_ :  We have a new CC home now: https://github.com/grincc

* _anynomous_ :
-Ecosystem development
-Community involvement and activities such as bounties on small tasks, treasure hunts.
So in summary everything that comes with a healthy ecosystem both from a technological perspective as well as from a community involvement perspective. Make it as easy as possible and as fun as possible to join in for all members and use their unique talents for Grin.
Does anyone else have sugestions or remarks on what should absolutely be part or not be part of the spending guidelines RFC for the CC?

* _defistaker_ : promotional efforts
* _anynomous_ : Also what can be improved compared to the guidelines from the OC.
I agree, but with care, so no promotion for other parties, at least not paid.
promotion in this case would be for example treasure hunts, activities for communities, but not google Ads. Although I a sure no one would suggest that here 😉
* _defistaker_: In existing RFC, it was mentioned, Grincon as an example

* _dtavarez_ : I have my doubts regarding of bounties, I don't think that's working as we were expecting before
* _geneferneau_ :have there been additional bounties besides @_mark_hollis_ ?
* _dtavarez_:  I don't think so *** answering to _geneferneau_'s question ***

* _dtavarez_: but I suggest to write something like a RFC for the spending guidelines and the we can agree on that

* _anynomous_ : In this case I am more talking about small bounties.
E.g. we discussed making a bounties, e.g. 800 Grin 1st price, 400 Grin 2nd and 200 Grin 3rd price for Grin tutorial videos.

 
* _mcmmike_ :I was stuggeling to mention it, but perhaps we should not encurage towards development of the rust implementation (but this has to be discussed further and I can explain it in a bit more detail).I think having these two funds , one for the rust development and our CC . 
But this should not exclude we looking for new developers in general !
If we can not agree on a developer between the two funds we most likely can hire one even for the rust implementation.
* _dtavarez_ : My personal opinion is that neither council should discriminate based on implementation. As long as a developer is looking to add value that we agree with, we shouldn't be affected by which implementation is chosen.

* _anynomous_ : Not talking about large bounties yet
* _phyro_ : I wanted to get this one going https://forum.grin.mw/t/bounty-suggestion-inflation-bugs/8628
 
* _mcmmike_ : I fully agree here and we should have a draft on our new GrinCC repositroy for everyone to read and comment.

* _anynomous_ : Sorry, have to switch back to parenting now, I will be reading now and then but not active much in this discussion. So the lead is back to you @_mcmmike_

* _mcmmike_ : to summarize we agreed on making a public RFC for the spending rules and make it public on the new grinCC repositories and add it to the next agenda meeting ? Did I miss something?


* _dtavarez_ : funding activities for communities I think should be supported one way or another
but still I would like to propose this: let's write a well detailed document about expending guidelines and then we can agree on it
 
* _anynomous_ : Yes, we do need an RFC with multiple rounds of feedback

* _dtavarez_ : we want to be transparent and coherent

* _mcmmike_ : I fully agree on this, but from the last two MW meeting, I got the feeling they want to support "only" the rust implementation. My personal oppinion is I am fine to support anyone who works on GRIN in any language he wants.
good, any last thoughts on spending rules  ?  If not we move on

* _dtavarez_ : we have two more topics

* _mcmmike_ : yes I know, just wanted to give a bit more time, not everyone writes as fast

* _dtavarez_ : I will write a draft for the spending rules then we can continue from there

### Topic 4 Funding Requests


* _mcmmike_ : we will move now to multiple funding requests, are we ok with discussing each one or should we add them to a list and talk about it once we agreed on spending rules?

* _jankie1800_ : I dont see any harm in discussing them

* _mcmmike_ : I am just thinking when we discuss them, not based on our agreed spening rules, this could get chaotic? :)
* _jankie1800_ : indeed good point
* _dtavarez_ : we could then consider the lack of spending rules as some kind of blocker for points 4 and 5
* _mcmmike_ : but I want to avoid loosing track of spending request, perhaps @_defistaker_ @_jankie1800_ can compile a list and add them to the next meeting agenda ?
* _jankie1800_ : I can handle this
* _mcmmike_ : are we ok, with not discussing this right now?
*** _jankie1800_, _defistaker_ 👍 ***
* _dtavarez_ : I'm ok
* _mcmmike_ : I would like to schedule a next CC meeting and open the new agenda, any suggestions on a next date? (bi-weekly / once a month / weekly) ?

* _defistaker_ : I think biweekly is best
* _cekickafa_ : https://forum.grin.mw/t/grin-fund-for-mining-idea/7978/30?u=  (Grin Fund for Mining Idea)
* _defistaker_ : I think this will be discussed after spending rules are established.
it was the 5th topic


* _jankie1800_ : i agree with bi-weekly
* _mcmmike_ : Mac wont be able to join the meetings due to his timezone if we keep it bi-weekly at 15 UTC.
* _dtavarez_ : bi-weekly for me is fine
* _mcmmike_ : but I am fine also with bi-weekly, 
@_defistaker_ @_jankie1800_ can someone of you open a new agenda including date and time on https://github.com/grincc/agenda/issues please after the meeting.


* _jankie1800_ : maybe stagger the UTC start time between meetings?
* _mcmmike_ : lets stick to 15:00 UTC for now
* _dtavarez_ : https://github.com/grincc/agenda/issues/2

* _mcmmike_ : if needed we need to give @_jankie1800_ and @_defistaker_ more rights to edit the issues (agenda) otherwise I think only we (owers) can edit each issue.

* _dburkett_: This excludes Mac though. Is there a time where he can be included?
* _mcmmike_ : lets think about if we move every second meeting to fit his time-zone ?
* _defistaker_ : what is his time-zone?
* _mcmmike_ : he told us its 3AM now at his place
* _phyro_ :  I think it's best if we discuss this on the issue for the next meeting or something, since Mac isn't around right now 
* _mcmmike_ : ok, we will add it to the agenda for next meeting and discuss this on Telegram  with Mac
* _dtavarez_ : I think we could leave the time flexible. We want Mac to participate

* _cekickafa_ : ***Sharing a telegram post of mac that stating "My target is 0.05-0.1" *** is it ethic true way that he mentions so lower prices for Grin.
it looks wrong to me and he is member of council
* _anynomous_ : @_cekickafa_ Everyone is free to guess gamble on the bottom, I guessed the current bottom.
* _cekickafa_ : but he is admin. does it look right?

### Topic 5 grin fund for mining
* _mcmmike_ : last point of the agenda:
grin fund for mining @_hendi_ @_anynomous_ please go ahead
on a general note for nhash:
Personally I got in contact with nhash and it seems somehow "legit" they are offering G1 mini and G1 batches from iPollo. But as long as I have not received any new iChickens from them I can not confirm.

* _anynomous_ : As discussed above, would like to have more small bounties and small Grin amounts for activities for the community. To get this grin as well as to contribute to security of Grin we are considering buying some G1 miners from the community fund.
We have not yet discussed much the details, like how many

* _geneferneau_ : can we start a bounty for an open hardware miner design?

* _anynomous_ : I propose to slowly buy in, also because it would not suprise me we will see a G2 mini within a year

* _phyro_ :is the idea to converge to optimal design and have a blueprint for anyone to produce these?

* _anynomous_ : @_geneferneau_ It is an interesting idea, however I think in practice it is hard since costs for development are high, and new designs are continiously made
I think this would make sense after seeing some more miners.
Since there is only one design so far, it is a bit risky since the chance is high a more optimal design is there
But back to topic, what do we all think of buying some G1 mini's from the community fund

* _geneferneau_ : yeah, it would be nice to have an open design, to allow for more producers in the space. possibly crowdfunding productions, using commodity parts, etc.

* _jankie1800_ : i dont think bulk g1-mini is good idea as they had bad QC last batch

* _dtavarez_ : I like the idea of offering a bounty to Lolliedieb maybe so he could try to upgrade the mining software
 
* _anynomous_ : That would be a good investment the whole community could enjoy that.
 
* _dtavarez_ : last time I checked the miner was a really old one and discontinued

* _anynomous_ : I think for now it would be good to further explore these ideas, get some cost estimates.
Regarding Community funds for miners, do we agree to buy in a few, and more if the product lives up to expectation?

* _phyro_ : I left some concerns about the idea on the forum, but I'm ok if others support it

* _cekickafa_ : better buy. it was 16k when first batch g1,  now it is 36 it should have been bought at first time.

* _geneferneau_ : 16k eur per miner? or 16k grin?

* _cekickafa_ : 16k usd for gq
* _mcmmike_ : And keep in mind, we possibly have a GRIN community mining-pool, in the near future. 
But I personally would buy max 1-2 for testnet even @_hendi_ is running the one from @_tromp_ for it. 
And only buy G1 for distributing to community as compensation (funding) and not use for us (CC) as long as we not agreeing on what to spend/use the GRINs we make.
* _cekickafa_ :g1 BİG one 42 gps
* _geneferneau_ : that's fucking insane
* _anynomous_ : Yes, so that would be something to consider, bets to buy G1 or a number of mini's
* _cekickafa_ : we can deliver it to _tromp_. or mike G1 BİG
* _anynomous_ : Ok, in that case, lets start with 1,  I was thinking of smaller number of GPU's though
* _phyro_ : I'm afraid if we'll be throwing real life tasks of running mining operations to CC members they will leave over time because this becomes time consuming
* _anynomous_ @_hendi_ what do you thinking, you have most experience here I think.

* _jankie1800_ : if it is going to fund the GRIN project in perpetuity then maybe NHASH or IPOLLO would robinhood gift us a unit :)
* _anynomous_ :Or at least a nice discount, that would be great, in turn we can share/market our experiences :D
* _phyro_ : That's also something I don't quite understand about the idea, this doesn't generate fund from nothing, someone needs to pay for the electricity and this will be the CC members
* _cekickafa_ : Which part you dont understand? its an economic investment for our trustable currency and distribution OF Grin coins to projects
* _phyro_: if we expect the value to increase over time, then a much simpler strategy with a similar outcome is buying and hodling - both have the same "gambling" nature

* _anynomous_ : The electricity cost we should compensate either by selling some mined grin, or directly with BTC
* _phyro_ : so if we make 1000 Grin profit from block rewards, the CC members will pay ~1000 Grin in electricity

* _mcmmike_ : Please also consider the jouristriction problems which come with mining in general .
* _anynomous_ : @_phyro_ the logistics of that might be a bit of hassle, but I think we can manage. I think we should discuss these obstacles some more before buying

* _anynomous_ : In this case we have two targets, 1) Extra security for the network, 2) steady income of Grin to spend on community activities
which is great for liquidity, many people also asked for more payments in girn.
* _mcmmike_ : Before this gets out of hand, show hands who runs a GRIN node (any RUST or G++) 24/7 ?
(( _phyro_, _mcmmike_, _cekickafa_, _anynomous_ raises hand ))

* _jankie1800_ : I will be :) does that count!?
* _mcmmike_ :  Lets pospone buying G1 for now and think about the benefits of mining with them. 
In the meanwhile setup more GRIN nodes to secure the network, we see low numbers of nodes, at the moment .

* _anynomous_ : Ok, time to put some back up again. Also, I think we should have pre-made Grin pi node packages.
We can discuss this more in the next meeting
* _mcmmike_ : we will be distributing them before christmas and you can make them on your own for now, check Grinnode repositories (3D printing STL; code, etc)

* _hendi_ : *** replying to _anynomous_ question about mining experience***  The 3 G1 minis run flawless now that I have other PSUs and better airflow in the server cabinet. Basically zero maintenance required. Though that could change at a larger scale. But 3 miners is far from "work"
* _anynomous_ : Yes, same experience here, they work fine. But I never managed large amounts of miners
* _mcmmike_ : I would say, we survived out first CC meeting and I say thank you to all participants and CC members who helped me.


**Meeting adjourned.**