# Council Meeting Notes May 10, 2022

Community Council (CC) meeting held @ 10 UTC in grincoin#general channel on Keybase. Meeting lasted 65  min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendence:_

* anynomous
* yeastplume
* cekickafa
* defistaker
* phyro
* dtavarez
* vegycslol
<br/>

# Short Summary

-  Current situation of PIBD has been discussed. __yeastplume__ will work on RFC.
-  Grin meet-up ideas/details has been discussed like location/date.
-  Grin-wallet contract prototype can be tested by community
-  Grin CC's last year performance has been reviewed and future projections has been made. 

<br/>

# Agenda Points & Actions

<br/>

* Last meeting notes here: https://github.com/grincc/agenda/tree/main/notes

* Current meeting [agenda](https://github.com/grincc/agenda/issues/55)

  1) Open discussions.
  2) Discuss the outcome of a CC reflection on the past year and brainstorm on future direction of the CC.
  
  
 
## 1) Open discussions
<br/>

__anynomous__ : First, an open discussion. Is there anything we need to discuss, share. @yeastplume any updates on the development?
     


__yeastplume__ :  Sure, from my perspective PIBD (testnet only) is progressed enough for review and merge into the main code. From there I'd like to create a (hopefully) smallish RFC to describe the sync process. Only problem is the number of hands we have on deck capable of review at the moment
While that's going on, I'm working on a number of smaller activities to assist with network health and tooling, I want to have a seed health tracker and a means to repopulate archive nodes for anyone who wants to run one. I'm also going through the list of seeds and will be revising it.

__anynomous__ : I can imagine. When do you expect a smallish RFC to be ready? Maybe in last quarter (or is that to optimistic) @dtavarez can start testing implementation of PIBD in Grin++. Preferably the whole network will support PIBD in the near future.

__yeastplume__ : Also thinking about a testnet explorer. (Also need to review mixnet code).. so plenty of things on the list.. once I'm through all that I hope to start turning attention to a core gui-like experience and to phyro's improved transaction building, but that's a few months off.

👍 (dtavarez)

RFC shouldn't be a big deal it's more documenting what's there and tweaking based on feedback, within the next few weeks I hope.

__dtavarez__ : For PIBD and Grin++ I would like a RFC.

__yeastplume__ : that's why I'm going to write an RFC.

__anynomous__ :  Sounds like you have enough on your plate @yeastplume. When you review, please also look at how well the documentation and the maintainability of the code is.

__yeastplume__ : Although most of the details are in the existing RFC, a second one will just describe the sync process.

__dtavarez__ :   Having PIBD working on the Rust implementation should more and enough for me to make the changes on Grin++.

👍 (yeastplume)

__anynomous__ : Yes, example code plus RFC should work.

__dtavarez__ :  Yes,
most of the issues reported by grin++ users regarding the sync process seems to be fixed on v1.2.7 that was something that it was needed from my pov.

__anynomous__ : Ok, that is good. what was the main problem in retroperspective?

__yeastplume__ :  yeah, the txhashset method needs to phased out for many reasons.

👍 (anynomous)

__anynomous__ :  With the txhashset , you mean sharing them as zip?

__yeastplume__ : Yes

👍 (anynomous)

__dtavarez__ : @yeastplume I am more than happy also to deploy the latest version on at least 25 public nodes whenever you need it or if you need I could  run few of them on testnet just let me know.

__phyro__ :  does zipping mmrs take a lock by any chance? I think some people had issues with node being unresponsive to the api calls, but i'm not sure what would cause that.

__yeastplume__ : definitely testnet only for a while, I think we have enough out there on testnet to test it (look for a capabilities flag 93 (or around there, don't remember exactly)
it takes a read lock, yes... the code is very lock-happy. responding to PIBD blocks also takes a read lock but it's only for a relatively small amount of data at a time

👍 (phyro)

__dtavarez__ : ok I will use at least 5 of nodes and deploy the latest alpha release.


__yeastplume__ : that would be great, thanks! I'll also be getting a public testnet seed up soon that will have pibd included

👍 (dtavarez)

__anynomous__ : Great. Did anyone have time to play with the Grin wallet contract prototype?
https://forum.grin.mw/t/grin-wallet-contract-prototype/9745

__yeastplume__ : I did :D I think it's an excellent way forward, particularly if all multi-party concerns can be worked out with it.

__anynomous__ : What is the --num-participants=XXX is for? So you can do some sort of CoinJoin? @phyro
I mean the self spend part is already nice, just wondering.

__phyro__ :  at the moment it supports only 1 or 2 because of the concerns shared in the safe-slates gist. It needs to know when it can finalize the transaction and this is done when everyone contributed their keys and partial sigs, but to know this, you need to know how many participants you have
hence, when making a self-spend, you need to tell explicitly you have a single party involved in a transaction

__anynomous__ :  A ok. But when enabling more than 2, there is a problem. Not sure what you mean with "safe-slate gist"

__phyro__ : https://gist.github.com/phyro/cc0265cfc27d0405eefe63c490048265

__anynomous__ : Thx. Will read up later.

__phyro__ : there's a "problem" described there. How much of a problem it really is is debatable (there's a bunch of comments with tromp)
but solving also for this would be a bit much to begin, so I simplified to 2 parties


__anynomous__ : Sure, makes sense.
Are there any other developments we need to share/discuss?, otherwise I propose we move to the second agenda item.

__phyro__ :  if someone else finds time or wants to test things, I suggest we do that (I'm not sure anyone checked the testnet exchange flows and gave any feedback on this)
it's imo important to take some time and give feedback to people to encourage further contributions otherwise we can easily get even those that contribute demotivated

👍 (cekickafa, johndavies)

__anynomous__ : I think we need some more time for that. At least, I had it planned but did not get to it yet.

__phyro__ : it's no rush, we all have other things to do, just something to keep in mind for whatever it is we are building

👍 (anynomous, dtavarez)


__anynomous__ : Regarding our second agenda item:

 ##  2) Discuss the outcome of a CC reflection on the past year and brainstorm on future direction of the CC

                     
__anynomous__ : @dtavarez Do you mind if I share the link to the notes, or you prefer copy paste?

__dtavarez__ : go ahead.

__anynomous__ :  https://cloud.punksec.de/index.php/s/9Rc2Bpr7qi2rTyG

So in summary, we had a meeting to Reflect on the CC's work so far and to brainstorm where we wanted to put our energy and focus on in the coming year.
 It was just a nice informal chat to catch up, always good to have some face to face time with other grinner,  these notes summarize our reflections.

All of us felt and wanted to do more, but life happened, we also needed to keep up our daily life and work.
I think the last part, The plan is most interesting:

  - Be more proactive.

- Move the audit of the atomic swap forward, create a bounty for reviewing and deployment.

- Have both small or big meetup events, October or end of the year. E.g. Berlin, Amsterdam, Zurich.

- Focus on having well documented building blocks to work with in the ecosystem, e.g. how to run a mining pool, how to interact with wallets via their API. How to setup a mining pool. We need both documentation and video content for all these which we can link to on GrinHub and the GrinCC website.

- Be easier going on spending micro funds on documentation and video documentation as small incentives.

- Web-wallet, browser extension to have something like MetaMask wallet or My Ether Wallet. GUI rust wallet.

- Maybe move to having one groundkeeper in the future for note keeping and outreach.

- Deploy CoinSwap.


__yeastplume__ : Definitely think a meetup event would be good

👍 (anynomous, dtavarez, phyro, cekickafa)

__anynomous__ : Personally we felt it would be great to have physical meetups again. All of us get more motivated when chatting face to face, especially when enjoying a beer with our crypto talks. It is also the best way to connect to other crypto enthusiasts. I mean social media is fun, but those who really care often go to meetups.


__phyro__ :  I agree, in person meetups are good and a great way to build trust among each other

__anynomous__ : Also, I think we kind of failed at some smaller tasks because we were to formal about spending micro funds.
E.g., should we really discuss and vote to spend 100 Grin on a meme contest or on some video bounties..? We will try to be a bit more easy going and flexible to get things done.

👍 (cekickafa)

__phyro__ : which usually also means less conflicts

👍 (dtavarez, yeastplume, cekickafa, defistaker)

__anynomous__ : My question to you, are there things that you think we missed out on, things to improve, something we should put our energy on in the future?

__dtavarez__ : there is an ice cream shop available in berlin for us to have a meetup at any moment; and also the house of satoshi in zurich, but for now most people gathering there are german speaker fyi. Best ice cream in berlin btw

__anynomous__ : Also the organizers of Bitcoin Wednesday, a monthly meetup in Amsterdam indicated they are willing to help organize an event.
But I have to apologize, I have to go now.
Thx for a great meeting! @dtavarez you can take over👋

👍 (cekickafa, defistaker, phyro)

__dtavarez__ :  Like @anynomous said the CC is open to feedback so feel free of sharing your thoughts
could be now or later is ok

__phyro__ : I'm good with the suggestions. I only want it to not be in a country where the expenses are very high so that those that really want can afford to attend.

__dtavarez__ : berlin is cheap and well connected.

👍  (phyro)

right now I'm not sure I can organize anything, I already have a huge list of things to do, but if anyone has experience in this and is willing to help, please let me know.
I'm incline to something simple that be replicated in other cities.

👍  (cekickafa, yeastplume)

__defistaker__ : Would it be a one day event?

__dtavarez__ :  could be, one afternoon where people could hangout, drink something, eat, and chat; and we could have small 5 to 8 minutes talks related to grin, privacy and crypto
nothing fancy

__yeastplume__ : could definitely be done via a meetup group

__dtavarez__ : yes

__defistaker__ : I would love to attend but travel cost will be very high for a single day event for me.

__yeastplume__ : but not tied to a particular city.

__dtavarez__ : Correct.

__cekickafa__ : i am planning to host at Turkiye for a few day or a week in the future.. Workshop near beach and sun. You swim and code with laptops : A nice scene for promotion, can make a viral video😂

__dtavarez__ : it would be nice to have a model or framework for the meetup

>cekickafa: i am planning to host at Turkiye for a few day or a week in the future.. Workshop near beach and sun. You swim and code with laptops : A nice scene for promotion, can make a viral video

beach? sun? I like that!

__cekickafa__ : yes, i will record you all with shorts😎

__dtavarez__ : sure :)

__phyro__ : 
> defistaker: I would love to attend but travel cost will be very high for a single day event for me

I'm not sure we'll be able to do a multi-day event. It's usually much harder to organize (although I have no experience with this tbh) and we have a relatively small community right now

__defistaker__ : i see

__phyro__ : 
> defistaker: i see

the cost problem you mention is real though, it's why I mentioned it would be best to not be in the most expensive city/country.

__defistaker__ : Yeah, travel costs for me would be more than 1000Euro.

__phyro__ : I think we'll have no chance but to try something small and adjust over time as we learn. might be interesting finding out who would even be willing to come and for what cost

__dtavarez__ : schengen area is fairly affordable, but that's why I think it would be perfect if we could have a model for the meetups so anyone could run a grin meetup.

👍  (cekickafa, phyro)

The trick inside the eu is to avoid the main airports of the big cities.


__dtavarez__ :  so, I think this covers our relaxing agenda of today, let's think about model for a meetup that could be replicated everywhere
thank you for your time 👋

Thanks 👋 (cekickafa, defistaker, yeastplume, )



 ## *Action points*
 - PIBD testing and RFC
 - Spend micro funds on documentation and video documentation as small incentives.
 - Explore ideas (date/city location ) for Grin meet-up.
 - Attend  Bitcoin Wednesday, a monthly meetup in Amsterdam.



**Meeting adjourned.**




















