
# Community Meeting Notes September 13, 2022

Community Council (CC) meeting held @ 15:00 UTC in grincoin#general channel on Keybase. Meeting lasted 59  min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_

* dtavarez
* cekickafa
* defistaker
* yeastplume
* deeev
* renzokuken
* phyro
* anynomous
* vegycslol


# Short Summary
 
-  Biweekly Meeting schedule affirmed.
-  Bounty for writing a CFFI wrapper of secp256k1-zkp fork. (https://forum.grin.mw/requesting-help-with-writing-a-cffi-wrapper-of-our-secp256k1-zkp-fork/10024 ) has been discussed.
- Retroactive Grants like idea (https://blog.opengsn.org/taking-retroactive-grants-from-concept-to-practice-at-gitcoin-grants-round-11-649497d08519).


# Agenda Points & Actions
 

* Last meeting notes here: https://github.com/grincc/agenda/tree/main/notes

* Current meeting [agenda](https://github.com/grincc/agenda/issues/66)


__dtavarez__ : @cekickafa would mind to introduce the first item of the agenda?

__cekickafa__ :
 ##  1) Community Biweekly meeting Schedule

__anynomous__ : Regarding this topic, you mean to discuss if the scheduled times are still convenient for others or if we should change times?


__cekickafa__ : well, as phyro said before, if someone want to engage to meetings, can request,propose a time. Else, schedule looks fine.

__anynomous__ : I know that for the CC members these times are convenient. One of us prefers the 10:00 UTC time, for the other members, both times work out. One of the difficulties is that if community members would not find these times convenient, we would not find out easily, because they wont be here to discuss it.Let me ask for everyone present here. Do the current times 10:00 and 15:00 UTC work for you?

__dtavarez__ : I prefer this time.I am  OK with this time.

__cekickafa__ : i am OK also

__anynomous__ : Same here

__defistaker__ : Same

__anynomous__ : @phyro @deeev Do the current meeting times, 10:00 and 15:00 UTC work for you?

👍  phyro, deeev 

__deeev__ : Perfect.

__dtavarez__ : My suggestion is to set all the meetings at the same time (this time), and we let one day open for change. 

👍   cekickafa, defistaker 

__deeev__ : just wondering for people in the US, would be tricky.

anynomous 👍 

__anynomous__ : Perfect. In that case I think we should take a passive approach, if anyone has a problem with these times or want to discuss a topic at another time, they are welcome to suggest so. But without specific notice we keep these times.

👍   cekickafa, defistaker, phyro ,dtavarez, deeev.


##  2)   Bounty for writing a CFFI wrapper of secp256k1-zkp fork. (https://forum.grin.mw/requesting-help-with-writing-a-cffi-wrapper-of-our-secp256k1-zkp-fork/10024 )

__anynomous__ :  I discussed this with @dtavarez . I find it hard to estimate, but for now we got to an estimate of 10-20k in euro as bounty for the wrapper. Conditions are, open source (Apache or MIT), well documented and sufficient test cases for the wrapper.
@renzokuken propose making the bounty extendible. For that reason we thought 10k as a basis might be enough, extending to 20k if it can with sufficient argumentation be shown that additional time and work was needed.
☝️ Just a rough estimate, so feedback is welcome, especially from developers.

__phyro__ : https://github.com/rustyrussell/secp256k1-py

dtavarez 👍

__renzokuken__ : Thank you. I have some remarks: 1. It has to be MIT licence because the wrapped library is under MIT. 2. I think 10K EUR is quite a lot given then I just need someone to find how to run the build with missing methods and I will handle the rest of the work (wrapping them, making into a module etc)

dtavarez 👍

> phyro: https://github.com/rustyrussell/secp256k1-py

In the read me of my repo there is same link as an example, I used it as template while working on it.

phyro 👍

__dtavarez__ :
>phyro: https://github.com/rustyrussell/secp256k1-py

maybe that can be forked.

__renzokuken__ :

>__dtavarez__ : maybe that can be forked.

This does not have zkp methods, no commitments, no range proofs etc, just basic secp256k1

__deeev__ : Lets have as base currency $. Euro will likely continue to go down. 
However, i'd say we start with 3k$ for any significant progress. And we let renzo judge if the work provided is enough for him.

renzokuken, dtavrez,anonymous, cekickafa 👍

__renzokuken__ :  Yes I think $3K is reasonable.

__anynomous__ :  Sounds good to me. If no one takes the bait, we can always reconsider and go up with our bounty.

__deeev__ : I dont much like bounty itself and to lock it for a single person.

__anynomous__ : I can imagine thought, that someone who takes the  bounty also would like an estimate of the complete finished wrapper, how much? 6k?
I think locking itself is not a problem, as long as we put a deadline on the lock. E.g. show significant progress within 3 months.
Again, just my estimate, so feedback is welcome.

__renzokuken__ : I think once it builds making it into a wrapper is quite simple. But preparing some examples and docs could take a while

anonymous 💯

__anynomous__ : I think documentation and testing takes most of the time actually.

__renzokuken__ : Agreed.

__anynomous__ :  Ok, everyone agrees, thumbs up for 3k for some real progress, total bounty is still hanging though, 5k?

__dtavarez__ :  let's do not underestimate the repo is quite big *[Graphic](keybase://chat/grincoin#general/53946 ) 

__defistaker__ : I think 3k-10k is generous, it should attract developers.

__dtavarez__ : 25k lines of code is not a joke.

__anynomous__ : Ok, I think 10k is manageable considering its worth.
So 3k for showing significant progress, 10k $ total.

defistaker 👍

__dtavarez__ : 3k to 10k sounds good to me.

__anynomous__ :

>__dtavarez__ : 25k lines of code is not a joke.

True, but most of that is C, so not actually added work.

__renzokuken__ : 

>__dtavarez__ :  let's do not underestimate the repo is quite big *[Graphic](keybase://chat/grincoin#general/53946 ) 

Which repo is it?

__deeev__ : Libsecp zkp

__anynomous__ :  I think the non C code is about 10%, so 3000 lines of code and documentation.

__dtavarez__ :

>__renzokuken__ : Which repo is it?

https://github.com/mimblewimble/secp256k1-zkp

__renzokuken__ : 

>__anynomous__ : True, but most of that is C, so not actually added work.

Yes and CFFI lib handles most of the work, this bounty is a clever copy paste for someone who knows how to compile C code.

anynomous 👍

I think if someone knows how to handle header files and knows which files to exclude and what definitions to copy from secp256k1-py this bounty is super trivial.

__anynomous__ : Ok, lets vote. Everyone in favor of 3000$ for significant progress, 10.000$  total bounty.Requirements, MIT licence with good taste cases and documentation.

__renzokuken__ : Just for me it’s a trial and error as I have no experience with that

__deeev__ : However, if a person interested by this work want more. We could increase. What I like to do in these case would be just say to renzo, judge the work and reward accordingly. The cc can say we give a range of 3-5k.

renzokuken, dtavarez 👍

__phyro__ : it's possible that once we upgrade our libsecp fork someone will have to upgrade this.

renzokuken 👍

__deeev__ :

>__phyro__ : it's possible that once we upgrade our libsecp fork someone will have to upgrade this.

True.

__anynomous__ : Probably that would mean minimal changes though, only the C under the hood should change right? We should have access to the original repo though.

__phyro__ : and when we upgrade, perhaps the linked py ffi would almost match and could be used completely and be extended. Idk really, just something to keep in mind.

renzokuken 👍

__renzokuken__ : If that situation occurs I will 1. Try to make new build with update repo 2. If fails automatically I would try to fix myself 3. If that fails I would ask for help again.

deeev 👍

__dtavarez__ :

>__renzokuken__ : If that situation occurs I will 1. Try to make new build with update repo 2. If fails automatically I would try to fix myself 3. If that fails I would ask for help again.


could you transfer the repo to grincc? we could  give you write permissions.

__renzokuken__ : Of course.I will remove donation information from the readme first.

dtavarez, deeev 👍

Noticed php and js cffi wrappers work similar to Python so maybe deps.c file could help us kill 3 birds with one stone.

__dtavarez__ : can we move to the next topic: 

deeev, anonymous, cekickafa, renzokuken 👍

##  3) Retroactive Grants like idea (https://blog.opengsn.org/taking-retroactive-grants-from-concept-to-practice-at-gitcoin-grants-round-11-649497d08519)

__dtavarez__ : Retroactive grants in summary;

I would like to suggest Retroactive Grants. People can nominate themselves or dominate another person on the basis of contributions made.
I do not have the process clear yet but that is the basic concept. The objective is to recognize the impact that the contributions from community members have made on the Grin ecosystem.
one quick example could be @nicolasflamel1 and the hardware wallet implementation, if the code can be reviewed, audited and improved  I do not see why not to donate or @renzokuken with grinventions would be another example
I have more examples in my mind, but that the idea, if we agree that it could be something objectively good for Grin we could come up with a formal proposal.

__deeev__ : I'm all for it.

__defistaker__ : I support this suggestion.

__renzokuken__ :  The community council could go through community nominations, review what was done and attribute a prize.

__dtavarez__ : correct.

__cekickafa__ : Thats a good idea.

__dtavarez__ : i know,right.

__deeev__ : Actually for nicolas flamel, i dont see the need of retroactive grant needed since there's already a bounty on this.

__renzokuken__ :  Non-technical people could also be nominated. For blogging, making videos, organizing events etc.

__deeev__ : 

>__renzokuken__ :  Non-technical people could also be nominated. For blogging, making videos, organizing events etc.

I quite like that as well.

__anynomous__ : I think the idea has merit, not sure about the details yet. In general, if everyone thinks someone deserves a bounty retroactively, it should be no problem.

__dtavarez__ : 

>__deeev__ : Actually for nicolas flamel, i dont see the need of retroactive grant needed since there's already a bounty on this.

yep but he should go through the constrains though to get the bounty.

__deeev__ :   Even if its still 20$ for a video. That may still be highly appreciated from the maker.

__anynomous__ : Only problem I have is that I think we should not create expectation that everything will get paid. Volunteer work should be there.

dtavarez 👍

__renzokuken__ : 

>__deeev__ :   Even if its still 20$ for a video. That may still be highly appreciated from the maker.

Many YouTubers don’t even get that.

__deeev__ : Based on contribution and community willing. I agree that contribution should always be rewarded.

__renzokuken__ : Even a single tweet could be rewarded if makes an impact.

__deeev__ : 

>__dtavarez__ : yep but he should go through the constrains though to get the bounty.

Which constraint?

__dtavarez__ : 

>__deeev__ : Which constraint?

https://forum.grin.mw/t/locked-support-ledger-wallet/8517

__deeev__ : 

>__renzokuken__ : Even a single tweet could be rewarded if makes an impact.

Community willing. What i like to do usually is to reward someone that did something and did not asked anything in return.


renzokuken 👍

__renzokuken__ : I remember when I joined in I used to bitch a lot about website, I didn’t realize I could PR to repo to suggest changes and now such people could be rewarded for making an initiative.

__anynomous__ : Mmm. I am divided. I like incentives, but I hate creating expectations.

__celickafa__ : Grin itself is an expectation somehow :)

__renzokuken__ :  We could steal the review process from other organization ;)

__deeev__ : 

>__anynomous__ : Mmm. I am divided. I like incentives, but I hate creating expectations.

That's why. I'm saying just reward people when they did something and asked nothing in return. Just like a gift.

__dtavarez__ : but it is still retroactive and proposed by the community members themselves.

__phyro__ : we have very few people contributing for free today (actually, it's increasing now). I'd try to get as many contribute for free without expectations or hopes they may get something.

deeev, anonymous 👍

__dtavarez__ : if the community understand someone is adding value should be taken into consideration.

__renzokuken__ :  This also resolves the problem of estimating how much a challenge is worth. Hard to predict the efforts needed but post-factum everything is clear.

__dtavarez__ :

>__phyro__ : we have very few people contributing for free today (actually, it's increasing now). I'd try to get as many contribute for free without expectations or hopes they may get something.

yes, and I do understand that I do not disagree but what we could do is to be open to support contributors.

__phyro__ : contributors with a good record gain community trust and are more likely to get their next request approved.

deeev, anynomous 👍

Also explaining why B got it and not A and C might make A and C feel bad about their contributions
in the sense that the community does not appreciate their effort enough.

__anynomous__ : I think these free 'bonusses' are ok. But only for small amounts. For larger contributions, why not let people create a Funding Request (I know it creates a hurdle), but they could always say, please pay me afterward what you think it is worth.

__dtavarez__ : I think we all agree on that the lack of man-power is no good for grin, right?

__deeev__ : Agree on that.

phyro 👍

__anynomous__ : I think we all agree on that, the danger is really that incentivising one as a suprise might feel like a disincentivize to another, the examples @phyro gave.

__dtavarez__ : True.

__cekickafa__ : if different approach will bring man power, better worth a try.

__deeev__ : But giving grant does not mean we'll have more contributors. We re lucky on the fact that someone gave 100 btc. But those are limited and we should be careful to not be so generous at the same time.

__phyro__ : it's a bit of a social problem really. I think good contributors will come because they like the tech, just like everyone else before them that came :)

__anynomous__ : Hence, I think this idea is fine, but we should limit it, only fun bonusses, but then again that is rather close the bounty system we have, people can justs propose to add their work as small bounty.

__deeev__ : If we start by granting people and we'll not have more funding on the future, we could count only on contributors.

__anynomous__ : How about we agree to keep it only small amounts, so pocket money? Anything large would be an exception, funding request or a request to create an additional bounty.

👍 deeev

__deeev__ :  Lets stimulate community members while at the same time endorsing the spirit of free decentralised work out of the love for the project.

__phyro__ : this too orders contributions by importance.

__anynomous__ : @phyro so what is your final verdict/opinion, just not do it and keep the current system?

__dtavarez__ : I would like to give it more thought based on the feedback received. if you don't mind and move the conversation to the forum.

👍 deeev

__phyro__ : 

>__anynomous__ : @phyro so what is your final verdict/opinion, just not do it and keep the current system?

idk, I don't really want to influence the decision.

__dtavarez__ : is that OK?

>__phyro__ : idk, I don't really want to influence the decision.

all opinions influence the decision.

__anynomous__ : Same here, I need to think this through more as well. I think it would require some forum discussion. In general I like that reputation of doing work for free just give you trust, hence more easy to create a funding request or request a bounty. But again, we need more feedback on this.

__deeev__ : Let's move that conv to the forum.

👍 dtavarez

__anynomous__ : And all opinions are welcome, we all are just community members here, council members of one council or another are no exception, they just collect opinions and cast their final votes accordingly for proposals but they are free to express their opinions.

__cekickafa__ : Forum or keybase, it should be discussed more broader than a meeting time. It is important and vital for Grin future.

__dtavarez__ : I will open a forum post. I think there are valid points here.

👍 cekickafa, anynomous.

__anynomous__ : Ok, that is the descission for today, I think it is clear that there are ups and downs and that more feedback is needed.
So that is it for today, that wraps up the meeting?
Anything else that needs to be discussed or added to the next meetings agenda?

__dtavarez__ : that's for today. 3 topics in 1 hour, record time!


## *Action points*

* Community meeting schedule stays same.
* Bounty for writing a CFFI wrapper of secp256k1-zkp fork idea accepted.
* Retroactive Grants like idea will be discussed more.


**Meeting adjourned.**