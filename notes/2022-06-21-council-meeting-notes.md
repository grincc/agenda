# Council Meeting Notes June 21, 2022

Community Council (CC) meeting held @ 15 UTC in grincoin#general channel on Keybase. Meeting lasted 60  min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_

* anynomous
* yeastplume
* cekickafa
* defistaker
* phyro
* deeev
* renzokuken
* satoshocrat
 

# Short Summary

-  Request funding for @cekickafa as groundskeeper is discussed.
-  GRIN Telegram bot development, implementation flow/documentation is discussed.
-  Bounty GRIN Telegram bot locked for @renzokuken.


 

# Agenda Points & Actions
 

* Last meeting notes here: https://github.com/grincc/agenda/tree/main/notes

* Current meeting [agenda](https://github.com/grincc/agenda/issues/58)
  
  
  1) Telegram bot bounty ; https://forum.grin.mw/t/grin-bounty-suggestions/9866/2?u=renzokuken

  2) Bounty suggestions, https://forum.grin.mw/t/grin-bounty-suggestions/9866/2

  3)  Request for funding @cekickafa; https://forum.grin.mw/t/request-for-funding-cekickafa-june-september/9823/5
 
## 1) Telegram Bot Bounty 


__cekickafa__ :  @renzokuken volunteered for Telegram tipping bot.

__renzokuken__ :  hey guys. Happy to build the bot for you, I like making botz, with or without the bounty... still happy for the bounty because after all, one step closer to 100K ツ which is the only life goal I have at the moment lol

🚀 anynomous, cekickafa, deeev, satoshocrat, johndavies, defistaker.

__anynomous__ : I think the bounties is a great idea. If Renzokuken wants to take on one of the bounties, it means they are already working ;)

💯 defistaker. 🤝 renzozuken, cekickafa ,satoshocrat.

__phyro__ : I'm not familiar with tipping bots, is this a custodial thing?

## 2) Bounty suggestions

__anynomous__ : There are a few other possible bounties I would like to propose, but for that I need input from developers like @yeastplume . If he thinks this is useful and if the rewards is somewhat in the right range of value.
I would like to propose the following bounties:

1) wallet stopes communicating with the node for no apparent reason

•  Identify cause, bounty 0.1 BTC

o  Make solid suggestion how to fix the problem, additional bounty 0.05 BTC

•  Complete identification and solution, 0.2 BTC
2) nodes being out of sync 
•  Identify cause, bounty 0.1 BTC

o  Make solid suggestion how to fix the problem, additional bounty 0.05 BTC

•  Complete identification and solution, 0.2 BTC

__deeev__ : 

>__phyro__ : I'm not familiar with tipping bots, is this a custodial thing?

It is indeed.

👍 phyro.

__anynomous__ : It has to be, otherwise the other person needs a wallet online all the time.

__phyro__ : 

>__deeev__ : It is indeed.

with the ability to withdraw to your wallet?

__anynomous__ : Unless.... we implement some BBS

👍 satoshocrat.

__renzokuken__ : 

>__phyro__ : with the ability to withdraw to your wallet?

Bot could work both ways, deposits and withdrawals, I suggest to make it slatepack based
it would require the owner API running in the network reachable from the bot process, bot process would hold the secret key to access the owner API.


__deeev__ : 

>__phyro__ : with the ability to withdraw to your wallet?

Yes of course, otherwise it useless. I think the main purpose of tipping bot is sort of mainnet faucet for new users in telegram chat.

👍 phyro.

__anynomous__ : Ok, so basically like the EasyGrin wallet, right?

__phyro__ : it would be nice to write the implementation flow down for those of us who aren't familiar 👍

__cekickafa__ : Telegram has huge user base. It is a very good idea tipping bot.

__anynomous__ : It is one of the easiest ways to stimulate real usage. Think like Doge Coin.

💯 cekickafa, satoshocrat

__renzokuken__ : 

>__phyro__ : it would be nice to write the implementation flow down for those of us who aren't familiar 👍

you mean, document how it would be implemented before starting or document the implemented code once done? either is ok for me.

👍 deev

__anynomous__ : I would start with a workflow, general idea we can all understand and provide feedback on. A more detailed documentation after implementation.

__renzokuken__ : sure thing, so like a 1-2 pages doc describing features and how is it going to be implemented for a general overall review, did I understand it correctly?

__phyro__ : 

>__renzokuken__ : you mean, document how it would be implemented before starting or document the implemented code once done? either is ok for me.

might be good before, just so we have some upfront knowledge of what to expect from a bounty completion.

👍 renzokuken

__deeev__ : 

>__anynomous__ : There are a few other possible bounties I would like to propose, but for that I need input from developers like @yeastplume . If he thinks this is usefull and if the rewards is somewhat in the right range of value.
I would like to propose the following bounties:1) wallet stopes communicating with the node for no apparent reason

For the 1, is there any opened issue about it?

__phyro__ : otherwise the completion goal is assumed rather than written down.

__anynomous__ : For now, we can lock the bounty for you @renzokuken.

🎉 cekickafa, satoshocrat 🔥 renzokuken

__renzokuken__ : I totally agree the process should be formal, we should not create a precedence for easily distributed bounties in the future.

👍 phyro, anynomous.

__anynomous__ : @deeev I did not check recently. I knw these are long standing issues, some complains by exchanges, by @dtavarez and by some users who experienced it. There should be Github Issue I guess.
@deeev Since you are a developer. Do you think the bounty amounts are in the right order of value?
Let me just repost these bounty sugestions here:
I would like to propose the following bounties:

1) wallet stopes communicating with the node for no apparent reason

•  Identify cause, bounty 0.1 BTC

o  Make solid suggestion how to fix the problem, additional bounty 0.05 BTC

•  Complete identification and solution, 0.2 BTC

2) nodes being out of sync 

•  Identify cause, bounty 0.1 BTC

o  Make solid suggestion how to fix the problem, additional bounty 0.05 BTC

•  Complete identification and solution, 0.2 BTC

__cekickafa__ : @yeastplume ?
@tromp is good at setting bounties.
Low limit 1 Btc.

__phyro__ : I 'm not sure the objectives are clearly defined, there could be many issues why wallet stops communicating. Likewise there may be more issues why nodes could become out of sync. Is there a concrete issue that's been written down?

__anynomous__ : I think before making it an official bounty, I should first lookup the Github issues. I think the main problem here is that these issues has been reported but not context exist. It could be indeed many issues.

__deeev__ : I agree with phyro on that, might be better to trackdown the issue first, pool logs etc...

__anynomous__ : The main issue is that because these problems are poorly documented, no one is taking them on.

__renzokuken__ : 

>__phyro__ : I 'm not sure the objectives are clearly defined, there could be many issues why wallet stops communicating. Likewise there may be more issues why nodes could become out of sync. Is there a concrete issue that's been written down?


How about the bounty would be distributed the person who reproduces the problem and provides the logs that demonstrate when wallet / node stop responding?

__yeastplume__ : Yes, I don't even think we have a proper issue documenting the problem.

__anynomous__ : Ok, maybe we should start with that. It might be that the logs just tell what is going wrong.
But then again, who is gone run those test and produce those logs.

__deeev__ : 

>__anynomous__ : Ok, maybe we should start with that. It might be that the logs just tell what is going wrong.

__deeev__ : @dtavarez had this issue?

__anynomous__ : He had issues with some nodes being out of sync. He is actually in a good position to spot these issues, since he is running so many virtual nodes.

__renzokuken__ : 

>__deeev__ : @dtavarez had this issue?

I also had this problem and I had it recently, it fixed itself magically.

__anynomous__ : Problem is, he is not available right now and rather overworked with some tasks he is doing for the CC as well as with Grin++.

__renzokuken__ : @phyro gave me suggestions how to document it but it fixed itself before I got the logs of sufficiently low level.

__anynomous__ : Ok. Please, anyone who encounters this issue, run logs and post them on GitHub.
I can understand that these bugs are really frustrating for exchanges and people who build upon Grin. For now, I will postpone making any bounties.

__phyro__ : I think to solve these things, we'd need consistent contributors that know the codebase well.

__deeev__ : Anyone that encountering any issue, should document it throught on github. I would be up to giveaway a small bounty for bug hunters.

👍 phyro

__cekickafa__ : full time?

__anynomous__ : Those are always the 100% best solution to all our problems 😅
But if we do not have those, we might create some bounties to pull people into testing and analysing the code. At least it might save some time for whoever has to fix the issue, which at the moment always is @yeastplume.


__phyro__ : I guess I would like to avoid to make it standard to expect a reward for a bugfix 

👍 deeev, trinitron

__anynomous__ : Just my own opinion, someone does not have to be a full time developer to be a systematic contributor. However, to call someone a core developer... well that would require quite some dedication.

__phyro__ :  but yeah, the shortage is inconvenient.

__anynomous__ : @phyro I agree it should not become a standard. But if a problem is pressing enough to threaten the ecosystem, I think we can make exceptions.

👍 cekickafa

__renzokuken__ :


> __anynomous__ : Those are always the 100% best solution to all our problems.
But if we do not have those, we might create some bounties to pull people into testing and analysing the code. At least it might save some time for whoever has to fix the issue, which at the moment always is @yeastplume.

People liked the bug bash challenge and few times I was asked if it will be run again, maybe an overall bounty program could replace such a challenge, one thing I would like to say, reviewing those reports is also a lot work, sometimes even more than finding them so perhaps a bounty to reproduce a report would also be reasonable.
For instance, you find bug, first requirement is to submit necessary data to reproduce,
second requirement is for someone to reproduce it.
once reproduced both of them get bounty.

__yeastplume__ : Has anyone opened a tracking issue for this?
it's hard to call it 'pressing' when we don't even have a clear bug report, mostly just anecdotal evidence.

__anynomous__ : I have to go now unfortunately.
 
## 3) Request funding for @cekickafa

Before I leave, the council members support the funding of @cekickafa Feedback on his proposal is welcome, but unless anyone has major objections. We approve of his funding request.

👍 defistaker.

__cekickafa__ : 🙏 Thanks for opportunity and trust. I will do my best !

🎉anynomous, defistaker.

__renzokuken__ :

>People liked the bug bash challenge and few times I was asked if it will be run again, maybe an overall bounty program could replace such a challenge, one thing I would like to say, reviewing those reports is also a lot work, sometimes even more than finding them so perhaps a bounty to reproduce a report would also be reasonable.
For instance, you find bug, first requirement is to submit necessary data to reproduce,
second requirement is for someone to reproduce it.
once reproduced both of them get bounty.

this would be an incentive
1. for general audience to regularly try things out and document
2. for more tech oriented and experienced users to keep reviewing and reproducing reports

and all this without causing extra work to the core team, they would be basically getting reproduced case reports with all the data that fits their requirements.

👍 cekickafa, anynomous, defistaker, satoshocrat

__cekickafa__ : i remembered that Grinnode challenge. A few new people joined after that challenge.

💯  satoshocrat.

__phyro__ : having extensive issue reports is always good, but with the current manpower, it doesn't guarantee solving these issues or reviewing them:/
btw, where is Jankie?


__cekickafa__ : He is absent.

👍 phyro.

__defistaker__ : I guess, as all topics are discussed, meeting is over.
gotta go, thanks everyone 👋

__cekickafa__ : well maybe @yeastplume has saying, he joined.

__yeastplume__ : all good, need to go thanks everyone!

__anynomous__ : all good, need to go thanks everyone!


## *Action points*

* Lock Telegram bounty for @renzokuken
* Define objectives clearly for bounties.
* Formalize implementation flow/documentation of GRIN Telegram bot.




**Meeting adjourned.**






























