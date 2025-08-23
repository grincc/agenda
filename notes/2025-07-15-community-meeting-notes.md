**Community Meeting Notes July 15, 2025**

Grin Governance Council (GGC) meeting held in Telegram @ 22:34 UTC. Meeting lasted approx. 85 minutes.

Notes are truncated, and conversations are sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

**Community attendance:**

*   Wiesche
*   Ardocrat
*   Ckeci
*   transatoshiツ 
*   Wayne George
*   Alexander
*   defistaker
*   anonymous
*   Smart Move

**Short Summary**

The discussion focused heavily on the status of Grin++, the potential need for an alternative C++ node, and the challenges with PIBD. The development of a new lightweight C++ node by Wiesche was discussed as a potential alternative. An action was taken to contact 2miners about their recommended wallet. The group also covered the need for a Grin multisig implementation, the fix for payment proofs, the status of the new GGC BTC fund multisig, and an update on GitHub organization permissions. Finally, the new Grin-Telegram-Bot was demonstrated, and its associated bounty was discussed for closure. 
Wallet UX discussion.


**Agenda Points & Actions**

Current meeting agenda https://github.com/grincc/agenda/issues/184

*   Fixing peers, Grin++ node bans Rust nodes
*   Multisig Implementation
*   Payment proofs fix
*   GGC BTC Fund Multisig Status
*   Grin Github Organization Permissions
*   Sync/PMMR Issue
*   Grin-Telegram-Bot Bounty 





## Fixing peers, grin++ node bans Rust nodes ##

__Wiesche__: Fixing peers, grin++ node bans Rust nodes.
does anyone know if david is working on it?

__Ardocrat__: Issue was known
https://t.me/GrinPP/45953

__Ckeci__: According to github, no commits since last year.

__transatoshiツ grinminer.net__: This is why I wanted to remove it from grin.mw until development resumes

__Wayne George__: Sounds like PIBD would fix the issue

__Ardocrat__: Some work started
https://github.com/GrinPlusPlus/GrinPlusPlus/commit/1d90b2dc1becf7f5d229f2374c7edd3db63df0d2

  👍 cekic, wiesche,winnie 

PIBD itself has issues
Cause bad peers.

__Wiesche__: i write david
👍 ardo

__Wayne George__: Does anyone here have the ability to work on PIBD?
For any wallet

__Ardocrat__: Together we can

__transatoshiツ grinminer.net__: I don't know that there are any C++ coders around

__Wayne George__: We may not need grin++ going forwards

__Wiesche__: Wiesche is a C++ dev

👍 ardo, transatoshi

__transatoshiツ grinminer.net__: It's gonna remain an issue as long as 2miners has it as their recommended wallet

I can contact them about it

👍 wayne

I'll add it to my calendar

__Wayne George__: I think we need a good alternative to replace grin++. Sorry I haven't used Grim enough to know how it compares

👍 wiesche

__Ardocrat__: Alternative implementation. Grim is grin-wallet (rust)

__transatoshiツ grinminer.net__: It's everything you need in a Grin wallet IMO, the ability to run a node on mobile is 😸

__Ardocrat__: As C alternative - Zig

__Wayne George__: But sounds like Wiesche could build an alternative too

__Wiesche__: I have already started to program a c++ lightweight node. But I'm still in the deep levels (p2p messages, secp256k1-zkp implemented +wrapper, sha etc.)
Messaging and communication goes so far between my node and the Rust node. Wanted to take care of threads soon. But that's a lot of work.

👍 ardo, ckeci, transatoshi, winnie

__Wayne George__: I think we need technical meetings outside of this.

__Ardocrat__: Its here everyday.

👍 wiesche

__Wiesche__: But that only makes sense if David does nothing more on Grin++

__Wayne George__: To help understand how much work is involved to do things

__Alexander__: Why not continue work on grin++? @wiesche

__Wiesche__: I would like an implementation on the QT Framework. CrossCompile and Web.
Separation of the node and the wallet is also important
Getting into other people's code is not always easy either
Building on MSVC alone

## Multisig Implementation ##

__Wayne George__: I do want to bring up multisig too. Any new wallet could consider implementing it
Sounds complicated but perhaps there is support out there if we have the will
Like the Beam dev

__Wiesche__: Multisig must be in the Rust area.

__Wayne George__: What makes you say that?

__Ardocrat__: @wiesche We need to start from docs, discussed with Vladi



__Wiesche__: It is the basis
would you do that?

__Ardocrat__: I am rather engineer than scientist

__Wiesche__: Me too

__Wayne George__: How much is it worth from start to finish to have it? Perhaps we could catch some attention with money

__Wiesche__: I asked david.
If he is not actively working on it, I will continue my developments (c++ node)

__Ardocrat__: Maybe @vlad_gelfer can help
Smart people are at universities

👍 wiesche

__Wayne George__: I think we should keep in touch with him. Seems that most of us ignored his posts https://forum.grin.mw/t/funding-proposal-grin-multisig/11837/6?u=waynegeorge

👍 ardo, wiesche

**Payment proofs fix**

__Wiesche__: Shall we move on to the next point?

Payment proofs fix. @aglkm ?

https://forum.grin.mw/t/grin-product-wishlist/9704/61

__Wayne George__: Do we need manpower to do testing etc?

__Wiesche__: Yes and an implementation if necessary

__Wayne George__: Sounds like we need a funded team to get on with stuff

__Ardocrat__: Hand testing is doing good, writing tests is job @waynegoerge

__Wayne George__: A paid project manager and paid devs

__Wiesche__: yes, I have started to implement the endpoints of the contracts branch

## GGC BTC Fund Multisig and GitHub Permissions ##

__defistaker__: I think first we need BTC fund multisig to fund developers 🙂

__Wiesche__: I can say something about this

__Wayne George__: Sorry what do you mean?

__Wiesche__: We have now set up the wallet.

Anon is taking care of the transfer from the old wallets.

So everything should soon be running smoothly again

__defistaker__: Great, thank you Wiesche.

👍 wiesche

__Wayne George__: Oh you meant dev fund. Yes as Wiesche said.

👍 defistaker

__Wiesche__: I'm really sorry.

I ask several times a week so that we can make progress

__Wiesche__: Next Point

https://github.com/grincc/agenda/issues/177#issuecomment-2973518577

That is a very legitimate question.

Does anyone see any other people there?

__Wayne George__: What is this point?

__Wiesche__: Grin Github organization.

👍 wayne

__Ardocrat__: Seems like all gone after last events.

MimbleWimble

__Wayne George__: Well it seems that we should have a single repo with all GGC members with access for a start

__Wiesche__: but the authorization should not lay with one person

__Wayne George__: We need Yeastplume to help us set up access rights to protect the code but we need access for organisation
But yes perhaps one or two others should even have access to the code

I assume there are still others with code repo access

__anonymous__: Yeastplume gave me access, but I do not have time right now to set up a new directory structure and access for al GGC members. Hopefully soon.

👍  ardo, ckeci, wayne, wiesche

__Wiesche__: To all repos?

__Wayne George__: Would you like help?

__anonymous__: I clicked accept, did not have time to check but I think it was the whole repo.

__Wayne George__: Sounds great!

__anonymous__: I am not a github magician, so if I run into issues I will ask for help in the private chat.

👍 wiesche, wayne

**Sync/PMMR issue and Grin-Telegram-Bot Bounty**

__Wiesche__: Next Point

Synch/ pmmr issue.

https://github.com/mimblewimble/grin/pull/3807

@ardocrat do you have any news?

__Wayne George__: Sorry I have no input on this point

__Ardocrat__: Still migrating to new db

__Wiesche__: Thanks for the update

__Wiesche__: And now the last point

**Grin-Telegram-Bot Bounty**

I have implemented the bot and it is currently being tested.
I have made some coins available.
The bot is used several times a day.
It makes sense for us to store a GGC wallet address.

👍 ckeci

__Wayne George__: could you summarise what the bot can do please? I haven't learned much about it

__Wiesche__: /start@grin_mw_bot

__grin-bot__:
Hi Wiesche,
### Getting the address
1. User runs `/address` command.
2. Bot replies with slatepack address.
The response message template should be customizable.
### Deposit protocol
1) User runs '/donate' to get manual
2) Send a Slatepack to donate GRIN
3) Bot send repsonse Slatepack
4) Finalize
### Withdrawal protocol
1) User runs '/faucet' to get manual
2) Send a Slatepack to receive GRIN
3) Bot send repsonse Slatepack
4) Finalize

__transatoshiツ grinminer.net__: I should've just made the damn bot instead of a faucet www site lol. It works great, though the instructions are no offense really bad.
I'd be willing to rewrite them

__Wiesche__: You can Donate or use the faucet (with Slatepack, Files or TOR).

__transatoshiツ grinminer.net__: It makes sense to established Grin users, but new people aren't gonna understand what it's talking about

__Wiesche__: Write me nice instructions :)

__Ckeci__: it is a great work wiesche. Telegram bot is big boost for Grin adoption.👏🏻

👍 ckeci

__transatoshiツ grinminer.net__: I will, I had to rewrite my faucets instructions several times before people stopped needing assistance

__Wayne George__: So it can be used to receive grin donations or send free grin?

__Wiesche__: here is the process

https://forum.grin.mw/t/bounty-for-telegram-bot-locked/9876/14

👍ckeci, defistaker

Yes, but currently limited to two GRIN per day

__transatoshiツ grinminer.net__: How much of a balance does it currently have? I was going through ~150-250 coins depending on the day giving away 1ツ, giving out 2 is generous but you gotta keep it liquid with small UTXOs or else unclaimed slatepacks will bite ya. I had to write a script to auto cancel slatepacks >15min old.

__Wiesche__: i have write cancel_tx > 10h

__transatoshiツ grinminer.net__: Nice, wish I'd have thought of that initially

__Wiesche__: It is based on the secure API and I have done a
implementation in C++ of the Wallet and Node API.
I will split the implementation into submodules.
Then we can develop more nice tools.

__transatoshiツ grinminer.net__: Gotcha, mine is a lazy implementation using Rust to send bash commands
I plan to switch to API once I'm more familiar with it
+1 wiesche

__Wiesche__: Ckeci we still have to do something about the bounty. Close the thread?

__Ckeci__: Yes, bounty assigned to you imo.👍

👍 vinnie, anonymous, wiesche

**New Wallet Development and UX Focus**

__Wiesche__: That would be all the points.

A question on my part.

Does it make sense to build another C++ node (lightweight)?

__transatoshiツ grinminer.net__: 5 minutes left, shall we wrap it up?
I think as long as Grin++ sits idle, yes

__anonymous__: Grin++ has seperate node

__Wayne George__: I'd say yes if it's bringing something new like PIBD (once working 100%), new UX, other features such as hardware wallet support @wiesche

__Wiesche__: What is your opinion?

__transatoshiツ grinminer.net__: NikolasFlamel has already made firmware for Grin on Trezor and Ledger that someone could use to do that. I use the standalone HTML wallet with a Trezor safe 3 @wiesche

👍 wayne, anonymous

__anonymous__: I would first check if it does what you want it to do. Perhaps some tweaks and you have a better Grin++ node or a light version of it.

👍 wiesche

__Wiesche__: I find the connection to Qt quite charming.
Also for a wallet later with WebAssembly.

__Wayne George__: I assume no one wants to work on grin-gui in rust?
I would

__transatoshiツ grinminer.net__: I would

__Wiesche__: Grim is the new grin-gui

__anonymous__: GUI programming is not my thing, I stick to bug fixing for now.

👍 wiesche.

__Smart Move__: Do you to open source this , will like to contribute @wayne (I assume no one wants to work on grin-gui in rust?)

__Wiesche__: Are you working on something special?

__Wayne George__: It is already
https://github.com/mimblewimble/grin-gui

__Smart Move__: Cool,
On it

__anonymous__: Not much, little time. For now only fixing grin-wallet config generation and some wallet errors.

__Wiesche__: I'm glad to hear that

__Wayne George__: In any wallet we make, I say that we should focus more on UX over technical features
It should be easy for the average person to use too
Our wallets are currently very techy
we could have an advanced mode for techies

__Wiesche__: I think Ardo did a lot on the Ui from GRIM

__Wayne George__: I need to have a good sit down with it

__Ardocrat__: More simplicity added, but not on release yet, current problem is Tor, cause not working everywhere
Can build from source to get last changes

__Wiesche__: Which Os are you worried about?

__Wayne George__: Do I need cargo and all of those things?

__anonymous__: For easy to use wallets, most important to get the node to be better, faster, more stable etc. O, and linking node (e.g. on Umbrel) to wallet via QR. Light wallet that can do that would be great.

👍 wayne

__Wayne George__: I use to struggle building grin-wallet back in the day lol

__Wiesche__: is quite simple

__Ardocrat__: Its ISP problem.. Obfs4 bridges blocked
Tor deactivated my acc on Gitlab

😠 wayne

With Proxy can only send

__Wiesche__: Umbrel, docker, node I would probably tackle.

🔥 annymous

Maybe a thread with a bounty makes sense.
So purely official

__Wayne George__: Nice conversation here. I'm glad we can be open about our challenges and offer solutions

__Wiesche__: Unfortunately, I have never dealt with this before
for no reason?

__Ardocrat__: I got this email later after registration
Its important for mwixnet, as it uses Tor

🔥 wiesche

__Wiesche__: That's right.
So many construction sites


__transatoshiツ grinminer.net__: Getting me access to the website resources like the registrar and web server




__Wiesche__: + Umbrel impl. Bounty
Maybe there will be more developers.
Otherwise I would take on the topic.

__Ckeci__: Summary 

**TO DO List**
Btc fund multisig
Github reorganization
Fixing peers grin++
 Payment proofs fix
Access to grin.mw website:server and registrar
Bounty idea: Umbrel implementation.

🔨 👋🏽

**Meeting adjourned**
