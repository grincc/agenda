

# Community Meeting Notes August 29, 2023

Community Council (CC) meeting held @ 10:00 UTC in grincoin#general channel on Keybase. Meeting lasted 45  min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_

* future3000
* aglkm
* ardocrat
* anonymous
* cekickafa




# Short Summary
 
- Open discussion about;
 -  GrinCC elections, CC mining farm equipment
 - Grin Api. 
 - Grin++ Api + Cli.
# Agenda Points & Actions
 

* Last meeting notes here: https://github.com/grincc/agenda/tree/main/notes

* Current meeting [agenda](https://github.com/grincc/agenda/issues/101)







__anonymous__ : No agenda, everyone is welcome for a 🍵 and informal chat!

https://github.com/grincc/agenda/issues/101






__cekickafa__ : So we have 3 candidates for election so far ?


__anynomous__ : Yep, not to bad if you ask me. Especially since there might be more coming still.


__future3000__ : 👋

👋 anonymous, cekickafa




__anynomous__ : I will copy from Telegram public CC channel:

Update: So far we have three candidate posts, more might follow:
- Danila: https://forum.grin.mw/t/anouncement-grin-community-council-election-call-for-candidates/10693/7
- trab: https://forum.grin.mw/t/community-council-candidate-trab/10704/7
- triniton: https://forum.grin.mw/t/community-council-candidacy-trinitron/10697/7

Candidates who want to be in the newsletter should make their candidacy post at 7th of September at the latest. The 8th of September the official election voting time starts, but in the mean time as candidate you can already collect likes / votes
https://t.me/grin_CC_public/77

👍 cekickafa, future3ooo

__cekickafa__ : That is good anyway. 3 of them, known members in community.
I was expecting more than 5 :)

__anynomous__ :
Exactly, each of them  is interesting as a candidate in their own way. Danila is admin on Grin++ support channel, trab and Trinitron are long term community members with reasonable understanding of the tech.
Would be nice if @dburkett still volunteers as candidate, but I understand if he has to little time
Well, you can become the 4th candidate 😉

__cekickafa__ : Duty calls :)

__future3ooo__ : We really need to promote the election abit more.


__anynomous__ : But be warned, it easily eats through your energy as happened with David T.
Yes, did we already have it in the newsletter?
I think so right.

__cekickafa__ : 4-5 days within newsletter will be published. I will put it.

👍 anonymous

Community mostly on forum, if we promote it on social channels, will it be useful? i have no idea. Since eligible members we need.

__anynomous__ : By the way, did any of you ever looked into learning Rust?
I just started with the Rust book.... and I finally start to see why Rust is the #1 most popular programming language for multiple years and why it has a growth rate of 225% on a year on year basis. It takes some getting used to, but Rust really has your back on preventing mistakes and creating orderly projects.

👍 ardocrat

__future3ooo__ : Thinking to run a community contest for the best bill board design prompting a candidate. The winner gets rewarded a certain about of Grin pixels once payments go live here:  __www.grinpunk.com__

👍 anonymous, cekickafa 🔥  ardocrat 

__anynomous__ : Cool stuff!

__cekickafa__ : Gotta mention grinpunk  on newsletter again.

__anynomous__ : Wait till it is live, if will have the biggest impact.
Or maybe building up anticipation is also good 🤔

__cekickafa__ : Ok. Mentioned at previous one anyway.

__future3ooo__ : 

>__anynomous__ : Wait till it is live, if will have the biggest impact.

The biggest hype usually comes before launch 😂

👍 anonymous, ardocrat

__anynomous__ : @future3000 It is not out of your league, but indeed it does take some getting used to. I come from Python and R, which are completely different in style and thinking.
I am not a great programmer, so I think Rust can be for anyone. Also googgle tried it out with their employees, and apperently it is not harder to learn than other languages after a 6 month test.
It is just not an easy language if you never red a book about it IMO, at least I had a hard time grasping the grin node and wallet code when I looked before starting to read the Rust book.

👍 future3ooo

__future3ooo__ : Google employees are probably pretty elite in general though 😁

__anynomous__ : Maybe they are a bit above average. But I am not, when it comes to coding at least.
@yeastplume any updates on development?
I think it is till early morning for him, but asking does not hurt.

__future3ooo__ : Is Grin wallet API working ?

__anynomous__ : I guess that means he did not have his morning ☕ yet, 😁
grind node, or grin++?
I have not tried yet to be hones, but they both work as far as I know. I need to check if David already merged the code h in his latest release and whether it is only for the client node or also Grin++ GUI version.
These are typically the things I do not have time for, but which should be checked for proper feedback between development and governance.

__future3ooo__ : grin_wallet

__anynomous__ : Yes, the API works for that one. I remember in the past some users complained that at times it needed restarting, but I think that issue was solved in the latest release, at least in 5.2 (many improvements to stability, I never needed to restart).
EDITED
Only according to David it is a hassle to setup the connection with the owner API, it is very secure though which is also really important..
https://docs.grin.mw/wiki/api/node-api/
https://docs.grin.mw/wiki/api/wallet-api/
If you want to use it and have problems with he documentation, you can always ask David. He played a lot with it since he unified the Grin++ API with the grin rust node and wallet api. Only the way you connect to them is slightly different (harder but more secure with grin-wallet)


__cekickafa__ : Does Grin++ has CLI now ?

__anynomous__ : It does, but I think it is release as alpha or beta, so not as main yet since David still has concerns about the security.

👍 cekickafa

__future3ooo__ : I think there’s still this issue here : https://github.com/mimblewimble/grin-wallet/issues/635

__anynomous__ : Grin++ client version, is marked as not secure though
https://github.com/GrinPlusPlus/GrinPP-CLI/pull/7


__cekickafa__ :

>__future3ooo__ : I think there’s still this issue here : https://github.com/mimblewimble/grin-wallet/issues/635

invoice flow broken ?

__anynomous__ : In the same thread they post a link to a version that provides a hot fix

https://github.com/pkariz/grin-wallet/tree/fix/invoice-issues , but I do not think it has been solved in the main branch. You can ask @yeastplume. Best to ask him in a DM, he normally answers pretty fast, at least in my experience. Tagging him in the channel works less well.

__ardocrat__ : 

>__anynomous__ : By the way, did any of you ever looked into learning Rust?

That's nice to hear, come from theory to practice, all you need to understand is borrowing-ownership system and lifetime for sure :)

👍 anonymous, syntakjax



__anynomous__ : Lol. Yes, exactly that. First glance Rust looks annoying since getting simple code running often leads to errors, but you soon appreciate Rust catching and explaining them and helping you to avoid major issues down the line.


__aglkm__ : Hey all 👋

I suggest adding a permanent topic "track community grin miners issue" into the agenda. So we have any updates on the meetings about the situation.

 😁ardocrat


__anynomous__ : No need to have it as a topic, but we can ask. @future3000 did the guy from the mining farm reply yet on your proposal to renegotiate a deal that is more balance and favourable to them?

__future3ooo__ : Not yet. But I’ve only recently messaged him about the 50-50 split part. Will let everyone know his response in the CC telegram group
Re connecting up and testing. The other guy from the farm messaged me back after the last CC meeting saying he wanted to setup a time for last week. I said yeah sounds good, but then didn’t get a response. I sent him a follow up message earlier today.

👍 anonymous

__anynomous__ : That is all we can do.


__cekickafa__ : Maybe dtavarez better ping them also, since he knows the facility and persons.
@future3000 efforts are limited in this case, thats is all he can do.


__ardocrat__ : 

>__anynomous__ :  Lol. Yes, exactly that. First glance Rust looks annoying since getting simple code running often leads to errors, but you soon appreciate Rust catching and explaining them and helping you to avoid major issues down the line.

Learning By Doing approach works here 100%

👍 anonymous

__future3ooo__ : Also re the miners. I can get around 0.11 USD per KW. So a last resort option could be me hosting them 😅 really don’t need that admin or noise in my life, but it’s possible. I have the space in my garage and have run larger mining setups before.

__cekickafa__ : That is a better option.
Completely better than unknown custody. We cant predict the future if Grin gets mainstream.

__anynomous__ : Mmm, not sure. I think it would be like you taking 😅 🔫 
It probably would eat up your time and energy like it did for @dtavarez. IMO it is better to accept the loss, or the risk of losing it than further taking blame for something that was a community decision to begin with.

__ardocrat__ :  And one Cow :) https://doc.rust-lang.org/std/borrow/enum.Cow.html
OK, last meme for today

__cekickafa__ : 

>__anynomous__ : Mmm, not sure. I think it would be like you taking

i would. If only there were no custom tax %300🤐

__anynomous__ : That is another big bottleneck. Lets say we would spend 20-30% of the value of the miners in costs to ship them and try to set it up somewhere else with an electricity rate which is certainly higher than at the current location....it just does not make sense to me. So I see it as an investment that is possible lost or losing, but we just have to accept it and try to stick to our plan as best as we can.


__cekickafa__ : i agree, it is mostly a lost.


__anynomous__ : If I am very self critical, we already lost since most miners return their investments in the first months, which are already past.
So if we can get anything out of it still, some passive Grin flow, that would be like a bonus.

👍 cekickafa


__ardocrat__ : 

>__anynomous__ : If I am very self critical, we already lost since most miners return their investments in the first months, which are already past.
So if we can get anything out of it still, some passive Grin flow, that would be like a bonus.

Yeah, we have no trusted company like Blockstream for Grin to host miners, so situation is understandable

__anynomous__ : Exactly, that was our problem to begin with. So in retrospect, buying so many miners (more than individual community members could manage), was a mistake. But then again, no one could foresee we would get a war, bringing up electricity prices in many locations making profitable mining so dam difficult.
In behind sight it is always easy to make the right decisions 😛

__ardocrat__ : Epidemic, war, next cataclysm, so we can lose them on this island for real.

💯 anonymous


__anynomous__ : The only certainty in life is that everything is uncertain.

👍 cekickafa, ardocrat

__cekickafa__ : So you say Grin is an experiment, so this stuff. Case is clear. Bonus is welcome if we receive.


__future3ooo__ : 

>__anynomous__ : If I am very self critical, we already lost since most miners return their investments in the first months, which are already past.

That’s not necessarily true in this case. Usually miners get their largest returns early on because more efficient hardware is introduced or the number of network miners grow and eat away at profits. Neither of those are true in this case, as far as we know now.


👍 aglkm


__aglkm__ : Grin hashrate is decreasing, and grin mining is profitable again.

__anynomous__ : It depends, if Ipollo introduces a new generation or batch of miners in this upcoming bullrunn, there will be little return of investment. If they do not, existing miners would make a good profit.

I do know a fair amount of miners have crashed and burned (including my own unfortunately). So there are less miners operational than sold.

__cekickafa__ : There were worth of 25kgps miners sold by ipollo.

👍 anonymous

__anynomous__ : In case, our bets are made, we can only see.

>__cekickafa__ : There were worth of 25kgps miners sold by ipollo.

Not that many have crashed and burned, so that should mean there are a lot of miners on standby.

__ardocrat__ : 

>__aglkm__ : Grin hashrate is decreasing, and grin mining is profitable again.


Its jumping +-50%, average monthly hash is ~7KGps

>__anynomous__ : It depends, if Ipollo introduces a new generation or batch of miners in this upcoming bullrunn, there will be little return of investment. If they do not, existing miners would make a good profit.

Maybe Bitmain will introduce miner for Grin as they made with Monero, so they should pump it for better liquidity 😂





 
## *TO DO List*

* Re announcement of Grincc Election on newsletter.





**Meeting adjourned.**



