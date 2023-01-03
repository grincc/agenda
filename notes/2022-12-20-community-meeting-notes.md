
# Community Meeting Notes December 20, 2022

Community Council (CC) meeting held @ 10:00 UTC in grincoin#general channel on Keybase. Meeting lasted 98  min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_

* anynomous
* future3ooo
* cekickafa
* dtavarez
* defistaker
* yeastplume




# Short Summary
 

- Python wrapper bounty is reopened due to @walkbackgod not responding.Developer @nicolasflamel made contributions and volunteered for the bounty. GRINCC supports @nicolasflamel on principle,  feedback from @renokuken will be observed. 
- Request for funding @dtavarez discussed and community voted. Technical deliverables is defined as Grin++ CLI, API & documentation. 
- Request for funding @cekickafa discussed and community voted. Tasks are defined as financials, drafting transactions, keeping account and newsletter.
- Meeting notes task assigned to @satoshocrat, his funding requests will be voted.
- Test miners electricity costs payment is discussed and agreed on paying @mattczt for duty tax bill cost.
- Grin/Wallet Api problem is discussed, focused on getting developers communication to each other so they can respond more quickly. 


# Agenda Points & Actions
 

* Last meeting notes here: https://github.com/grincc/agenda/tree/main/notes

* Current meeting [agenda](https://github.com/grincc/agenda/issues/75)




__anynomous__ : @jaw709  @navie, would be great if you could be there in the CC meeting, even better if you can during the meeting when asked turn of your miner, which will proof that you have been mining on testnet.

Lets take 1 minute to read the agenda, if anyone has any topic to add, please let us know now.☝️
Before starting with the agenda points, I would like to give an update on the TO DO's from last CC meeting.
@cekickafa  tried to contact walkbackgod many times via forum, he read his messages, didnt reply.

For that reason I think it is fine to reopen that bounty. If walkbackgod wants to work on it in the future, that is fine, but if someone else would like to work on it he/she can request to lock it.

👍 future3ooo, defistaker.

__cekickafa__ : yes, indeed.

@nicolasflamel1 done some contribution already i think.

👍 future3ooo, anynomous.

__anynomous__ : Agree, disagree with this decisions 👍 👎

👍 future3ooo, anynomous,defistaker, dtavarez,cekickafa

__future3ooo__ :

>__cekickafa__ : @nicolasflamel1 done some contribution already i think.

Yes, sounds like he wants to pick it up.

__anynomous__ : Ok, we can ask him if he would like to work on it and if so if he would like to lock the bounty to himself.

👍 nicolasflamel1

Any more thumbs up down, for unlocking the bounty @dtavarez @future3000? @defistaker ?


__defistaker__ : @nicolasflamel1 also contributed to exchange-faq, I would like to thank him for that https://github.com/cekickafa/hub/commit/62bbad8c7df19663d936b6b04172c5ed5a3c1884

♥️ future3ooo, 🚀 anynomous

__anynomous__ : Happy to see @nicolasflamel1 has become an active contributor to the project🎉.

💯 cekickafa, future3ooo, defistaker

Ok, lets move on to the agenda for today:



First agenda point:



##  1) Request for funding @davidtavarez January-April 2023.



[Forum discussion]( https://forum.grin.mw/t/request-for-funding-davidtavarez-january-april-2023/10205/2 )

👍 future3ooo

__anynomous__ : My opinion on this funding request is that I am in favour. I always wanted grin rust and grin++ to exist as equals with unified API's for any downstream developers. The only question I have is if this tasks will require 3 months or not. Maybe @yeastplume can better estimate how much time such a task takes.

__dtavarez__ : I want to make it easy for people to develop new things on top of Grin++ now and in the future, but that requires a robust API. And that’s what I want to continue to focus on. The current API is very UI-bound at the moment, and this should be improved. I have been working on improving the API using as a guide the API in Rust, the RFC and adding the changes that I think are important. In order to make sure things are working fine, I will bring to life the CLI version of Grin++, this CLI version should be using the new APIs and it should have a basic compatibility with the Rust API.

👍 anynomous

__future3ooo__ : @nicolasflamel1  please feel free to submit a funding request if you want to contribute more. We need more core devs.

👍 anynomous,defistaker, nicolasflamel1, cekickafa, johndavies.

__dtavarez__ : Recently Satoshocrat managed to compile the master branch for a Raspberry Pi4, this is a huge step, and simplifies the efforts on increasing portability. I would love to make possible to users to run their Grin++ wallets on their Pi4, and a CLI version seems to be more reasonable to me.
just for the record: the SecureAPI flow won't be implemented on Grin++




__anynomous__ : True, Grin++ would be to heavy in its current form on a Raspberry Pi. I run only the rust wallet and node on my pi's.
Regarding the secureAPI, I know this has been debated and many do not like it, I simply have to get experience myself using it to see if indeed it is so hard to handle, or if it actually is a great security feature.


__dtavarez__ : In my personal experience, and in my experience supporting developers, the benefits of the SecureAPI flow do not outweigh the hustle

__anynomous__ : Ok, I think we need more eyes on this/opinions and if needed bug reports, for now you can simply not implement it in Grin++.

__dtavarez__ : but again, that is just my opinion.

__defistaker__ : Can I ask to summarize deliverables on the funding as list items so that I can put it in grincc.mw

👍 anynomous

__dtavarez__ : if someone else writes the flow for Grin++ the code will be of course reviewed and merged potentially.

__anynomous__ : @dtavarez Can you summarize the deliverables.

__dtavarez__ :

>__defistaker__ : Can I ask to summarize deliverables on the funding as list items so that I can put it in grincc.mw

A CLI version runinng on a Pi4 and using the new API can summarize everything.

__defistaker__ : Using the new API on raspberry pi?

__anynomous__ : The new API = a unified API between Grin++ and grin rust? I personally like it more that way.

👍johndavies

__dtavarez__ : compatiable with this API https://docs.rs/grin_wallet_api/latest/grin_wallet_api/trait.OwnerRpc.html

👍 anynomous, defistaker

__anynomous__ : Ok, good. Lets proceed with voting.
Everyone in favour or against funding David for this request (also non-council members can indicate their vote) with 👍👎.

👍johndavies, anynomous, future3ooo, nicolasflamel1

__dtavarez__ : I am in favour 👍

__cekickafa__ : are you voting yourself?

__anynomous__ : David can indicate but his vote is not counted. I need more thumbs there☝️, either up or down, or voice any concerns now.

__dtavarez__ : I did not vote.just made a comment

>__cekickafa__ : are you voting yourself?

why so serious? 😅

__anynomous__ : You could have also commented a vote against yourself :)

😅dtavarez

__cekickafa__ : hehehe

__cekickafa__ : i am serious.Especially about decision. Related to Grin direction.

__dtavarez__ : Grin is fine, Grin will be fine, don't worry

__anynomous__ : No one is allowed to vote for their own funding requests, that would be corrupt. So in the end we take into account all votes and concerns of both regular community members and CC members, but only the CC members vote that result based on that feedback will be used to make the descision.

👍johndavies, cekickafa

__cekickafa__ : no doubt it will be fine.

__anynomous__ : Ok, I have three votes in favour, of which two from non-funded community members, we will need more to finalize the desciscions. I anyone has any more feedback or concerns, voice them now. My only concern would be if the workload is indeed 3 months work full  time.

__cekickafa__ : it is January to April= 4 Months or mistaken ?

__anynomous__ : Good point, 4 months.

__dtavarez__ : I had added more endpoints previously, for example, but then, when I tried to apply them in the desktop version I realized my mistakes at first
So this time instead of writing the C++ code blindly I want to write the implementation right away to make sure they are actually usable
that's why I am including the CLI not just the APIs, so we're talking about the APis, Documentation and a CLI.

__anynomous__ : Ok, I think only other developers can estimate how much time it will take exactly, it will probably also really depend on how you implement it.
For me it is ok to take the vote further to the other CC members since we have also other agenda points to discuss. It is just a pity there are not other developers present here to give their feedback.

Next agenda point.


##     2) Request for funding @cobragrin Dec-March 2023.

[Forum Discussion](https://forum.grin.mw/t/request-for-funding-cobragrin-december-2022-march-2023/10208/4  )



__anynomous__ : We discussed within the CC how much we actually want to spend on Groundkeepers. Since Grin is rather calm right now (actually a good thing for development), we would like to cap total funding of Groundkeepers at 2.5k$.
This would mean that with this funding request, 1500$ would go to @cekickafa and 1000$ would be available for @satoshocrat. There is a lot of room for discussing distribution of tasks.

__dtavarez__ : based on previous discussions the Groundkeepers tasks are the next:
1- Administrative tasks.
2- Writing & Publishment of Developments, upgrades and news
3- Finance PR Contributing to grincc/finance PR for transparency and accountability.
4- Tracking, calculating and making sure the draft are created.
I think @cekickafa is doing an excellent job with the Administrative tasks. I support him continuing to do it.

__cekickafa__ : i would like to keep financial tasks and grin newsletter, tracking and calculating payments . Satoshocrat can take meeting notes.

__dtavarez__ : I think that is quite a load for just one person

__cekickafa__ : i am fine with it.

__anynomous__ : I think that is a reasonable workload for 1.5k$

__cekickafa__ : You said satoshcrat will help you with documentation. my task are clear and transparent.

__dtavarez__ : 4 main tasks, 2 people, 2 main task for each person
is that simple the newsletter is OK so far, but I think there is a space to improve it

__anynomous__ : Probably we can ask volunteers to provide input, like technical pieces or so.

__cekickafa__ : The newsletter's goal is to summarize the most recent and important Grin upgrades and developments so that people know Grin is not dead and can quickly see the status of Grin, save them from having to look for the latest news themselves. Ipollo and Nhash appreciated the newsletter and asked specifically to be recognized in it for their donation of Test miner G1 mini asics.

__dtavarez__ : and I've been clear enough already about what I think in regards of the spending logs and the tracking, and calculation topics

__cekickafa__ : But you will focus on technicals or those financial , governance isssues?

__dtavarez__ : what do you mean?

__cekickafa__ : yeastplume is heavily busy with gui wallet, grin++ and you funded well also and should be responsible for 
acknowledging bug reports and, if possible, attempting to resolve the issues. Renzokuken python is an example

>__cekickafa__ : But you will focus on technicals or those financial , governance isssues?

that is a workload you interfere still i meant.

__anynomous__ : It is easier for developers to detect bugs and make reports because they are the ones encountering them.

👍 cekickafa

__dtavarez__ : I am just saying is it way better just to focus in one or two things instead of 10
and that applies to everyone
I am not writing the newsletter and I am just giving my opinion on how can be better

__cekickafa__ : yes, it will apply to everyone

__dtavarez__ : I can only focus on Grin++ right now for example

__cekickafa__ : Anyone is free to start and contribute a newsletter, hope they do.

__anynomous__ : Can we summarize this and wrap it up, or the meeting will extend to much.

__dtavarez__ : it seems to me we do not have an agreement on what the tasks are for the groundkeepers.

__cekickafa__ : i am fine with GrinCC decision. i will contribute and do my best as usual.

__anynomous__ : Ok, those tasks are the financials, drafting transactions, keeping account and newsletter (of which later in cooperation with Satoshi and anyone who contributes a piece).
I would like to request everyone to vote using 👍 👎

👍 anynomous, defistaker, future3ooo

__dtavarez__ : so indeed we could group the tasks in 4 categories, right?
1- Administrative tasks.
2- Writing & Publishment of Developments, upgrades and news
3- Finance PR Contributing to grincc/finance PR for transparency and accountability.
4- Tracking, calculating and making sure the draft are created.

__future3ooo__ :

>__cekickafa__ : Anyone is free to start and contribute a newsletter, hope they do.

I can start to help assist you with parts of the newsletter if need be.

👍 cekickafa, dtavarez ♥️ johndavies, anynomous

__dtavarez__ : my suggestion is to split the workload in two


__cekickafa__ :

>__future3ooo__ : I can start to help assist you with parts of the newsletter if need be.

thanks, i will give you the contribution rights.

__anynomous__ : Lets not forget the vote ☝️

__dtavarez__ : there is no need for one person to do everything, and by dedicating more time to a task I understand that the final result can be better.
can we move the decision one week?

__anynomous__ : Yes, at @satoshocrat for your funding request we will expect you to be actively involved in the newsletter.
Actually, we can also postpone the vote itself, since both funding requests for groundkeepers are less than a day old, which is a bit short for vote although I can already say I will vote in favour.

__dtavarez__ : just to make sure we are all in the same page

__cekickafa__ : Satoshcrat contributing the newsletter is minimum. So i dont see any benefits about  discussion.

👍 anynomous

__anynomous__ : Ok, in that case we need others like @future3000 to help with checking the text and such.

__cekickafa__ : i will handle the contribution right to @future3000  as well.

__dtavarez__ : the problem here is that it is not clear what is the expectation for each groundkeeper.

__cekickafa__ : it is clear

__dtavarez__ : it is not

__anynomous__ : I think mostly for @cekickafa it is clear, for @satoshocrat we now only have the note keeping, so there is room for either more work-load or less funding.

💯 cekickafa, future3ooo, defistaker


__dtavarez__ : I suggest we split the workload in two and see how things goes

__anynomous__ : I think for @cekickafa the three tasks for 1.5k$ are fine as long as there is some help/input on the newsletter. For @satoshocrat we should have another look at the funding request and see what tasks can be added/removed, as well as what he wants himself.

👍 cekickafa

__dtavarez__ : thing thing is that the newsletter can be improved, and the finance reporting is incomplete

__cekickafa__ : Satoshocrat term is after me. We are one month off of cycle anyway.

>__dtavarez__ : thing thing is that the newsletter can be improved, and the finance reporting is incomplete

Becuz you didnt review it ?

__anynomous__ : I think for example keepting notes + technical tasks such as these for @satoshocrat :

"My proudest contribution this cycle has been undoubtedly troubleshooting and testing successfully the compiling of Grin++ on RPi running Ubuntu 22.04. This task I did have guidance from David Tavarez on the linux-specific processes, but the research and hours of quasi-masochistic trial and error was both fun and fruitful."

Would be fine.

👍 defistaker

__dtavarez__ : the Administrative tasks have been solved by @cekickafa very well not doubt.
I would like to see how @satoshocrat can improve the newsletter

__anynomous__ : That is also an option, but @satoshocrat  should get more involved then. In any case, extending to 1.5$k would be a bit much IMO since then we would spend 3k on basic work while our objective is only 2.5k$ in total.

__future3ooo__ : I’m happy to approve @cekickafa ‘s request now and discuss @satoshocrat ‘s further.

__anynomous__ : I think we can do the final vote in 2 weeks from now, but the discussion here already indicate that most are in favour of approving the funding request from @cekickafa, for @satoshocrat we have to fine tune the workload a bit to fit 1k$
Lets move on to the next topic, since we are already in over time.

__dtavarez__ : I am not in favour as it is right now

__anynomous__ : Ok, can you specify.
Or do you want to pospone that for the forum or the meeting in 2 weeks.

__dtavarez__ : bad in the results, my logic tells me that it is too much of a burden for one person.
I would suggest to pospone the final decision

__cekickafa__ : https://forum.grin.mw/t/cekickafa-progress-update-sept-december/9662/9 

my tasks are trasparent and questionable. We dont need this drama. Job is done. Why this mess ?

👍 johndavies

__anynomous__ : Ok, we need to discuss this more. Based on the results I think @cekickafa has no problem with the tasks assigned, appart from that he needed more input/checking of the newsletter, which only minimally happened.

👍 cekickafa

__dtavarez__ :

>__cekickafa__ : https://forum.grin.mw/t/cekickafa-progress-update-sept-december/9662/9 

my tasks are trasparent and questionable. We dont need this drama. Job is done. Why this mess ?

I have already explained myself several times, it is not drama.

__cekickafa__ : you are complicating everything, offering a problem, presenting it like a solution and complaining and accusing us after it.

__dtavarez__ : I'm sorry if I am not being clear enough that's why I want to suggest to pospone the decision maybe I am getting things wrong

__cekickafa__ : everything is clear.

__anynomous__ : Ok, sorry, I am going to interfere here. 
It is clear that some of us want more discussion, but the general sentiment is clear that there is support for this funding request.
We can leave further discussion for the forum, or the next meeting simply because the post is less than 24 hour old, we agreed we would always give the community around a week to give their input

💗 johndavies

No need to complicate it, but in that way no one can complain.

__cekickafa__ : My funding period already ended on December 15. I need the payment if approved.

__anynomous__ : For me it is simple, the results have been good, newsletter needs more input, so we can give it or @satoshocrat has to step up since he was supposed to do this as well. But again, that discussion is for later.

__dtavarez__ : 1 out of 4 tasks are good

__cekickafa__ : I have organized Grinİstanbul last month and covered all expenses on mine

__dtavarez__ :  2 (the newsletter) can be improved
and the financial logs are awful
I am saying: just focus on 2 out of 4 tasks

__anynomous__ : We can make the vote in 6 days from now, you already have my and @future3000 👍

__cekickafa__ : Thank you.

__anynomous__ : This discussion can be continued on the forum.

__dtavarez__ : good

__cekickafa__ : excellent

__anynomous__ : Our next topic: Sorry, I am combining both for the sake of time,


## 3) Request @jaw709 Jan-April 2023.@navie funding Dec 22- Q1 2023.

__dtavarez__ : https://forum.grin.mw/t/request-for-funding-navie-dec-2022-q1-2023/10210/6?u=davidtavarez

one user offered himselfs to funding this

__anynomous__ : We have to check if indeed that user paid, no need to pay another time

__dtavarez__ : correct. if the userd did not send any transaction, I am in favour of the CC supporting this

__anynomous__ : Also, we could ask them to disconnect their miner, we will see a drop in hashrate, which will give proof they were mining Testnet. Or we just pay on faith.

__cekickafa__ : With Grinmint.com you can connect and check with email.

__dtavarez__ : https://testnet.grinexplorer.net/

they are not using grinmint.com. they are doing solo mining

__anynomous__ : In that case we can ask them to drop the connection as proof.

__dtavarez__ : I provided them with the nodes

__anynomous__ : Ok, we will ask such proof, then we can pay @jaw709 , for @navie we have to check if he already was compensated.
@cekickafa can you contact him on the forum (TO DO for next meeting)?


__cekickafa__ : Sure.

👍 anynomous.

__future3ooo__ : 

>__anynomous__ : Ok, we will ask such proof, then we can pay @jaw709 , for @navie we have to check if he already was compensated.

Ok so pay both now unless naive has been paid.

__cekickafa__ : jaw709=satoshocrat. Mattczt3 runs test miner.

👍 anynomous.

__anynomous__ :  ok.

__cekickafa__ : Mattczt demads duty custom bill for 65 pound and electircity costs 34.5 pound as well

__future3ooo__ :  I don’t like cc paying electric but I’m happy to approve the first payments on good faith. Don’t need to drag out any longer

💯 anynomous

__anynomous__ : Rather expensive, but that is the UK unfortunately.
I am also ok to pay on good faith, since micromanaging costs a a lot of peoples time. But yes, I also would have liked electricity to be paid/volunteered.

💯johndavies

__cekickafa__ : https://github.com/cekickafa/finance/blob/main/pending-payments.md

I will add here.

👍 anynomous.

__anynomous__ : Ok, next and last topic.

## 4) Wallet issues; mimblewimble/grin-wallet.owner api.

__cekickafa__ : yes that is important issue.

__anynomous__ : I can try to reproduce the issue. If one cannot retrieve a transaction log, that is rather bothersome. But maybe the problem has to do with other details, e.g. maybe id=0 should be id=1, I will have a quick look at it this week.
It would be better though if those who have experience with the software answer, such as the developers @yeastplume.
Is there more to discuss regarding this bug that appears to be rather problematic since @Marekyggdrasil is losing his motivation over it?

__defistaker__ : That is the most important thing, He was very motivated on telegram Grin Bot

👍 future3ooo

He even plans to extend it to a general framework for bot development.

__cekickafa__ : @renzokuken is a honest Grin fan. I would like to see him more with Grin developmment

👍 anynomous

__defistaker__ : Grin should not lose a capable developer like him.

__anynomous__ : I hate it when unnecessary problems like these kill someone's enthusiasm, but I can understand. It remains to be determined if it is a problem with help/support, the software, documentation or just bad luck.
In any case we have to take practical issues like these serious.

__future3ooo__ : 

>__cekickafa__ : @renzokuken is a honest Grin fan. I would like to see him more with Grin developmment

Yes, I hope he takes a break to reset and then submits a funding request.

💯cekickafa

__defistaker__ : No one is responding on the issue also.

__yeastplume__ : I have a lot of things going on, but I'd absolutely take this seriously if someone came here and brought it up and said it was affecting their project. Thing is, first I heard about any of this was a twitter rant about how unresponsive devs are. I thought this to be grossly unfair, it's not like he doesn't know how to find me.

👍 anynomous

__anynomous__ : Ok, so in this case it basically was just a missed communication issue. Maybe next time not only report the bug but also directly contact on KeyBase @renzokuken, since I know @yeastplume to be very responsive there.

__yeastplume__ : Unfortunately, putting an issue up on github isn't enough, I have no idea how serious this is for somebody's project unless they let me know about it. If he'd just asked, I'd have looked at it immediately.

💗anynomous, cekickafa

__dtavarez__ : I think he asked

__anynomous__ : Ok, in that case I think we do not need to discuss it further but just to remember to keep close contact and direct communication channels. Also, it is fine for @renzokuken to just take a break of submit a funding request when he is running out of finances of motivation.

💯cekickafa

__dtavarez__ : @yeastplume what would it be the proper way to report things then?

__yeastplume__ :

>__dtavarez__ : I think he asked

He couldn't have asked me directly because I wouldn't have ignored him

__future3ooo__ : 

>__yeastplume__ : Unfortunately, putting an issue up on github isn't enough, I have no idea how serious this is for somebody's project unless they let me know about it. If he'd just asked, I'd have looked at it immediately.

Can you please look into it now ?

__dtavarez__ : 

>__yeastplume__ : He couldn't have asked me directly because I wouldn't have ignored him

that's true

__yeastplume__ : Putting stuff up in github is a good start, but because it's mostly just me on 4 grin-related repos now, I can't prioritize unless people get my attention in some other way.. I do see the issues but it's not always clear that it might be having a huge detrimental effect on someone's project.

__dtavarez__ : to be fair when someone report something on Grin++ they tend to DM me directly but most of the times I do not like it that way

__yeastplume__ : Yes, unfortunately people might need to shout a bit louder if an issue is directly affecting them

👍 johndavies, cekickafa

__cekickafa__ : 

>__yeastplume__ : Yes, unfortunately people might need to shout a bit louder if an issue is directly affecting them

i will take this advise seriously.

__anynomous__ : Unfortunately I have to go right now. Before I leave, I would like to to Thank you all for your input and also make you aware of this thread:
https://forum.grin.mw/t/grin-gui-excitement-thread/10204/31

I hope you are as excited as I am😁🎉!. @yeastplume my virus scanner flags the gui build, I will later look what the problem is, but we should try to avoid that ofcourse.

👍future3ooo

__cekickafa__ : GUI 💛

__yeastplume__ : Anyhow, I am happy to look into it, and will prioritise if he's not taking a break.

👍 anynomous 🚀 cekickafa, future3ooo, anynomous

Heh, only caveat is that nobody's allowed to shout about the GUI yet, it's too new 😀

💗johndavies

__anynomous__ : Thanks all 👋  Feel free to continue the discussion.

👋 defistaker, yeastplume, future3ooo, cekickafa



## *TO DO list*


* Contact @naive about Test Miner electricity payment.

* Get feedback from [Pythoncffi-secp256k1  Wrapper Bounty](https://forum.grin.mw/t/locked-python-cffi-secp256k1-zkp-wrapper-bounty/10030/3) .


 

**Meeting adjourned.**