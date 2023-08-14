

# Community Meeting Notes July 04, 2023

Community Council (CC) meeting held @ 10:00 UTC in grincoin#general channel on Keybase. Meeting lasted 22  min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_


* future3ooo
* anynomous
* phyro
* waynegeorge




# Short Summary
 
- GrinCC wallet information is being discussed and agreed to contact @Hendi for tx output info.
- GRINCC governance format and process of electing new members has been discussed.
- Coinswap progress info/ feedback given by @phyro. 
- Current situation of CC mining farm has been talked and @future3OOO gave feedback about it.

# Agenda Points & Actions
 

* Last meeting notes here: https://github.com/grincc/agenda/tree/main/notes

* Current meeting [agenda](https://github.com/grincc/agenda/issues/94)



__future3000__ :  

## To Do List.

- Forum discussion about creating bounty for HD wallet.
- Feedback for GrinCC member review.
- Financial PR review and GrinCC Wallet report.

## Proposed Agenda

- Update / progress information about Coinswap @scilio @phyro

- Grin CC mining farm update:
  -  How many miners are in operation?
  - What pool are they mining on?
  - Is there a dashboard link that the community can monitor ?
  - How often are miner payouts being sent to the GrinCC wallet and when was the last payment?

- Process for electing new CC member




__anynomous__ : Regarding the To do's, it reads bounty for HD wallet, should be HW wallet. This has been done. There are now four discussion topics for feature proposals including a possible bounty for a HW (Hardware Wallet).

👍 future3ooo

__future3000__ :  Recent post for reference: https://forum.grin.mw/t/funding-proposal-2-bounty-for-a-hardware-wallet-implementation-bounty/10600/21

👍 anonymous

__anynomous__ : Also #TO DO 2  feedback on the forum for reviewing CC candidates has been done. Results, Hendi and David T want to step down as CC members, the rest stays on for now with MCM Mike using a representative, so mostly active as key holder only.

#TO DO 3 The financial pull request, I know it has been reviewed, not sure if it has been pulled yet.

__future3000__ : 

>__anynomous__ : #TO DO 3 The financial pull request, I know it has been reviewed, not sure if it has been pulled yet.


Is the last Cekick payment? https://github.com/grincc/finance/pull/14


## 1) GRINCC wallet info

__future3000__ : Do we have any update on the GrinCC wallet audit?
Is there anything we can do to help?


__anynomous__ : You mean the Grin wallet? I requested Hendi to send the folder with his wallet information and wallet Trxs output. Not received yet.

So either have to wait for that or implement the deepscan bounty I proposed. I am also looking if I can implement it myself, so we can Skipp the bounty, but that is just in my own time.

__future3000__ : Yeah. Has Hendi replied to any DMs about it?

__anynomous__ : Yes, he was not at home, so no access to the wallet. He told me to wait.

👍 future3ooo

__future3000__ : ok, I recall him saying he was away for a few weeks. So we'll bring this back up at the next CC meeting and hopefully you have more info then.

👍 anonymous

## 2) Coinswap Progress

Any updates on Coinswap @scilio ?

Has this been reviewed ? https://github.com/mimblewimble/mwixnet/pull/20/commits

@phyro @yeastplume @tromp


__anynomous__ : I think not yet.

__phyro__ : It's waiting for us to review it. I can't speak for others, but I've had some personal things that came up and have had much less time lately. I think Scilio is working on the reorg scenario protection in the meantime. I'll try give it a pass in the next few days or so.

💓future3ooo, anonymous, jdavies

__future3000__ : Thanks, appreciate the update.

__anynomous__ : No hurry, take your time. Better have a good look than a superficial one.
Should we move to the next topic?

__future3000__ : 

## 3) Grin CC mining farm update:

Bad news:

Found out today from David that the CC farm is not online and all devices are off, due to complications with the facility. 

Here’s the dashboard address here:
https://grinmint.com/dashboard.html?email=grincc.farm.873450.0onqk%408shield.net#

Last payout was on the 30th of April. So I'm assuming it went offline sometime in April.

We knew David no longer wanted any involvement with the CC farm, he’s been vocal about it for some time but no one else put their hand up to take over. However, I don’t think anyone else was aware that the farm was offline until after some discussions today. We thought the miners were still online but payouts from Grin mint were frozen. 

The noted complications with the mining facility were that:

- there were many devices from the first batch that tend to lose the settings on restart
- some other devices were not initializing the miner properly
- late payments
-they had to invest more time and effort maintaining the devices up, that was not their plan.
- Late payments were very annoying for them.

Sounds like the 30% profit share was not sufficient. 

David has passed on the mining facilities contact details, and I’m going to take over and contact them to see what needs to be done to get them back online.

__anynomous__ : Indeed sad news. I expected the farm to be running like normal. I think they shutdown before I made the last payment to them for facility costs.

__phyro__ : Thank you for taking over @future3000

👍 anonymous, waynegeorge

__anynomous__ : This will take some time to sort out, we do not know these people, only through David.
Indeed, thx for taking on this task/burden.

__phyro__ : as a general advice, don't put too much burden on your shoulder. We all have limited amount of free time and only a small part of it can be used for Grin. It's more important to feel comfortable staying around in the long run.

👍 anonymous, future3ooo

__future3000__ : In other news:

I’ve forked the GrinCC site that @defistaker created: https://github.com/stakervali/grincc-next

Can now be found here:  https://github.com/grincc/grincc-next

Community members were complaining about PR’s not being merged, so thought it’s best if CC can manage this moving forward in our own repo, since none of us had write access to make changes.

Have been meaning to reach out to @defistaker to discuss but haven’t had the chance yet.

https://github.com/stakervali/grincc-next

https://github.com/grincc/grincc-website-

Hendi owned the grincc.mw domain, however, it's now in the process of being transferred over to me.  So I'll be repointing the site from the GrinCC repo.

👍 anonymous, 🚀 phyro


## 4) Process of electing new CC Members.

Now we have the confirmation of 2x CC members leaving, We need to discuss the process of electing new CC members. This process needs to be agreed, then documented and used for any new appointments moving forward.
EDITED
Does anyone have any comments on the section process/ criteria?
Regarding the CC BTC wallet: From memory, it was was said before that no more keys would be transferred if another CC member left and that all funds would be sent to a new wallet with new/ continuing member holding the keys.

__waynegeorge__ : There seemed to be an issue related to cc members not carrying out responsibilities consistently. As I understand, the role isn't paid. Perhaps that should change?

__anynomous__ : For me, I have one thing to say. Originak three members were selected as experts, old members and three were elected. I think it might be wise to not make everyone community elected, but also select some trusted members ourselves.


__future3000__ :

>__anynomous__ : For me, I have one thing to say. Original three members were selected as experts, old members and three were elected. I think it might be wise to not make everyone community elected, but also select some trusted members ourselves.

So for example, in this case the community elects 1x member and CC/ OC elects the other member?   How would this work moving forward though, if only 1x member was departing?

__phyro__ :

>__waynegeorge__ : There seemed to be an issue related to cc members not carrying out responsibilities consistently. As I understand, the role isn't paid. Perhaps that should change?

I don't think this role shouldn't come as a huge burden. If it does, something probably needs to change

__waynegeorge__ : I think it takes a fair amount of time to keep up to date with conversations and issues. Perhaps it becomes overwhelming
I'm just wondering if the question should first be whether the current roles/responsibilities system is working

__anynomous__ : I think there is no problem with the system, but we should avoid taking on too many responsibilities as CC members. We only facilitate, we do not need to drive/force the project.

👍 phyro

Paying CC members would be undesirable IMO. 

💓future3ooo, jdavies

That is also why we have a groundskeeper to support us.

__future3000__ : 


>__waynegeorge__ : There seemed to be an issue related to cc members not carrying out responsibilities consistently. As I understand, the role isn't paid. Perhaps that should change?

I don't think CC should be a paid role. Grin is very fortunate to even have funding and having to pay for everything almost goes against the essence of the project. Having paid CC members would bring even more "politics" into it. Gives me the ick just thinking about it. 

IMO the only exception for having a paid CC member would be if they take on all the GK duties and essentially lead the CC and push the direction. 

I do for feel bad for the likes of @anynomous who's taking on alot of the CC burden ( especially in recent times), he's essentially been the lead and consistently been active for years on end now. Probably averages anywhere from 5-10 hours per week on Grin tasks without any compensation( That's the kind of people Grin needs).  I'm personally going to try take on more responsibility, however, having new motivated CC members will certainly help.

💓 anonymous, waynegeorge, phyro

__anynomous__ : I contribute freely with pleasure, I hope others will do so as well.

🚀 phyro, 💓 ardocrat

__yeastplume__ :  hi, just on holidays for two weeks without machine, will respond to any queries then, hope all stays well

👋 anonymous, phyro, arodcrat, future3000

__phyro__ :

>__anynomous__ : I contribute freely with pleasure, I hope others will do so as well.

These things can seem to go unnoticed, but we all appreciate the free time you guys invest.

💓 anonymous, waynegeorge, ardocrat, vegycslol, future3ooo

__waynegeorge__ : I appreciate those views.

__future3000__ : 

>__waynegeorge__ : I'm just wondering if the question should first be whether the current roles/responsibilities system is working

The actual role of a CC member shouldn't be a large burden:

 "Grin Community Council members are primarily representatives of the community and are keyholders of the communit funds. They are expected to responsibly manage the keys of the community fund wallets and manage Funding Requests and Bounties in accordance with the spending guidelines. Although preferred, being an active community member is not a requirement. If a council member cannot participate in the councils activities for a prolonged time, he or she is requested to consider stepping down if more suitable representatives are available. Decision making on funding request as well as defining, checking and reviewing deliverables is a community effort."

However, many in the community have higher expectations and get frustrated with the lack of progress, especially when funds are being spent.  It all becomes very political. 

CC has had issues with questionable spending, timeliness of payments and accounting reports ( GrinCC wallet is still not fully accounted for). So there could be some better systems put in place in that regard, however, there has already been various changes made to rectify this moving forward. We still need to confirm how best to manage the GrinCC wallet and account for all txs. 

The biggest issue is that many lost motivation. Which always happens when a project is down, but more so with Grin because we're a small community with a lack of direction and development. Many have lost faith. Atleast to some degree.

__anynomous__ : I think among all CC members we have to discuss what they want. We have two leaving members, I would propose to for example elect one new member and appoint one other Member selected by the CC on being a long standing and trusted Grin community member.

👍 future3ooo

True, it can be tiring sometimes. The trick is to then take it back a notch, do stuff you like more, then get back in the ring with new motivation.

👍 future3ooo

True, some community members have too high expectations. They just need to realize they have to put in their own effort for change. Anyone can do anything in this project.

👍 phyro

__future3000__ : 

>__anynomous__ : I think among all CC members we have to discuss what they want. We have two leaving members, I would propose to for example elect one new member and appoint one other Member selected by the CC on being a long standing and trusted Grin community member.

Do you mean for the community to elect one member?

👍 anonymous

__anynomous__ : Yes.

__waynegeorge__ : Is there anyone that wants a CC role currently? I remember John Davis wanting it in the past then withdrew
I think Leedan would be a good candidate if he wanted it.

__anynomous__ : Not sure either. I think the CC. Can make a hot list of community members to ask to become 5th member after selecting one continue asking community members if they are willing to be part of an election for the 6th member

Also community members who want to can join this election.

__future3000__ : 

>__anynomous__ : Yes.

That sounds reasonable to me, especially this time around. However, I want us to come up with a predefined process for electing new members that the majority are happy with. For example, I don't want people crying if only 1x other CC members leaves and then the CC appoints a new member with no community input.

__anynomous__ : Good point. I think we should for example replace the remaining two appointed members (Hendi and MCM Mike) only with appointed members. For the other 4 members, if they step down we can make elections.
We started with four appointed and only 2 elected members, now we go to 4 elected, 2 appointed.
This makes sense since we need to always have some "experts" in the CC for good decision making. So partly democratic, partly technocratic.

💓 future3ooo

__future3000__ : 

>__waynegeorge__ : Is there anyone that wants a CC role currently? I remember John Davis wanting it in the past then withdrew

I'd be happy with @johndavies24 he's gonna blow up at us from time to time 😂 but he's trustworthy, offers good insight and has been motivated enough to stay engaged for years on end now.

__anynomous__ : True, well if you can manage his outbursts I do not mind😉. I think he can be elected, quite certain he would get enough votes.

This time we have to plan enough time for the election, I do not want to repeat the same drama as last time.

__future3000__ : 

>__anynomous__ : Good point. I think we should for example replace the remaining two appointed members (Hendi and MCM Mike) only with appointed members. For the other 4 members, if they step down we can make elections.
We started with four appointed and only 2 elected members, now we go to 4 elected, 2 appointed.

I don't think it matters much anymore who was initially appointed/ elected, but having technical people on CC is critical.

👍 ardocrat

>__anynomous__ : This time we have to plan enough time for the election, I do not want to repeat the same drama as last time.

Yeah for sure, I propose to create a forum post announcing the 'election' that follows the structure from the original "Call for Grin Community Candidates" post https://forum.grin.mw/t/call-for-grin-community-candidates-for-additional-fund-granting-control/8521

 There should be a cut off date when all applications must be made by.  We could time the cut off date to align with a Grin Newsletter, so all Candidates would get mentioned at the same time. The votes could then be counted some days later.

 >__anynomous__ : I think among all CC members we have to discuss what they want. We have two leaving members, I would propose to for example elect one new member and appoint one other Member selected by the CC on being a long standing and trusted Grin community member.

Before we move ahead on this, let's get some more feedback.
But for now. Meeting adjourned 🔨


@cekickafa plz add this follow up to the agenda for the next CC meeting 🙏

👍 cekickafa



## *TO DO List*


 
*  Getting wallet information and wallet Txs output from @hendi.
    
* Discuss and create predefined process ( that gets documented in the CC repo) for electing/ appointing new CC members moving forward.




**Meeting adjourned.**



