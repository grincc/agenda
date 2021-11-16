 # Council Meeting Notes November 09, 2021

 Community Council (CC) meeting held @ 15 UTC in grincoin#general channel on Keybase. Meeting lasted 45 min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

<br/>

### _Community attendance:_

* __anynomous__
* __yeastplume__
* __jankie1800__
* __cekickafa__
* __defistaker__
* __renzokuken__

<br/>

# Short Summary

- Grin integration Bisq Dex is ongoing.
- A list of [grin tools](https://github.com/grincc/tools) has been published by __anynomous__
- __yeastplume__ is getting back to grin development, working on issues and PIBD.

<br/>


# Voting Results

<br/>

no votes held


# Agenda Points & Actions

* Last meeting notes [here](https://github.com/grincc/agenda/blob/main/notes/26-10-2021-community-meeting-notes.md).
* Current meeting [agenda](https://github.com/grincc/agenda/issues/22).

<br/>


## 1) Agenda

* __anynomous__ : Welcome everyone to todays Grin CC meeting.
Find the agenda here:
https://github.com/grincc/agenda/issues/22
Lets take 2 minutes/seconds to read it ;)

    For today's agenda we only have one official item:
-bisq-network/growth#205 (comment)
Grin integration Bisq DEX.

    Personally I am hyped if Bisq would continue its support for Grin since in spirit Grin really fits well with Bisq

    For who did not do so yet, please upvote the DAO proposal:
https://github.com/bisq-network/proposals/issues/350
 
    I only red up on the discussion last minute so I do not know all the details. Does anyone know if any actions are required from the grin community/developers?

* __jankie1800__ : I noticed the bisq developer mentioned they have already started working on the proposal as well.

* __anynomous__ : I think the developers are really in favour which is a great sign. Still the DAO vote is needed to make it official.
If no actions are needed from us there is little else to do but :crossed_fingers:

    Since   __@yeastplume__ is here. I was wondering, are you actively working on grin or grin-wallet at the moment? I did not have time to check github.

> * __yeastplume__ : I'm starting off by picking up PIBD again on grin itself, but I'm also going to start slowly looking at outstanding issues/PRs in both repos as well as try and get development as a whole moving again.
> * __anynomous__ : Great, I was hoping someone would pick up PIBD again, it was a real pity that it was dropped.
> * __yeastplume__ : a lot of work was already done, it needs to be put together and the actual sync process defined; I'm about to merge https://github.com/mimblewimble/grin/pull/3659 which is the first bit of work to get it going again. 
> * __yeastplume__ : BTW applying PIBD to the header sync portion as well would be a huge win, if anyone wants to think about how that might be done.
> * __anynomous__ : Would it? The header part is rather small right. Or would it be a big win since many nodes are only leeching and not seeding.
> * __yeastplume__ : I've just synced from scratch a few times, the header portion always takes a couple of hours
> * __anynomous__ : Ouch, ok, that is still a lot. And not that many transactions in blocks yet means the header takes up relatively a lot of space.
> * __yeastplume__ : for me at least, it's a YMMV thing obviously, but optimising it to allow parallel downloading from multiple clients via PMMR segments would help this significantly
> * __anynomous__ : Yes, the benefits should be equal for any type of data.
> * __yeastplume__ : but yeah, the txhashset.zip file exchange is extremely inelegant, so it makes sense to phase that out first
> * __anynomous__ : Remind me, PMMR stand for... something merkel?
> * __yeastplume__ : Prunable Merkel Mountain Range. It's an append-only data structure that forms the basis of how all of the chain data is stored.
> * __anynomous__ : a, prunable, yes.
> * __yeastplume__ : There's actually a good doc here I've been using to remind myself https://github.com/mimblewimble/grin/blob/master/doc/mmr.md
> * __anynomous__ : Thanks, I should read up a bit more on the technicals, I am getting "Rusty", and not in the good programming way:sweat_smile:
> * __yeastplume__ : So yes, PIBD is basically just chunking this structure into segments, so the segments can be transferred in parallel and the results put back together at the other side to re-create and validate the PMMR. I'm a bit rusty as I get back into being Rusty, but getting there :smile: 
> * __anynomous__ : Great. Who know, maybe one day I can join the fray, but still much to learn.


* __anynomous__ : Maybe it is useful to post a short overview of the current things being worked on for Grin:
    >    ### Developers ##
        Rahul S | hunter | hunterburn
        [ ] Not working yet
        Sheldonth
        - [x] working on multiple wallet support in grin-wallet (no payment needed for now)
        Scilio
        - [x] working on Coinjoin, nice progress being made with a lot of active reviewing by Tromp:
        https://forum.grin.mw/t/request-for-funding-scilio-coinswap-implementation/9149/51
        Gene
        - [x] working on Atomic swap, needs to update RFC for further reviewing by Tromp
        Mark Hollis
        - [x] working on Ledger hardware wallet support
        David T
        - [x] working on updating Grin++ mobile and desktop wallet
        * __yeastplume__
        - [x] Working on issues/PRs for grin grin-wallet, picked up PIBD for faster block syncing (headers also for in the future)?

    So many things are actively being developed at the moment, not even all paid. I hope @hunterburn will get warm for Grin as well, since there is still a lot of work to do on grin and grin-wallet.

* __yeastplume__ : I'm available for reviews, but it's still going take me a while to get back into the swing of things.

* __anynomous__ : No problem, glad to have you again among us:grin:. We were really short handed for a while on capable members for RFC's 

* __yeastplume__ : Thank you, it's good to be back and you all seem to be doing a great job on the community side!

* __anynomous__ : I would like to request everyone to review:
https://github.com/grincc/tools

    I started indexing all repositories related to Grin, scripts, tools and documentation. It is however very incomplete, especially many links to good documentations and articles are missing. 
    Personally I think it is important to create a hub and better manage all our resources (developers included :stuck_out_tongue:)

    Feel free to add anything directly via a pull request or post any missing links in comments.

    Are there any other topics, items that anyone would like to see discussed now?
    We have plenty room for open discussions, brain farts etc.

* __cekickafa__ : what s the situation of iPOLLO Miners?

* __anynomous__ : Just some further updates:

    - Groundskeepers have been paid
    
    - Community miners are being delivered soon (they are paid and in transport at the moment)
    after they arrived we will start distributing to the community members who ordered them.
    There are still plenty of miners available if you are interested.

* __jankie1800__ :  last it was mentioned there was a G1 available. groundskeeping is going nicely. I'm enjoying expanding on the community inituitives 

* __renzokuken__ : I already written my letter to Santa for this year and it has only one thing on the list...

    1. https://github.com/tromp/grin-rfcs/blob/early-payment-proofs/text/0000-early-payment-proofs.md#slate-changes

* __anynomous__ : Yes, exactly. We have ordered the G1 + 42 G1 mini, of which 12 are reserved for the council, another 5 are already reserved by community members, that leaves another 25 available.

    Proper payment proofs would solve a lot of issues with exchanges, not sure in what stage that proposal is.

* __cekickafa__ : i can reserve 2.

* __anynomous__ : Do you want 2, sure, DM me, it makes it easier for communication and for getting your address information.

    That leaves 23 available.

    Well, that was all I had to mention, discuss for today.
    Unless there is anything else we should discuss, I would like to wrap up the meeting for today and thank you all for attending. 
Lets press onwards:muscle:, many interesting developments with Grin lately:grin:

## *Action Points*

- Community members can contact with * __anynomous__ for hosting remaining miners.
- Community members are invited to support grin Bisq integration via upvoting [DAO proposal](https://github.com/bisq-network/proposals/issues/350)
- Community members are invited to review [grin tools list](https://github.com/grincc/tools)

__Meeting adjourned__