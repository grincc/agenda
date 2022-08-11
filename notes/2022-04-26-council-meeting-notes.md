# Council Meeting Notes April 26, 2022

Community Council (CC) meeting held @ 15 UTC in grincoin#general channel on Keybase. Meeting lasted 62  min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_

* anynomous
* yeastplume
* cekickafa
* defistaker
* phyro
* dtavarez
* vegycslol
* mineexpert




# Short Summary

-  Request for funding @davidtavarez May-July 2022 is discussed.
-  Grin book donation/funding request format is discussed.
- 

# Agenda Points & Actions



* Last meeting notes here: https://github.com/grincc/agenda/tree/main/notes

* Current meeting [agenda](https://github.com/grincc/agenda/issues/54)

1)  Request for funding @dtavarez May-July 2022 https://forum.grin.mw/t/request-for-funding-davidtavarez-may-july-2022/9740 

2) Discuss what funding or donation format would be best to support the creation of this Grin book https://forum.grin.mw/t/request-for-funding-grin-book-ascendio-minexpert-may-december-2022/9741/3
  
__anynomous__ : 
Welcome to todays CC meeting.
First lets start with a short summary, there is so much going on right now in the community to get excited about:

Announcements:
A lot of great things happening. For those who did not monitor the forum and KeyBase, some highlights.

•    There is a new node party with 20 new nodes thanks to David T.
https://github.com/grincc/agenda/issues/54

•    Nice map of all nodes out there, also thanks to David T.:
https://nodes.grincc.mw/

•    Update from Scilio, he finished Milestone 2 and will soon submit a Pull Request for the Coin Swap implementation here:
https://github.com/mimblewimble/mwixnet

•    Grin wallet contract prototype
https://forum.grin.mw/t/grin-wallet-contract-prototype/9745

•  Mimblewimble/mwixnet: Implementation of the Mimblewimble CoinSwap proposal.
https://github.com/mimblewimble/mwixnet

🚀 cekickafa, satoshocrat


For todays agenda, you can find it here: https://github.com/grincc/agenda/issues/54

Lets take 2 minutes to read the agenda, and the spam of interesting developments I just posted above.

__cekickafa__ : 2 min:)

__anynomous__ : You can take another 30 seconds if needed.
For our first agenda point.

## 1) Request for funding @dtavarez May-July 2022

__anynomous__ : He asks funding to continue development of Grin++, he wants to focus on better support for uses censored countries using tor bridge, payment proofs accessibility in the UI and API and one-time use addresses. Is that about correct @dtavarez ?

__dtavarez__ : Correct.

__anynomous__ : It is to soon to vote on it, but first I would like to welcome any feedback. Are these things that David should be working on, are there things missing in the request?

__dtavarez__ : I must say that these working point are prioritised by direct feedback from grin++ users. People were reporting problems to sync so I did work on that in the last release v1.2.7

__vegycslol__ : if you have 2 one-time addresses and 1 global one, how many tor listeners do you have? 3?

👍 anynomous

__anynomous__ : In my opinion they are also worthy working on. Many users from China and Rusia report problems right. Payment proofs and one-time use addresses are improving Grin as a day to day currency since it allows for matching payments to orders, automatic dispute settlement etc. As far as I understand you would indeed have 3 tor listeners in such a case. Not sure how many you can technically have without running into troubles.
Has anyone tested having multiple tor listeners active at the same time?
It is not recommended by the tor project: 
https://support.torproject.org/tbb/tbb-36/

__cekickafa__ : not  experienced.

__vegycslol__ : i haven't, i'm just curious about the solution.

__anynomous__ : Me to. I think it might be challenging to have many, already having 2 online at the same time would be great.

__vegycslol__ : what are we trying to achieve with one-time addresses? You could implement an address book (you give different address for each user which allows for banning/filtering transactions) or you could try to hide your tor endpoint

__anynomous__ : Trying to hide your endpoint.

__vegycslol__ : but hiding tor endpoint may not be as efficient since once you leak your global address then it's out there forever

__anynomous__ : In that sense, this could also be achieve by temporarily switching from the main tor address to the one time use address.
Indeed, basically you want to leak only adresses to risky parties that you use one time.
Having to turn of the main listener would allow coupling of the one time use address to the main address...

__vegycslol__ : sure but what do you do when someone you trust leaks it

__dtavarez__ : taken from the slatepack RFC.

__cekickafa__ : might be efficient,if you move your coins from global to  other wallet.

__dtavarez__ : By default, all wallets should generate a new SlatepackAddress for each transaction for improved user privacy and security. Wallets can optionally support the ability for a static, reusable receiving SlatepackAddress with a warning about the privacy risks of reusing these addresses.

__anynomous__ : It will never be 100 protective. Best would be to use the next account with the same wallet mnemonic in such a case, which would result in a new address.

__dtavarez__ : I think wallets implementation should follow approved RFC as much as we can

__anynomous__ : Yes, agreed. I am not certain anymore how multiple accounts are used right now in the wallet. I would have to look it up.

__dtavarez__ : I believe that it was a good recommendation and I want to implement it

__anynomous__ : I think we should explore this further. It will take some time and discussion but it is worthwhile IMO

__yeastplume__ : it's not trivial if you're opening a new tor listener each time

__dtavarez__ : I know.

__yeastplume__ : the idea of one address per use doesn't really sit well with the notion of creating a load of hidden services on tor, they take time to propagate and a lot of services going up and down on tor won't be reliable at all
so I think that's mostly why it hasn't really been done that way in the past.

__vegycslol__ : are we sure someone actually dove into the details when this RFC was defined? It sure sounds great at first, but the details should be carefully thought out

__anynomous__ : Maybe it is possible to run tor as a fake relay node. Meaning you pretend to relay for your own multiple tor addresses, that would allow one listener with multiple adresses.

__dtavarez__ : expiring the address every 24 hours seems to be an option imo too
instead of changing the address after signing an incoming tx. expiring the address every 24 hours seems to be an option imo too.

__vegycslol__ :

>__dtavarez__ : expiring the address every 24 hours seems to be an option imo too.

sure but there you have a race condition, which might be annoying for people who don't do both communication rounds on the same day

__dtavarez__ : so, do not enable it then. it is optional

__yeastplume__ : I've never been 100% happy with tor anyhow, single use addresses would work better via some other system, even BBS style (but that's a larger conversation)

👍 anynomous, dtavarez ,phyro , satoshcrat

__vegycslol__ : iirc bbs can be spammed. Anyway that's too big of a topic, continue as if i didn't ask any question.

__anynomous__ : you can run 2 relays on one IP4...
https://community.torproject.org/relay/relays-requirements/

__dtavarez__ : look, this is not written in a stone, but I want at least to entertain the idea, test it, and if it works, it works, if not, we don't merge it into the master branch

👍satoshcrat

__anynomous__ : There is also a very pragmetic option. One time use addresses do not suport tor, so default to slatepacks...

__dtavarez__ : I don't mind to be wrong

__anynomous__ : Being wrong is perfectly fine. I think the topic is interesting enough to spend funds on.

__vegycslol__ : the more we try the more we know 👍

__yeastplume__ : if only we could ever figure out a place to put a BBS style system.. agreeing a place where both parties can access should be simpler than needing a direct route between them
Yeah, experimentation should be what it's all about anyhow

__anynomous__ : Lets maybe continue this on the forum. In summary there are multiple interesting angels to explore:

a) Trying to pretend to be a relay to allow multiple tor addresses (so basically relay internally), or other haxor way to run multiple tor instances
b) Bulletin system. This has come back in many discussions, we should entertain this idea as well.
c) Be pragmatic and implement one time use addresses without tor.

__defistaker__ : what is BBS? Bulletin board system?

👍 anynomous, vegycslol

__yeastplume__ :

>__defistaker__ : what is BBS? Bulletin board system?

yes. pin your slatepacks on a board.

👍 defistaker

__anynomous__ : Lets continue with our second agenda item for today:
2)     https://forum.grin.mw/t/request-for-funding-grin-book-ascendio-minexpert-may-december-2022/9741/3
EDITED
Personally, I would love to see this book happening. 
I do however find this funding request somewhat challenging for multiple reasons. Therefore, I thought long and hard about it and checked our objectives and spending guidelines as a council:
https://github.com/grincc/docs/blob/main/spending-guidelines.md
The request appears to be in line with the objective:
-> Supporting non-profit, community-driven and inclusive promotional efforts for the Grin 

So this book can be seen as a ‘promotional effort’ by the community. The CC is allowed so spend some funds for this objective. However, the amounts to be spend were always supposed to be small amounts. E.g. some small funds for a meme or video contest, some free beers at a meetup etc. Secondly, we must consider the value of such a book to the community. Although I think the planned book has added value, I do not think the added value would warrant 2.500 * 9 = 22.500 euro of spending of the Community funds, even if that would be cost for the writer. 

Third thing to consider is the funding format. Personally, I think a bounty or one time donation upon completion by the CC combined with individual donations might be more suitable than a monthly amount. The exact amount the Grin Community Council can or should donate is something that requires some more discussion and thinking and should include the CC members not present today. That is roughly my opinion.

What do you all think?
https://github.com/grincc/docs/blob/main/spending-guidelines.md


Apologies, I am moving on to quickly. For the minutes of today. We cannot make an official vote yet on the funding request from David since it is to new, but thumbs up or down to indicate if you are in favour or against funding David T for this funding request.

👍 defistaker ,anynomous , cekickafa , phyro ,satoshocrat

__yeastplume__ : I am glad to see him continue work.

💯 phyro

__anynomous__ : I count that as a 👍

__yeastplume__ : (I don't vote on CC things, but don't want silence to be interpreted as disapproval)

👍 anynomous

__dtavarez__ : I will disappear only when users can buy/sell pizza without problems using grin. meanwhile I will stay

👍 yeastplume ,satoshocrat

__cekickafa__ : payment proofs sounds like a music to my ear.

💯 anynomous

__anynomous__ : The humbs up or down are open for everyone. This is not yet an official vote by CC members 
Alright, we will take that information to the other CC members for deliberation and official voting after the funding request had at least 1 week to gather feedback from the community.
For now back to our second funding request, the Grin Book, project Ascendio.
I expressed my long opinion and deliberations above:
keybase://chat/grincoin#general/48168
TLDR, I would love to support this book in one way or another. But the funding type as monthly amount, as well as the total amount are above what I think we should be spending for promotional efforts.

👍 defistaker, cekickafa , phyro ,yeastplume

What do you all think, is this something we could create a bounty or donation for? This would however not be in the order of the amount requested, it would be smaller and only upon completion.

__dtavarez__ : it is unfortunate that our community is not large enough to raise that kind of money. I love @minexpert writings

😊 minexpert

__phyro__ : yeah, I really like his blog posts

😊 minexpert

__anynomous__ : Same here, that is why I am willing to bend the rules a bit, because I am a fanboy.

__minexeprt__ : If I share my own thoughts again; I think the book will be a great ad campaign for Grin. Let's just think about this. Can we describe Grin to people in a few tweets or a few words? So we can think that this book will be the main advertising campaign.

👍 mo5itoo

__anynomous__ : We already have the GRINOIR, but that is hardly a book for regular people, only for the real crypto enthousiast.
 Yes, I think we can use this for advertisement as well as education.

__defistaker__ : https://tmgox.com/product/grinoire-cypherpunk-anthology-book-pre-order/

__anynomous__ : So it has some value, but I think a monthly fee is not best suited for that.

__dtavarez__ : That said, I think support that we should focus on supporting in-person meetings where people would get together to share a beer or a coffee and to chat and help each other set up public nodes, and/or portfolios; and also supporting the network and development. I think we should find an opportunity to support the book initiative somehow.

__yeastplume__ : just a suggestion that books/articles are usually written using an advance. Agree a total fee, then advance a percentage towards it, with the rest payable on release

👍 dtavarez

__anynomous__ : Agreed, we should spend more finances and effort on physical meetups.However, I also want to see what we can do to support this book. Good sugestion by @yeastplume.
Thumbs up or down on whether you think a donation or bounty should be in place to support this book, we can do a advance on that before release.

👍 dtavarez , phyro , vegycslol ,yeatplume, anonymous

__yeastplume__ : (that usually assumes royalties or a publisher making money though, might not be suitable)

👍 dtavarez

__anynomous__ : Well, we are making 'profit' on community education, and outreach that can enrich the community.
Thumbs up or down in the vote above☝️
We can lower the cost by using community for checking the English. Ok, now the more difficult part, how much of a donation from the CC would be warranted? 

__vegycslol__ : I mean since he said he didn't get anything from the previous donations, i don't expect donations to play any role in paying for his work/expenses.

__dtavarez__ :

>__anynomous__ : Ok, now the more difficult part, how much of a donation from the CC would be warranted? 

I think that can be discussed later; I would suggest something to bootstrap the project, but we should chat with @minexpert directly first I guess

👍 minexpert

__vegycslol__ : to get the final price for the work/expenses one would probably need to know how many chapters the book would have, how many pages, how many hours are expected to write it, what are other book related expenses etc

__anynomous__ : Agreed. We should also consider how much public information and documentation could be reused or not.

__dtavarez__ : that's why I think we should chat first to know how much it is needed to at least bootstrap the project

__anynomous__ : Alright, lets discuss this further on the forum as well as in direct chat with @minexpert

__dtavarez__ : I have never written a book I don't know the details

__vegycslol__ : 

>__dtavarez__ : I have never written a book I don't know the details

that seems to be the main issue we're having, we don't know  about it :D

👍 anynomus ,dtavarez ,cekickafa 

__anynomous__ : As much as possible, lets crowdsource what we can. E.g. language editing, lets just use volunteers. I volunteer.Thanks all for a productive meeting. 




   ## *Action points*
 - Discuss about Bulletin Board System on https://forum.grin.mw/
 - Discuss about implementing one time use addresses without tor on forum.
 - @dtavarez funding request for May-July 2022 accepted by community, GRINCC      will  vote until next meeting.
 - @minexpert Ascendio Book project funding format is more to be discussed on the forum as well as direct chat with @minexpert



**Meeting adjourned.**


















