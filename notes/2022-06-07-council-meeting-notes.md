# Council Meeting Notes June 07, 2022

Community Council (CC) meeting held @ 10 UTC in grincoin#general channel on Keybase. Meeting lasted 60  min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_

* anynomous
* yeastplume
* cekickafa
* dtavarez
* defistaker
* phyro
* deeev



# Short Summary

-  Secure Bulletin Board System and Relay system  discussions.
-  Adaptor Signature Atomic Swap completion and RFC.
-  Hiring and retaining long-term developers.
-  Situation of MWixnet and review by @yeastplume.

 

# Agenda Points & Actions

 

* Last meeting notes here: https://github.com/grincc/agenda/tree/main/notes

* Current meeting [agenda](https://github.com/grincc/agenda/issues/57)
  1)  Update on prospect of SBBS for more user-friendly transactions- bounty, proposal, timetable etc.
  2)  What to do about atomic swap needing completion.
  3)  Update about review of coinswap phase 2 from @scilio
  4)  Open discussions.

 
## 1) Update on prospect of SBBS for more user-friendly transactions- bounty, proposal, timetable etc.
 
__anynomous__ : Our first agenda item for today:
This item was added by jaw709, are you around?



 __yeastplume__ : is there a specific proposal (sorry need afk 5 mins)
__anynomous__ : No, it was a suggestion made by jaw709, not sure who he/she is on the forum on KeyBase.

 __phyro__ : 👋

__cekickafa__ : satoshocrat. admin telegram.

👍 anynomous


__anynomous__ : But, I think in general, it would always be good to brainstorm about a Bulletin Board like system. The suggestion made here is for the beam SBBS system:
https://github.com/BeammW/beam/wiki/Secure-bulletin-board-system-(SBBS)

I did not have much time to read it yet, in short I think encrypted message with PGP in a Bulletin board like system. Hence the name Secure Bulletin Board System (SBBS).

__cekickafa__ : Pinged @satoshocrat, but he is at USA. Maybe timezone problem.


__dtavarez__ : We have been chatting about it but there isn’t a proposal yet
I am personally in favor.

__anynomous__ :  think a bulleting board kind of system would be interesting to enable Non Interactive Transactions, sort of, without any changes to the protocol. Not sure how it compares to Grinbox from the past.
https://github.com/vault713/grinbox

__cekickafa__ : if it does not changes protocol👍

__phyro__ : SBBS still has interactive transactions, it just defines a place to drop a slate/contract.

__defistaker__ : I agree, supporting non interactive transactions would be nice.

__anynomous__ : Exactly, so it give the user experience of non-interactivity, but still interactive. On the other hand, slatepacks already support this. The advantage IMO is that a Bulletin Board allows you share without sharing anything linkable, such as a phone number.
What are your opinions on this @phyro and @yeastplume , I know you also though about a bulleting board system in the past. Not sure it that was the SBBS kind of system, or something else.
To be honest, I think it is a interesting direction to explore, but I simply did no read up enough on the topic to have a well formed opinion.

__phyro__ : I'm not too familiar with these systems to be honest. I tried to think about potential solutions a bit and came up with https://gist.github.com/phyro/1046022377fcb1886a1b4f6500f23773 which is a centralized solution to this. I don't think I've gotten any feedback yet apart from yeast on this
generally speaking, I think the focus was elsewhere, yeast is working on other things and I'm also not focused on sbbs
but I'd welcome more research and thinking how this could be best achieved.

__anynomous__ : Interesting, I cannot remember seeing that proposal before. Maybe it was not on the forum, or I just missed it.

__phyro__ : it's just some thoughts about sbbs things. I usually share these in hopes someone comes up with a way to improve it

__anynomous__ : I think it good to know the sentiment about this. I think there is interest, just nothing concrete yet. I think for now we can put it on a hold. Lets all research it a bit, read all the links:
https://github.com/BeammW/beam/wiki/Secure-bulletin-board-system-(SBBS)

https://gist.github.com/phyro/1046022377fcb1886a1b4f6500f23773

https://github.com/vault713/grinbox

We can also do so on the forum, just gather some opinions and see if there are other solutions/implementations to think about.
In the future if someone has time and willingness, he or she can take on this project if we find a suitable solution.

 __yeastplume__ : From my perspective, I'd like to see some kind of SBBS working as a V1 concept, then worry about how to make it more secure, spam-proof etc.. I think it's more important to get something working to see if anyone will use rather than spending years thinking through all aspects then finding out nobody wants it.

 💯 (anynomous, cekickafa ,phyro ,satoshcrat)

 Grinbox was a good idea (like SMTP for Grin), but it hasn't been developed for some time.

💯(anynomous)

__dtavarez__ : One could expand the p2p messages in order to avoid centralisation but adding more complexity to it, I do not think is the right move.

__anynomous__ : I agree, it should be a add on kind of thing, preferably stand alone, not part of the core messaging protocol.

__yeastplume__ : agreed, I think solutions should be optional and outside core messaging layers
 
 👍 phyro


__phyro__ : 
  >:  __yeastplume__ : From my perspective, I'd like to see some kind of SBBS working as a V1 concept, then worry about how to make it more secure, spam-proof etc.. I think it's more important to get something working to see if anyone will use rather than spending years thinking through all aspects then finding out nobody wants it.   

I tend to agree with this if we keep the solution as a centralized thing and not something on a grin node.

__anynomous__ : It would be best if we find something we can start centralised, but a solution anyone can deploy. In this way we can always go from centralised to semi-decentralised
EDITED
For now I think we can move on to the next agenda item:

## 2) What to do about atomic swap needing completion;

__yeastplume__ : at the moment, we can cross our fingers and wish very hard that atomic swaps were complete.

__anynomous__ : yep, that is about as much as we can do.
This post:
https://forum.grin.mw/t/grin-bitcoin-adaptor-signature-atomic-swap-update-thread/8689

__yeastplume__ : More generally 
1) I think this and the next bullet point are lessons to everyone why development bounties don't work and

 2) I'm looking into ways of hiring more people directly via the core-team, but that's going to take time to see results and I can't really say much more than that at the moment.

 👍 anynomous


 __anynomous__ : We need Reviewers, right?
Or was there a problem with his proposed implementation.
Yes, bounties are fine, but only as an additive solution and with very very good documentation and test cases so others can understand the code.

__phyro__ : iirc, @tromp asked to write a clearer RFC version because it was confusing to understand, but this never happened.

__cekickafa__ :  @geneferneau

__anynomous__ : A yes. @geneferneau Are you still following the project?

__yeastplume__ :

 >__anynomous__ : 
Yes, bounties are fine, but only as an additive solution and with very very good documentation and test cases so others can understand the code.

They're not enough for development. A 'solution' isn't a lump of code, it's continually evolving software that needs someone to maintain it and take care of it over time.

  👍 anynomous,dtavarez


  __phyro__ : I was looking at this and this thing is huge. We most certainly lack manpower to review it. It includes new concepts like an output with shared ownership which includes multiparty rangeproofs I believe etc.

__cekickafa__ : Cant we ask for Jasper help?

__anynomous__ : 

> __yeastplume__ : They're not enough for development. A 'solution' isn't a lump of code, it's continually evolving software that needs someone to maintain it and take care of it over time.

True, that is why it best works for adaptive solutions. E.g. ecosystem, not core related stuff.


__dtavarez__ : I think also multisignature-outputs are required https://github.com/GeneFerneau/grin-rfcs/blob/multisig/text/0000-multisignature-outputs.md

👍 phyro

 __phyro__ :

>__cekickafa__ : Cant we ask for Jasper help?

 I haven't seen him around. This doesn't look like something you review in a day or two, at least not give it a proper review.

__yeastplume__ : I strongly disagree. It don't believe it works at all for any kind of solution, not unless you have a long-term maintenance contract and the maintainers are responsive, which is not the case for either this or the mwmixnet project.

__anynomous__ : Time will tell, without a bounty I am afraid the mwmixnet would not have come farther in any case. So time will have to tell if bounties work at all and for which cases.

__yeastplume__ : Say it's delivered tomorrow and bounties are paid? Who's going to maintain it then?

__anynomous__ : If it is well documented, test cases etc. Anyone can take it on. The difficulty is that most code is coder specific, not well documented etc. and as such hard to maintain or grasp by others. In theory bounties can work, in practice it will be hard for them to work effectively due to these constrains.

__yeastplume__ : It's not a matter of documentation, Any developer can take on any lump of code given enough time. But is anybody going to? Who is lined up for it? If there's a critical bug does everyone just put up with it or stop using it?

__anynomous__ : It is not black and white.
For example, imagine past developers who worked on the grin rust node and wallet code, to take on some task for bounties, not as fixed contractors if they prefer that for some reason. That could work, they understand the way of thinking and the flow of the code in general. I think everyone here prefers dedicated long term developers, but we have to work with what we have for now. Until more dedicated developers either show up, or are developed, trained. Sometimes I think we need something like a trainee program.

__dtavarez__ :

>__anynomous__ : If it is well documented, test cases etc. Anyone can take it on. The difficulty is that most code is coder specific, not well documented etc. and as such hard to maintain or grasp by others. In theory bounties can work, in practice it will be hard for them to work effectively due to these constrains.

The hardest and the more expensive part of development is maintenance
if we will continue with bounties we need to make sure anyone could maintain the code pushed.

👍 anynomous

__anynomous__ : I am agreeing with both of you @yeastplume @dtavarez , but we have to work with what we have. In many cases we know already all that bounties are not suitable for some tasks. So I do not think having bounties 'around' poses a threat to the project, we should just be wise when to deploy them.

__yeastplume__ : Bounties can work in the case of finding/fixing critical bugs or protocol issues, which are by their nature very well-defined and tasks with clear completion criteria. But for general development, which requires ongoing work and discussion, I'm not sold.

👍 anynomous, st_proton, dtavarez

__dtavarez__ : me, neither.

__anynomous__ : Me, neither. How about a trainee program, what are your thoughts on that?

__yeastplume__ : Well, in theory I think the project needs to hire developers. How that can actually happen is a large open question the core team has struggled with throughout
again, I'm looking into options there via the core team.


__anynomous__ : I think one problem is that we have a very large 'threshold' as project. Basically, if you are a developing or novice developer, there is no way to start.

__dtavarez__ : One way could be introduce people to the code and the protocol, fixing low priority bugs, if they get addicted to the yellow, we could discuss how to "hire" them.

__yeastplume__ : okay, but how are you going to pay for them and their health-care benefits?

__defistaker__ : I would be interested in a trainee program, I want to contribute but don't know where to start  like anynomous said :)

__anynomous__ : That is the problem/challange, I would think some sort of lower payment, no health care etc. Just like other long term developers, but with a lower starting amount, slowly going up.
I am not sure if this is a good idea, just something I plaid with on my mind.

__dtavarez__ :

>__yeastplume__ : okay, but how are you going to pay for them and their health-care benefits?

Pay them enough to afford a private solution, but that could be a problem in, say, Germany, I don't know about the rest of Europe.

__yeastplume__ : unfortunately I don't think you'll attract experienced developers under those conditions in the current market
Anyhow, sorry this is a much larger discussion. We can try different approaches between CC and OC teams and see if anything ends up working over the longer term.

__anynomous__ : Indeed. This solution would be mostly for novice, new developers.  Which begs the question how much they can help with developing core code. Ok, just wanted to throw it out here. We can all think about it over time, or discuss it on the forum.

__yeastplume__ : But overall, I think the thinking should be more on the challenges of  'how do we hire and retain longer-term developers' than bounty-based development.

__anynomous__ : I agree there. I think onboarding, is the right term to look for here. How and why would developers get onboarded in Grin.

__dtavarez__ : 

>__anynomous__ : I agree there. I think onboarding, is the right term to look for here. How and why would developers get onboarded in Grin.

let's make a list of TODOs or Things to Fix or whatever we will call it, set priority and difficulty, and assign small bounties for the "low hanging" that will onboard them.

👍 defistaker, satoshocrat

__anynomous__ : We can start with that, and also think if anyone 'aspires' to become a Grin developer, how to get them there. We can discuss further in chat and on the forum.

__dtavarez__ : QAs could even help testing PRs
one does not have to be a developer to contribute.

__anynomous__ : Ok, I think we can discuss it further on the forum. Maybe try different approaches, see which ones work.
For our next topic:
## 3) Update about review of coinswap phase 2 from @scilio
I doubt anyone had time to review it yet. Did anyone have time already to review?

__yeastplume__ : I spent a good while reviewing and trying to run what's there, yes. I left a few comments but my overall impressions here: https://github.com/mimblewimble/mwixnet/pull/3#issuecomment-1142013362

__dtavarez__ : 

>__anynomous__ : I doubt anyone had time to review it yet. Did anyone have time already to review?

29 comments on the PR already
kudos to @yeastplume for his review.
https://github.com/mimblewimble/mwixnet/pull/3

__yeastplume__ : Unfortunately, regardless of milestones I think the project is still very far away from being complete. Without wanting to be disrespectful as the code that is there is generally good.

__anynomous__ : I see, it probably needs more interaction, brainstorming with others.

__yeastplume__ : But the author has not responded to a single comment since April. This combined with the 'plan' as it stands doesn't give me any reassurance that a proper solution will be delivered.

__anynomous__ : As always, communication is key.

__yeastplume__ : That's the biggest red flag. We've had a couple of code drops with some rudiments in there, but no engagement or conversation whatsoever. The interaction between servers (which is the guts of the protocol), hasn't even been discussed. You'd expect there to be conversations about various approaches and back-and-forth as a solution develops, but I don't see any indications that this will suddenly start happening. So unfortunately, most of the engineering challenges still need to be addressed in the project.

__anynomous__ : Ok, well, it is ok to first develop on your own and then enter that discussion. Bust since that discussion came up now, that discussion needs to be had to shape the mix nodes into something we can all work with (and maintain).
It is as it is for now. I think we need to keep reaching out and discuss any issues, or just deliberate some of the approaches used. Maybe some are very well thought of, but probably not always these 'thoughts' have been documented. Then need to be communicated.
Our last item for today is:

## 4) Open discussions.

__anynomous__ : Is there anything that we need to discuss more? I think we already touched upon some other items, in our previous discussion points, such as how to attract developers. These points can be discussed further on the forum.

__dtavarez__ : 

>__anynomous__ : Ok, well, it is ok to first develop on your own and then enter that discussion. Bust since that discussion came up now, that discussion needs to be had to shape the mix nodes into something we can all work with (and maintain).

It is not. I warned this to happens.
We needed a clear documentation.
Then the code.
it is so frustrating to me to be honest.

__anynomous__ : It would have been better, but it is also our 'fault' for not starting the discussions and reviewing faster. We are just understaffed.

__dtavarez__ : I can't.

__yeastplume__ : I don't mind code/documentation being done before or after each other, so long as communication is happening and it's clear the owner is actively working things out and genuinely driving the project.

__dtavarez__ : Now we are in a position where the work is stopped.

__anynomous__ : At least, I think it is clear, we need to have this communication to validate Milestone 2.

👍 Cekickafa

Unfortunate, but let's not just assume the worst yet. My impression is that the intentions and work done has been done genuinely. Lets keep reaching out and see if we can discuss and alleviate anything missing in documentation.

👍 defistaker

__dtavarez__ : it is not communication, there no documentation, no clear view of where we are heading with that
it happened with atomic swaps which is more complicated stuff and now again, with this which is not that complex.

__anynomous__ : That was milestone 1 right...

__yeastplume__ : Let's just say it's about 15% done with no real plan around how we're going to get from where it is now to completion.

__dtavarez__ : exactly.

__anynomous__ : Ok, that sounds like a lower estimate of how much of the work has been done than I assumed. I will have to look at the code to form a real opinion.

__yeastplume__ : And no, this one is really not that complex, there's a bit of server to server interaction needs to be worked out, but nothing that should be hugely challenging.
(and 15% isn't a definite number, but I think it represents the work that should be remaining, in my mind).

__dtavarez__ : should we wait? should someone take responsibility of the PR?

__anynomous__ : I think we just need communication first. If this still hangs in 1 month, we can think of other actions.

👍 defistaker.

__yeastplume__ : I'd like to, but there's another 10 things I'd also like to look at.

__anynomous__ : So, for now, lets put this on pause, until we heard from @scilio

__dtavarez__ : All would have been avoided with well discussed and clear documentation of each agreed milestone... like I warned.
I hate to say it.

__anynomous__ : Ok, well, you could have brought it up as an issue for milestone 1, or did you?
In any case, lets wait for and see.

__yeastplume__ : To be fair, there's no doubt that the lack of reviewers or people available to discuss at the time it was being formed has had an effect
same with lack of review on atomic swaps
But I think we're starting to turn a corner there.

__phyro__ : it's not all gloom and doom tbh. I'm fairly sure we have something that can be picked up and continued which is better than not having anything imo.

👍 anynomous.

__anynomous__ : I think so to, so lets not blame any developers, the blame is with the process, which in turn is a consequence or our current situation with lack of people fore reviewing and developing.

__yeastplume__ : 

>__phyro__ : it's not all gloom and doom tbh. I'm fairly sure we have something that can be picked up and continued which is better than not having anything imo.

yes, as I said what's there is good and usable.

👍 phyro.

__phyro__ : the thing I'm concerned about is the fact that scilio doesn't seem to be around much.

__anynomous__ : Exactly, so lets stay positive and see where we get for now communicating with @scilio

__phyro__ : it's much easier to review things when comments are addressed fast, otherwise you wait for weeks and then you need to get back into it which takes more time.

👍  cekickafa, anynomous.

__deev__ : Been long time not been there, my 2ct would be that we should at least trying to hire (paid) core devs. So there's always someone being able to review, correct, answer to issue and continuously working on grin everyday. When i've been trying to make PR, most were just ignored for months.. Right now seems to me, its on the shoulder of yeastplume only, and its awesome to see him doing that without funding. I would even suggest yeast to request funding for his work. But more active core devs would be better.

👋 phyro, yeastplume , vegycslol, johndavies.

__dtavarez__ :

>__deev__ : Been long time not been there, my 2ct would be that we should at least trying to hire (paid) core devs.

Let's hire you.

__anynomous__ : You are welcome to apply to become a core dev @deeev.

__dtavarez__ : hiring @deeev is a no brainer.

👍 anynomous.

__yeastplume__ : to be clear, I'm funded via the core team

👍 anynomous.

__dtavarez__ : I would love to have @deeev onboarded via the core or the community council.

👍  cekickafa.

__anynomous__ : @deeev Any interest in becoming a Grin core developer, or should I take your silence on the topic as answer ?

__deev__ : For me applying, I need to think more about it. It's a big responsibility. And been a while i've not done anything on grin. My suggestion was not for me being into it. But more on general. For example, i would have loved seeing @geneferneau there.

__yeastplume__ : @deeev  I've PMed you, would love to discuss a bit further.

__anynomous__ : @deeev Well, @geneferneau is also more than welcome to apply. It is just that he has not been around lately.


__phyro__ : @anonymous, core funded contributor would probably need to be roughly as active as igno/antioch were. This is probably a requirement if you're a part of a team.

__yeastplume__ : just the usual expectation from a fullt-time developer on a project.

__phyro__ : true.  👍 

__anynomous__ : Well, part time work for e.g. 3-5 days would also be fine right. As long as the funding is requested for that amount. The activity should basically match the requested funding.

Ok. I think that is all that need to discuss for now.
With that I would like to adjourn this meeting. We can further discuss the various topics on the forum, github or here.
Thanks all for a great meeting.






## *Action points*

* Make a TODO List for fixing/finding issues and assign small bounties to onboard people with developer skills.

* Communicate with @scilio to validate MWixnet Milestone 2

* Discuss with @deeev about hiring as GRIN developer.


**Meeting adjourned.**




              
















