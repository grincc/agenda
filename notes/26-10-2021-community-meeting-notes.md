 # Council Meeting Notes October 26, 2021

Community Council (CC) meeting held @ 11 UTC in grincoin#general channel on Keybase. Meeting lasted 40 min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

<br/>

### _Community attendance:_

* __anynomous__ 
* __future3000__
* __mark_hollis__
* __dtavarez__
* __vegycslol__
* __cekickafa__
* __defistaker__
* __yeastplume__
* __phyro__


<br/>



# Short Summary

- Reflection of 40 weeks. GRiN Community Council
- Scilio-Coinswap. Forum update.
- exchange listing and support. Technical discussion


<br/> 

# Voting Results 

<br/>
no votes held

<br/>

# Agenda Points & Actions

* Last meeting notes [here](https://github.com/grincc/agenda)
* Current meeting [agenda](https://github.com/grincc/agenda/issues/20)


<br/>

##	1) Agenda 

* __anynomous__ : So today's, agenda is basically blank.We have space for updates from @scilio and @mark_hollis. And we can discuss anything else as well. Like what there should be on the agenda in upcoming meetings.

* __defistaker__ : @scilio posted in forum (https://forum.grin.mw/t/request-for-funding-scilio-coinswap-implementation/9149/)
He mentioned that he is working and made good progress

* __anynomous__ : Great, and he chose rust, which is in general a good choice.

* __cekickafa__ : Glad we have atomic swap ,nano ledger ,Grin++ Mobile and Coinswap!

* __anynomous__ : So looks like everything is progressing nicely. It looks like Rust is still the main language in this project, which is in a way great, since it is a secure language.

* __defistaker__ : Rust is the most loved language by developers in stackoverflow surveys

* __anynomous__ : Rust has great potential, it is a bit like Grin itself in nature. It has not caught up yet with the larger existing projects/programming languages, but its design decisions will dictate it is there to stay and grow for the long term.

* __cekickafa__ : Lots of things developing silently

* __anynomous__ : Exactly, I like it. things are best when they do not need to be over managed, they just keep on rolling.

## 2) Community Council Reflection

* __anynomous__ : Since there is nothing else on the agenda for today, I would like to ask to think a bit about what we have done so far in the past 40 weeks (20 Grin CC meetings).
Are we going in the right direction, do we need to do more as community and as community council?
Anything else we should be adding to future agendas, things we should organize, things we should discuss. Just trow in whatever comes to mind.

* __anynomous__ : Some things that came to my mind.
-> It is not my call to make. But I was thinking, it might be good to have quarterly Grin OC meeting. Just to organise and check we are going in the right direction, pay the bills, did everyone update their projects etc?
-> We should start organizing meetups again physically, luckily there is progress there. Both for a meetup in Berlin (Germany) , as well as some enthusiasts who would like to help organise a meetup in Amsterdam (Netherlands)
-> Maybe pick up video challenges with bounties in the coming months?

* __cekickafa__ : Those are very good ideas for Grin community. it can show that Grin is vivid and people can contribute more.

* __defistaker__ : I think we are building a foundation slowly, but firmly

* __anynomous__ : Glad to hear so 

* __cekickafa__ : well those councils always slow i think,no matter what in open projects naturally. Also I want to say that; Grin Community is still shrinking and getting centralized

* __anynomous__ : You mean the OC is slow, or just councils in general? I concur, I have been in many councils in my live, all where slow. The stakes are high, but the practical progress is slow, and that is fine since we do not want to make many mistakes, we want to have well founded decisions.

* __cekickafa__ : By community,pool and exchange- Yes it is normal pace I think. But its getting smaller or is it my concern? I meant Grin ecosystem.

* __anynomous__ : My experiences so far are that growth often happens in jumps. Like with the CC, a few major projects are initiate, wait 1/2-2 years, some major milestones are made, then new major steps can be made.

* __anynomous__ : So progress is often seemingly slow during most months, but the development continues in the background as we have seen with @scilio- But @cekickafa you think we should add discussion of mining pools to the agenda?

* __cekickafa__ : I think it won't help. Miners choose their own way.

* __anynomous__ : True, I only think we can make it easier, that's all. The rest is just natural selection.


## 3) Exchange Listing & Support
 
* __anynomous__ : I am curious how come you think "Grin community is still shrinking and getting centralized", because there are less members on this CC meeting, or other indicators?

* __cekickafa__ : Becuz we bow to a single exchange with pool. I find it unnatural after many things done since past years. I didn't mean GrinCC. Ecosystem. pools and exchanges

* __cekickafa__ : I mean before slatepack it was hard but ecosystem was bigger ,now tx are more comfortable but we shrink.it is unnatural
All big pools gone.

* __anynomous__ : We are also discussing it among CC members because we are concerned. There is however only so much we can do. The problem is that Gate.io chose for their own type of implementation of transactions using memo to link users to a transaction.
We can offer them an alternative way, using slatepacks, like grinmint uses. But we can only offer, if they do not want to implement it. If they do implement it, miners can use other pools like Grinmint to directly transfer there.
This is the main reason Chinese miners do not want to use grinmint as well as other pools, because they do not want an extra step between the pool and gate.io

* __yeastplume__ : Just sidetracking a bit on the subject, sorry, does anyone have a list in their heads of the major reasons so few exchanges are running Grin ATM? I know of quite few myself, but would be good to have this info down somewhere; thus far in this convo we have TOR and the need for exchanges to link identity to users, (our payment proofs aren't enough for that)

* __cekickafa__ : Memo link your identity. taint you.

* __yeastplume__ : yes, but like it or not, exchanges are running under ever-increasing regulatory requirements, they need to be able to link transactions to users even though Grin is designed to prevent exactly that

* __anyomous__ : That is one reason: The other is the need for interactivity, their regular infrastructure is not build for that. When using RSR, this should not be much of an issue though.
As long as a user uses an account, this should proof he or she did the transfer. Hence, simply copying and pasting slatepacks and confirming with a passwords should be ample proof, but it requires different infrastructure/information flow, which exchanges are not used to.

* __dtavarez__ : TOR is probably one of the reasons. Kucoin had an issue that we took too long to solve, the issue is solved today but they haven't update their system yet. I can guess they also need to fully implement the changes to support the latest hardfork.

* __yeastplume__ : Yes, the need for interactivity makes it different from all the other bitcoin-derived coins and makes it a special case to integrate that most exchanges don't want to deal with

* __phyro__ : By far the easiest way to integrate is bypassing Tor altogether. The exchanges should also be aware that they need to be careful of play/replay attacks - though this should be in the integration guide. We currently don't have a guide that helps them understand that

* __cekickafa__ : In my opinion. Grin isnt responsible for those other exchanges. i dont think they have enough Grin reserves,they made a fractional reserve and now slatepacks come,people want to withdraw,they dont have enough liquidity

* __phyro__ : This depends on how exactly they integrate though e.g. which flows they use etc.

* __anynomous__ : Can anyone answer, why not slatepacks, apart from the extra work implementing them?

* __phyro__ : You'd have to prevent spam attack e.g. creating infinitely many step1 slatepacks- or step2 which might write to the database the new output (not sure about that)

* __yeastplume__ : slatepacks are just the transport they don't solve the fundamental issues exchanges have with integrating Grin, in fact they make it worse as it's a whole special layer to implement

* __dtavarez__ : The Slatepacks are robust enough to support the RSR flow by just adding a step but I think that is not a topic for today- I liked @vegycslol 's idea of having testnet implementations
My personal opinion is this: embrace Slatepacks and make it clear that Grin isn't BTC, especially in terms of UX. That could help to reduce confusing thoughts.

* __phyro__ : btw, as a part of https://forum.grin.mw/t/grin-testnet-exchange-example/8570 , I believe @vegycslol had to fix some things https://github.com/pkariz/grin-wallet/commits/fix/invoice-issues
I'm not sure they're good fixes since I'm not familiar with the codebase

* __dtavarez__ : I think it would be better for users and exchanges and everybody involved in Grin's ecosystem to understand and assimilate the interactivity

* __yeastplume__ : The problem with exchanges is the same though, they have 1000 coins to integrate and maintain, and they don't want to spend development time on some strange outlier unless there's a huge financial reason to do so.- with the added bonus now that regulation is getting harder, they need to identify their customers and Grin is designed against that, tx exchanges are a 'special' format, and the wallet is not designed for high-volume robustness, etc
> * __dtavarez__ : I agree- but If we see the Kucoin case for example, the interest was there, they also identified the issue but by the moment we fixed the issue they lost interest. They said they will update their system, but God knows when.

* __cekickafa__ : why? becuz they dont enough reserve atm. others not willing to integrate becuz of that. lots of them will have to delist Grin if price goes up- %80 miners tied up to gate. its 200k volume but other exchages make 1.5 mllion daily volume?. its just fake Grins.

* __defistaker__ : With all security checks and procedures, there should be a demand from users, otherwise integration will be slow

* __yeastplume__ : I think we can add optional layers that make it more acceptable to exchanges.. hardcore users can still use the core functionality of grin for enhanced privacy, but for acceptance purposes the vast majority of users don't have hard core privacy requirements
> * __dtavarez__ : That's correct.
> * __phyro__ : that's a fun problem. Given coinswap being turned on by some users, as a receiver, it's impossible to tell if you're going to receive coins from a coinswapped output (in SRS flow). My hope is that coinswapped outputs are considered 'clean' rather than 'tainted' and this is only possible if the majority uses it

* __vegycslol__ : I don't understand why grin would be any different than the others. It's indeed more private but whoever demands txs from you, you can give payment proofs, exchanges can do kyc (at least i see no reason why they couldn't). We could even have signing keys different to match state's certs
> * __yeastplume__ : It's technically very different from most other coins, it takes time and money and dedicated resources to integrate and maintain, which at the moment far outweigh the benefits of listing it for most exchanges

* __vegycslol__ : Yes for integration i agree, i meant from privacy point of view
> * __cekickafa__ : There is no privacy issue. all exchanges are KYC. monero is listed almost all

* __yeastplume__ : For privacy, you can slap anything you want on top of it to link users, even reveal and log amounts. I'm okay with this in general so long as all intended privacy features remain usable in the core.



## Misc
* __phyro__ : Perhaps we should do some fun community projects for low bucks. I'm not a fan of marketing moves, but at the end of the day, this is how other communities do it and it works. It's extremely low cost, creates better community engagement and builds up fun marketing material e.g. throw 20 bucks at grin halloween meme contest

* __cekickafa__ : At times when Bitcoin maxis discuss and projects Grin as scam. i think Grins biggest problem is its community,more private than coin :) Cryptocurrency is an internet stuff,when no one defends you look bad.Arranging Meetups is a huge thing for Grin imo.

* __vegycslol__ : I think we need ephemeral addresses to avoid some spam/ddos attacks, but that's not for now to debate, just to keep in mind or think about it

* __defistaker__ : After a slow beginning, I am glad to see, so many members joined the discussion. I think we can close today's meeting. Thanks all

## *Action points*

- Discussion: To have quarterly Grin OC meeting- for ongoing maintence requirements.

<br/>


__Meeting adjourned__









