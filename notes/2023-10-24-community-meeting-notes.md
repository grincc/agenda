
# Community Meeting Notes October 24, 2023

Community Council (CC) meeting held @ 10:00 UTC in grincoin#general channel on Keybase. Meeting lasted 74  min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.




### _Community attendance:_

* yeastplume
* waynegeorge
* ardocrat
* anonymous
* cekickafa
* phyro


# Short Summary
 
-   
 -  Grin 2020 wishlist is being discussed 
 - Future of Grin; wishlist- projections and essential ecosystem components are being spoken about.
 

# Agenda Points & Actions
 

* Last meeting notes here: https://github.com/grincc/agenda/tree/main/notes

* Current meeting [agenda](https://github.com/grincc/agenda/issues/113)



__anynomous__ : 


I added a status update for each item that I had any knowledge of, perhaps @yeastplume can fill in some of the blanks or correct me if I am wrong anywhere:

## Criticals / Must Have

1. [PIBD - (faster and more robust syncing strategy)](https://github.com/stakervali/grin-wishlist/issues/6)
In beta and being tested on mainnet
2. [multi-sig*](https://github.com/stakervali/grin-wishlist/issues/2)
Is not happening any time soon if I understand correctly, since there is no solution yet to generate threshold range proofs:
3. Wallet backend improvements
not very specific, I know the wallet had some bug fixes and stability improvements, are those what are referred to?
Many improvements and move towards contract flow with unified payment proofs
https://github.com/mimblewimble/grin-wallet/pulls?q=is%3Apr+ 
4. libsecp fork update 
 not updated, last commit to was 5 years ago 
5. safe cancel*
WIP, not merged https://github.com/mimblewimble/grin-rfcs/pull/71 

## Important

1. Tor support for nodes*
2. [light node*](https://github.com/stakervali/grin-wishlist/issues/7)
3. [testnet exchange/ making it easier for exchange integrations](https://github.com/stakervali/grin-wishlist/issues/4)
4. payjoins*
5. [binaries for older systems, older GLIBC or build on low RAM machine < 300MB]()
6. [invoice payment proofs*](https://github.com/stakervali/grin-wishlist/issues/10)
7. hardware wallets*

## Fix if time / Nice to Have

1. wallet view key*
2. [one-time use slatepack addresses for wallet*](https://github.com/stakervali/grin-wishlist/issues/11)
-Generate new slatepack address is implemented in Grin++, not yet in grin-wallet
3. flyclient*
-Nothing implemented, would require header history or inclusion proof according to discussions on KeyBase
4. [atomic swaps*](https://github.com/stakervali/grin-wishlist/issues/1)
-Gene made a first implementation of "bad" atomic swap, grin reaper offered to continue implementation, nothing fixed yet. Should the bounty be reopened? 
https://forum.grin.mw/t/questions-about-the-state-of-the-atomic-swap-pr-and-introduction/10332
https://github.com/mimblewimble/grin-rfcs/pull/83
5. aggregators
-mw MixNet/CoinSwap, third stage under review with two open issues out of 9 issues
https://forum.grin.mw/t/request-for-funding-scilio-coinswap-implementation/9149**
https://github.com/mimblewimble/mwixnet/issues/11
6. block archive node support*
-Implemented
7. [improve compatibility with OSX](https://github.com/stakervali/grin-wishlist/issues/3)
No specific changes as far as I know
8. anchors*
9. bulletproofs+*
-Not deemed safe yet I think, or was that bulletproofs++
10. NRD activation*
11. [Display slatepacks as QR codes in CLI
Implemented




__yeastplume__ : I think it's a good idea to have that, but what's there now is from a good while ago and I only just learned about this an hour ago. Maybe we can do this over a couple of weeks and look at an updated list then?

👍 anonymous

__anynomous__ : O, I forgot to mention that in the announcements
the idea is to have the exact same two topics in our discussion in 2 weeks from now at 19:00 UTC, especially since not everyone could join and one more CC member last minute bailed on us.

So this like a work in progress update where we are now and where we want to be in the coming years. Not something to brush over in one meeting.
I do not think we need to discuss today much in detail. What supprised me a little is that it appears as many changes happened in the Nice to have and not in the critical must have section.

__cekickafa__ : Sorry, critical must have is in order or it is randomly ?

__yeastplume__ : well, PIBD is pretty huge and important and that was done. safe cancel is part of the ongoing experimental contracts work

__anynomous__ : Those are the most important ones for me, only pity multisig is not yet in the cards, but in time.
One more question, is safe-cancel now implemented, or will it be in the new GUI wallet?

__yeastplume__ : there's a lot going on at the moment that isn't reflected in the list either. I think it would be best to have this posted somewhere for comments so we can take time to look at it and update
it's part of the contracts work, experimental and not 'done'. All of the experimental work is going into the gui wallet

👍 anonymous

__cekickafa__ : i mean safe cancel should be iplemented before multisig or vice versa ?

__anynomous__ : Sure, we will add it somewhere on github for everyone to update.
I will add the version with my updates here, anyone can edit to make more changes/updates

👍 cekickafa

https://github.com/stakervali/grin-wishlist

How is the development going with the GUI going @yeastplume ?

__yeastplume__ : It's going well, with contracts and early proofs and support for mwmixnet in there, but I'm not seeing a lot of people picking it up and trying things.

__anynomous__ : Ok, so it is ready for people to try out?

__yeastplume__ : I'm trying to get all of the new features there and visible in the one place

__anynomous__ : With testnet or do you think it is safe to use with mainnet already?

__yeastplume__ : it's always ready for people to try out
You need to manually select 'contracts' mode, I'd only use that on testnet for the moment

__anynomous__ : Ok.

__yeastplume__ : regular legacy transactions are on by default, they should be fine to try on mainnet.

__anynomous__ : If you think it is ready for testing, perhaps put it in a forum post with a link and some minimal instructions (and safety warnings 😛). I think some people would start testing. I would, but I would need some testcoins.

💯 ceckickafa

__yeastplume__ : I barely have any testnet coins either

__anynomous__ : Is the Testnet API faucet from @quentinlesceller still operational?

I guess we should fix that before asking people to test.

__cekickafa__ : i dont think it is operational.

__yeastplume__ : maybe if whoeever is mining can make then available

__anynomous__ : That would also work, not sure who is mining it at the moment. My miners al died, otherwise I could provide some.
#TO DO, @anynomous will contact the testnet miners on the forum and ask if they would be willing to distribute Testnet coins, or send some to me or @cekickafa to distribute them to those who want to do testing of the GUI wallet.

👍 cekickafa, vegycslol, yeastplume

__anynomous__ : Perhaps we can ask Quentin for his faucet code, so we can create some more Testnet faucets.

I think for now that is all we need to discuss on our first agenda topic,revisiting the Wishlist

__cekickafa__ : Testnet explorer is not active fyi.

👍 anynomous

## 2)  Grin Ecosystem wishlist, were are we now and where do we want to be in 2-4 years?

__anynomous__ : Again, this is an open question to think about longer than 5 minutes, we will revisit the topic in two weeks from now so all CC members can have their say.

__cekickafa__ : Frankly my personal opinion, i wouldnt' ve thought Grin would be in that current position according to 2019-2020.

__anynomous__ : In which way, would you expect more developments or less, if so which ones?

__cekickafa__ : in all terms, which one shall i count ? That wishlist is from 2020.

Multisig is done by gene at 2021. I repeat it is my sole view, i dont have the knowledge of tech development. In general terms, Grin is out of sight more than 2020.

__ardocrat__ :

>__anynomous__ : 
I added a status update for each item that I had any knowledge of, perhaps @yeastplume can fill in some of the blanks or correct me if I am wrong anywhere:

Hello, multisig as I see we have here as part of atomic swaps PR:
https://github.com/mimblewimble/grin-wallet/pull/618

__anynomous__ : I do agree that some developments were slower than I expected. However, I do think we haver to be nuanced in looking at topics by dividing them by those that were already technically perfectly feasible, and those that were not yet ready to implement.
E.g. PIDB was ready to be implemented and is mostly done, which is a rather major one. Also the new GU wallet and contract flow a a big upgrade.
But I agree on the multisig, that one suprissed me a little. I think it was mostly because gene simply dropped it instead of fixing it.

__cekickafa__ : Grin became introverted simply.

__anynomous__ : It went in bear marked mode 🧸 . But I have to warn to not think that there were no developments, a lot happened.
For me, the most important things are there. 
- Grin++ works great except for some bugs with cancelling transaction and some node issues. Grin++ has the option to generate new slatepack addresses which is great. Iron Belly works fine, and grin-wallet is much more stable and useful lately, actually a lot of updates here that most people did not notice:
https://github.com/mimblewimble/grin-wallet/pulls?page=2&q=is%3Apr
- MW mixnet nearly finished actually, just two more issues to solve.
- PIBD nearly there

__ardocrat__ : Safe cancel is must have I agree, had a bug on cancel already sent tx, so wallet repair required.

__anynomous__ : 1) multisig
2) atomic swap
3) bounty for Telegram bot
4) Web payment plugin
.. add here

__ardocrat__ : 5) Hardware wallet :)

__cekickafa__ : 

>__ardocrat__ : Safe cancel is must have I agree, had a bug on cancel already sent tx, so wallet repair required.

i got many DM s about this. Users trying to cancel, becuz they think tx not happened and there becomes a conflict. Is that the same issue ?

__ardocrat__ : Possibly

👍 cekickafa

__anynomous__ : A yes, we have one, but I am still in favour of more options:
https://forum.grin.mw/t/funding-proposal-2-bounty-for-a-hardware-wallet-implementation-bounty/10600

__ardocrat__ : And some weird issue when sent transaction is not confirming
Possibly issue with Dandelion

__anynomous__ : There is an issue in Grin++, that the status after cancelling is not properly updated, or is there also an issue with grin-wallet @ardocrat 
https://github.com/GrinPlusPlus/GrinPlusPlus/issues/230

__ardocrat__ : Must be critical..

💯 ceckickafa, ardocrat

__anynomous__ : See this issues (link above), made a while back. Yes that is critical, also Grin++ tends to block grin rust nodes, which I would consider critical, chain split anyone 

__cekickafa__ : yes, most of them (DM guys) were using Grin++. I have no idea if it is related.

__anynomous__ : Ok, but here is a difficult question.. which thinks do we ACTUALLY NEED that we do not have?
For me it is those critical issues, PIDB, contracts, safe-cancel, unified payment proofs (all worked on in the GUI wallet), multisig, atomic swap (these last two ones are an issue we should fix in the coming year(s) IMO)

>__cekickafa__ : yes, most of them (DM guys) were using Grin++. I have no idea if it is related.

It is, I had the exact same issue, even contact David about it today by coincidence

👍 cekickafa

__cekickafa__ : Mulitsig for coming years ? why, it was on the critical top list since 2020

__ardocrat__ : 

>__ardocrat__ : Must be critical..

https://github.com/mimblewimble/grin/issues/2880

__anynomous__ : For me the multisig is becomming more important because we might need it for a custom HW wallet implementation, see the bounty I linked a few post backs.

__ardocrat__ : 

>__cekickafa__ : Mulitsig for coming years ? why, it was on the critical top list since 2020

I guess we need to check Gene implementation,MWC has swaps for a long time :)
Multisig is part of them

__anynomous__ : Also we have someone who actually wants to work on it:
https://forum.grin.mw/t/questions-about-the-state-of-the-atomic-swap-pr-and-introduction/10332

If the OC does not want to, we can make our own bounty. But perhaps the OC wants to reopen the bounty for it. I have to check how much it was.

👍 cekickafa

__cekickafa__ : 50k $

👍 anynomous

he is @grinreaper who wanted to work. İdk if he is around.

__anynomous__ : Ok, well if BTC stays above 30k (I expect it to crash somewhere soon), then we can open a bounty, but first we should ask the OC members.
@phyro Do you know the status of the 50k bounty for atomic swap, is it still locked to @geneferneau or is it open, since we have someone willing to work on it?
https://forum.grin.mw/t/questions-about-the-state-of-the-atomic-swap-pr-and-introduction/10332

__ardocrat__ : 

>__anynomous__ : Also we have someone who actually wants to work on it:
https://forum.grin.mw/t/questions-about-the-state-of-the-atomic-swap-pr-and-introduction/10332

We just need to finish Gene implementation I guess

__cekickafa__ : 

>__anynomous__ : Ok, well if BTC stays above 30k (I expect it to crash somewhere soon), then we can open a bounty, but first we should ask the OC members.
@phyro Do you know the status of the 50k bounty for atomic swap

50k$ was for Hardware wallet imo.

__anynomous__ : Not sure, he chose a less safe option, we should reread again the details and why the OC thought this implementation might not be a good idea.
It is a lot of comparing of technical details and pro and cos.

__yeastplume__ : It's open as far as I know. I will not be advocating bounties personally. They don't work and they cause all sorts of trouble.
But that's just my opinion.

__cekickafa__ : 40k euro Gene requested for atomic swaps.

__anynomous__ : Can you specify the issue @yeastplume I 100% agree that having good devs on payroll is prefered, but since we have limits there, what is the bottleneck with hired musscle, is it the reviewing taking to much time, code quality, maintainability (documentation etc.), all of these or something else?

__yeastplume__ : you can't develop software with temporary hired teams. you need people dedicated longer-term.

👍 ardocrat,vegyclol, waynegeorge

__anynomous__ : Ok, but since someone is offering to work on it, what would in your opinion be a good solution. Offer them a position, perhaps first on tryout?

__yeastplume__ : people just do enough to cover the bounty requirements and little else, leaving the heavy lifting on us, and me in particular at the moment

__ardocrat__ : 

>__yeastplume__ : you can't develop software with temporary hired teams. you need people dedicated longer-term.

Not needed to hire, with bounty payment afterwards should be OK, as at any open source project :)

__anynomous__ : That makes bounties not very scalable indeed, if in the end implementing it take to much time.

__yeastplume__ : Again, I'm not in favour of if and I'm not agreeing to review any code produced by one. If you issue a bounty for something, you need to have a plan to review it that's not assuming we're going to do it then maintain it afterwards

👍 anonymous,vegyclol

__anynomous__ :  Does the OC offer more long term positions, or should the CC consider doing so. I have no problem with good old fashioned Funding Requests for long term devs.

__ardocrat__ : Just no more upfront payments, let them work till working result

__phyro__ : I can't recall correctly, but if my memory serves me right, it's not finished? There was a PR opened from Gene on this but we didn't have enough man force to review it (nor do I think we have it today).

__anynomous__ : If I remember correctly, gene did not implement all feedback, which was a major rewrite and tackling a couple of issues.

__phyro__ : I also agree with yeast, bounties put a lot of review and maintenance responsibility on everyone that may not be well thought out
I think tromp had some questions that were not addressed

__anynomous__ : Ok, so reopening is pointless then. I mean the CC is unfortunately not technically capable of reviewing any core tech.

__ardocrat__ : So if nobody can review anything, how will continue to work :)

💯 ceckickafa

__anynomous__ : To me it seems that the real solution is simply getting more long term devs.
Bounties are just a payment form, so the question is how to make sure funding is available, and we get the right kind of devs.

Developers :) yeah, we need more people willing to dive into the code and do things

__yeastplume__ : agreed

__ardocrat__ : 

> __anynomous__ : To me it seems that the real solution is simply getting more long term devs.

Sure, but how they will work, anyway we have repository maintainers and PRs to check
We still need to check code :)

__yeastplume__ : who is 'we' here?

__phyro__ : make small PRs, earn trust, make larger PRs

__anynomous__ : Do you see a way to increase the number of people doing that?
I mean I am even trying to learn Rust for Grins sake, but I have to admit diving in the core code is just a major challenge, even if you are somewhat technical.

__ardocrat__ : 

>__yeastplume__ : who is 'we' here?

Developers :)

__phyro__ : 

>__phyro__ : make small PRs, earn trust, make larger PRs

that's usually how trust is built over time for any project, I don't see Grin being an exception here

👍 ardocrat

__yeastplume__ : yes, exactly, even if it takes a while

__phyro__ :  perhaps if we're touching some critical parts, it might take more time to review but there's a lot that can be done around these parts

👍 ardocrat

__ardocrat__ : 

>__phyro__ : that's usually how trust is built over time for any project, I don't see Grin being an exception here

Small PRs I see can be checked easily, more large can take months or years..

__anynomous__ : So in summary, it cannot be forced. More bounties can only work if we would have more core devs and even then it is not efficient since the actual implementation in the node and wallet takes a lot of time + time spend on reviewing.
I think I agree there. Bounties only work for decoupled projects, e.g. ecosystem projects build on top of API's etc.

__yeastplume__ : changes to core functionality and the ability to review them effectively require a knowlege of the code and inner workings that take a very long time to develop.

👍 phyro

bounties are fine for small one-off things, but for functionality or core changes they end up creating more work for everyone else
than it's worth

__anynomous__ : Ok, I think we can record these arguments somewhere, since people tend to repeat this discussion on bounties, while each time the conclusion is the same, that bounties do not work that well, at least not for anything core related.

__cekickafa__ : i think there is a mismatch here.
Everything fall on core shoulders, and review, maintenance etc is a work load. Maybe core team should be expanded.

💯 anynomous

__anynomous__ : It should be. The problem is that to get those people is hard since they need to gradually get to know the code basis by doing error reporting, small bug fixes etc. Build a reputation by doing and not by first asking money.

👍 phyro, ardocrat

__cekickafa__ : Discussion about 2020 wishlist, we are at 2024 almost.

__yeastplume__ : 

>__cekickafa__ : Discussion about 2020 wishlist, we are at 2024 almost.

4 years later and we're still here with active development and people who care about the thing? I think that's an acheivement, not a problem


👍 phyro, cekickafa, jdavies

__phyro__ : especially during these hard times :)

__cekickafa__ : That we dont have man power became a broken record. Like it or not, it is open source project, no any other project come close to Grin and minimum interest is not acceptable.

__phyro__ : are you going to review mwixnet cekickafa?

__cekickafa__ : 

>__yeastplume__ : 4 years later and we're still here with active development and people who care about the thing? I think that's an acheivement, not a problem

i am agreeing with you about review and maintenance is a problem.

__anynomous__ : I think this nicely touches on the discussion why Bitcoin is unique and Tromps response:
https://news.ycombinator.com/item?id=37979829

Bitcoin is so successful partly by staying simple, by being conservative. Grin is the same in that respect, it is like the Chinese having a 10 year plan. It is not so much in quantity or speed, but by only adding what really should be added that Bitcoin is a great project. Grin is no different in that respect.

__yeastplume__ : I've tried several times with mwmixnet, done wallet integration code which is ready to undergo testing. I've asked the community to look at it and perhaps try running servers so we can have a closer look at it

__phyro__ : as people have said here, the problem is that you need people interested in Grin enough to dive into it. This means learning MW in depth, learning what structures Grin picked to implement it both in node and wallet side

__cekickafa__ : 

>__phyro__ : are you going to review mwixnet cekickafa?

what is the purpose of this question ? i am trying to find a solution to review and maintenance, lack of developer problem. Why are you tirggered ?

__phyro__ : Hmm, I may have interpreted you bold statement wrongly

👍  cekickafa

__anynomous__ : Actually, we are farther along with things like PIDB and contracts than I anticipated a year back. Only multisig and atomic swap take a bit longer than expected.

__ardocrat__ : 

>__anynomous__ : It should be. The problem is that to get those people is hard since they need to gradually get to know the code basis by doing error reporting, small bug fixes etc. Build a reputation by doing and not by first asking money.

Grin is money, my personal motivation is to make it better, so everyone can use without problems

👍 anynomous

__cekickafa__ : 

>__phyro__ : Hmm, I may have interpreted you bold statement wrongly

bold statement is our problem. We dont have enough man, and it is a problem to be solved. Yeastplume is right about longer contribution about review and bug, maintenance i meant fyi.

👍 phyro

__phyro__ :

>__yeastplume__ : I've tried several times with mwmixnet, done wallet integration code which is ready to undergo testing. I've asked the community to look at it and perhaps try running servers so we can have a closer look at it

testing things out is a task that doesn't take long to onboard. Testing mwixnet features is a good easy task for any volunteers :)

👍 anynomous,yeastplume  💯 cekickafa, ardocrat

the question is just about who's going to roll up their sleeves and do the work

__anynomous__ : @cekickafa It is sometimes indeed surprising that not all crypto enthusiast see Grin for the 💎 that it is. but I might be prejudiced.
Indeed, we could let the community do more testing. I think the trick is here simply to use the forum, not expect them to actively monitor Github or KeyBase.

__ardocrat__ : 

>__phyro__ : testing things out is a task that doesn't take long to onboard. Testing mwixnet features is a good easy task for any volunteers :)

Let's build testing plan and will make an announcement like we did with pibd @cekickafa

👍 anynomous, cekickafa

__yeastplume__ : yes, that's definitely something I think the CC can do that would help a lot

__anynomous__ : That worked reasonably well for PIDB, so we can do the same for GUI wallet and for Mixnet. Perhaps, only one at a time.

__phyro__ : Yeah that's good. A simple individual testing would also help as a start as we don't really know the state of the thing at the moment
at least I don't know it

__anynomous__ : Lets start with the GUI testing, I think it simpler than setting up a Mixnet server.

__yeastplume__ : Well, the GUI is really an OC thing, and I'm saving more general testing for when all of the new contracts-related work are integrated and evident
that's contracts, early payment proofs and mwmixnet sending?

__anynomous__ : Ok, so what would you like to have tested frist. In any case, you can control it simply by what you post on the forum. Whatever you post, some people will jump on it.

__yeastplume__ : so having a mixnet first would help that

👍 anynomous 

so I'm just saying mwmixnet would be far better for CC to focus on at the moment

👍 anynomous 


__phyro__ : also don't be afraid of asking questions here. It wouldn't hurt to make these channels more active ;)

👍 anynomous , ardocrat


__anynomous__ : True, I think many are hesitant to ask questions.
For now, I think we can adjourn this meeting. After that I might ask some questions 😉
Thanks all, see you next time, same topics, hopefully I can make a better overview by then

## *TO DO List*

* Mwixnet testing by community.

* Testnet coins distribution.






**Meeting adjourned.**
