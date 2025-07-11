**Community Meeting Notes July 1, 2025**

Grin Governance Council (GGC) meeting held in Telegram @ 22:30 UTC. Meeting lasted approx. 64 minutes.

Notes are truncated, and conversations are sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

**Community attendance:**

*   Ckeci
*   defistaker
*   Wayne George
*   Ardocrat
*   Кейл (trab)
*   anonymous
*   rainbow sixpoint5
*   Manuel
*   John Tromp
*   transatoshi
*   Wiesche
*   Smart Move
*   Alexander

**Short Summary**

The discussion covers follow-ups from the previous meeting, including the GGC multisig BTC fund status and GitHub/website reorganization. The main points include unifying grincc.mw with grin.mw, managing permissions for the grin-pm GitHub repository. Other topics are a proposal for CI self-hosted trusted binaries, the possibility of holding public voice chats for community engagement, the technical discussion of a database change for wallet performance, and addressing pending payments.

**Agenda Points & Actions**

*   Follow-up: GGC BTC Fund Multisig
*   Follow-up: GitHub Reorganization & Website Consolidation
*   Welcoming New Contributors. 
*   Secure Binary Builds
*   Grin synch PMMR
*   Pending Payments



Ckeci: 👋🏽

defistaker: 👋

Wayne George: 👋

Ardocrat: 👊

Кейл: ☝️

anonymous: 👋

rainbow sixpoint5: 🙌

Manuel: 👋

__Ardocrat__: good night

__Wayne George__: Are you going?

__anonymous__: Or just wishing us all a good night.

__Ardocrat__: slow mode 60 seconds

__anonymous__: Not chairing today, so time to enjoy a meeting with some beer🍻

__Wayne George__: Let's make a start and anyone late can catch up

__Ckeci__: Ok, there is no topic added, follow ups from previous meetings: GGC btc fund multisig and Github reorganizatioin.

__Ardocrat__: we are missing someone

__John Tromp__: 👋

__Wayne George__: Ah I didn't realise that there's no agenda today

__Wayne George__: I don't think we finished last meeting's one though

__anonymous__: I remember there were a lot of #ToDo's last meeting.

**GitHub Reorganization & Website Updates**

__anonymous__: @transatoshi_grinminerdotnet updated the website, that was one item on the To Do list

__transatoshiツ grinminer.net__: 👋

__Wayne George__: Yes, some website tidy up

__transatoshiツ grinminer.net__: Some people are still complaining about the top nav bar, I will experiment with giving it a background
I'm still moving so I'll find the time somewhere

__anonymous__: In a way I find it a pity to change it. Alternatively, now there is some pixel magic involved. Would it be possible to sample from all the pixels and just average the color on grayscale?
That would keep the magic intact but make it work on a chaotic background.

__Ckeci__: i think It looks neat, transatoshi.

__Wayne George__: Are we happy with the current GitHub and website setup generally?

__defistaker__: Are you talking about grin.mw or grincc.mw?

__transatoshiツ grinminer.net__: Yeah I could do something like that, I think it looks fine with a semi-transparent gray bg too
Grin.mw

__Wayne George__: I like having the org stuff in the mimblewimble repo

__anonymous__: I do think it make sense to arrange that. Wee need to get access to a folder there to the pm directory to put our github projects.

__Wayne George__: Personally I think we shouldn't have two websites and two Github organisations as it indicates division

__anonymous__: Was Yeastplume going to look into how to arrange the access rights for the project management repository?

__Wayne George__: We can do pull requests in the meantime until it becomes an issue
https://github.com/mimblewimble/grin-pm

I propose that we use this for all Meeting and governance content
👍 wiesche, tromp, anonymous

__anonymous__: Pull request are fine for changes to the documentation, however to have Git projects, you do need admin rights to that repository, righ?

__Wayne George__: Ah yes maybe

__anonymous__: And to some folders like for note keeping, best to just give full access.

__Wayne George__: We can set that as a todo. I'm happy to look at that if no-one else wants to

__anonymous__: Perhaps you can discuss it with Yeastplume, I think he was also looking into it. We have to look back into our privacy GCC Telegram chat where it was discussed.

__Wiesche__: Sry 👋🏻

__Ardocrat__: grincc website is outdated

__Wayne George__: I don't think we need it. I'd like to hear other's opinions but we technically don't have a CC anymore

__transatoshi_: Let me know what needs updating and I'll do it, I'm just too busy rn to review the whole thing myself

__Ardocrat__: unite with grin.mw everything to avoid fragmentation
👍 waynegoerge, rainbow, wiesche

__defistaker__: One of the objectives for grincc.mw was tracking funded projects and display a wishlist for newcomer developers, but it did not take off. Funded projects usually don't have regular progress updates

__Wayne George__: As an organisation thing, perhaps if we assign specific wishlist items to specific GGCC members who can take lead on them. So little micro projects. That person can then be the go-to person for that area

**GGC Bitcoin Fund Multisig and New Contributors**

__Кейл__: How is the new wallet to manage funds coming along?

__John Tromp__: we're waiting for David B to receive his hw wallet.
👍 ardocrat ,wiesche

__Smart Move__: Hi everyone, Am a rust developer , Contributed to bitcoin open source projects like Ferdimint and cashu. Wondering how I can contribute to this project.
👍 trab, wiesche, rainbowsix

__Wiesche__: Dot Bridge

__Wayne George__: Polkadot? Yes that was interesting. More reason for multisig as was mentioned
Hi! We have many things that are open to look at. We have experienced devs around if you have specific questions. Otherwise here is a good place to have a conversation about things you like

__Wiesche__: Yes, we need more developers

__rainbow sixpoint5__: is design help needed?

__Ckeci__: how did you learn grin, may i ask ?

__Кейл__: Welcome! So you probably already know Rust and know that Grin is interactive like Lightning? Maybe set up an account on our forum for easier asynchronous communication
👍 anonymous, wiesche, ardocrat

anonymous: Welcome, you can start by looking at https://github.com/mimblewimble/grin and https://github.com/mimblewimble/grin-wallet. There are quite a lot of open issues. Also functionality we would like to add. We can also discuss it on the the https://forum.grin.mw/

__Ardocrat__: hey, grin-wallet has no ability to select outputs on send now, for example

__Smart Move__: I will definitely do that
>@ckeci: how did you learn grin, may i ask ?
Twitter on a rust channel conversation
👍 ckeci, wayne
Is their a separate dev channel or all dev conversations happen on the forum

__Ckeci__: https://keybase.io/team/grincoin. Check #dev channel.

__anonymous__: I am not implementing coin control, just allowing better config creation and better use of the -t (top-dir) and -h (here command). There are more things I want to work on but Coin Control is not among them.

**CI/CD for Secure Builds**

__Ardocrat__: can we launch CI on grin.mw for projects, it can be more trust for binaries?

__defistaker__: By projects, do you mean grin and grin-wallet?

__Ardocrat__: gui too
👍 defistaker

__Wiesche__: CI is already available after every build, isn't it?
Or are you thinking more of nightlys or something similar

__Ardocrat__: yes to build on own server, not 3rd party, I think its important cause we have no strong signatures like iOS/MacOS on all platforms
👍 wiesche
also for release build, you need signature, it can be done with some script, by release manager
👍 ckeci
signature storage - its important not store secrets on Github etc

__Wiesche__: I had already suggested two tools that we should host ourselves:
CI => Jenkins
CD => Nexus
with a docker registry and raw files
👍 wiesche

__Ardocrat__: Java, banking standard :D
Jenkins is like swiss knife
eats ram @defistaker



__defistaker__:  good old java :). They are at trying to minimize it with graalVM in some projects.

**Community Outreach via Voice/Video Chats**

__Wayne George__: One other topic that came up is about video or voice chats. X Spaces was suggested some time ago. I do think as a community we should have more content out there for newcomers to learn about the history and visions for the future. We already are encouraging more GGC meetups to encourage comradery
+1 wiesche, rainbowsix

__rainbow sixpoint5__: this is important imo
I don’t want to open up to development by committee, but there should be more open ways for learning and involvement.

__anonymous__: It is indeed good and motivating to have more interactive meeting opportunities. I do have to warn though about privacy, not sure that X Spaces is at all privacy respecting...
👍 %100 wiesche, cekic, rainbowsix

__Wayne George__: As a suggestion, rather than general conversations, we could set a topic, appoint a chairperson, and have an open public discussion that can be recorded
We could use anything really if we just use voice
👍 anonymous

__rainbow sixpoint5__: Lots of people that were excited about Grin in 2018/19 are wondering what happened to the project and are starting to see BTC get swept up with wallstreet, bankers, govt etc
👍 wiesche

__Wayne George__: I think linear emission is such a strong attribute that should be emphasised more. Fair emission for generations
Other cryptos implemented it post such as Monero and Doge

__anonymous__: Yep, the creators could have called grin "Fair coin", because it is fair by design and fair in the sense of elegant/nimble, minimal design.

**Wallet Development and Technicals**

__Wiesche__: @ardocrat What is the status of the sync (pmmr)?
backend for pmmr is lagging

__Ardocrat__: Changing database, need to make migration
https://github.com/mozilla/rkv/blob/main/examples/simple-store.rs
https://t.me/grim_app/9002

__Wiesche__: Have you already gained experience?
@ardocrat
This is a very important point
👍 ardocrat

__anonymous__: @ardocrat Changing database, sounds like something you should discuss with Yeastplume
There might be alternatives such as identifying the cause such as a) to many call, b) latency in writing etc.
👍 wayne, wiesche

__Wayne George__: Is changing database a grin-wallet thing?

**Grin Multisig and Pending Payments**

__Wiesche__: In general, we need to push the topic of multisig (Grin)
+1 wayne, wiesche, ckeci

Wayne George: We need to reach out more
Perhaps see if any Beam devs fancy it
Beam do look like they've done a ton of stuff
I don't know what their user base it like though

__anonymous__: We did start the discussion on the forum, now we need someone capable to work on an Request For Feedback (RFC) Proposal
The Beam developer on the forum was quite helpful. Perhaps he might want to work on it, ...but it does require first having an RFC
👍 wayne, wiesche

__Wiesche__: @mubitech23

__defistaker__: May I ask about expected date for waiting fund requests to be paid?

__Wayne George__: Once we have the new multisig sorted, any outstanding payments can be made swiftly
👍 wiesche, anonymous, defistaker

__anonymous__: Like paying our groundkeeper.
👍 wiesche

__Wiesche__: Do you have anything pending?

__defistaker__: Yes, hosting expenses for grincc

__Wiesche__: Okay, we'll do our best to get this sorted out as quickly as possible

__defistaker__: thank you



__Wayne George__: I must leave now. Please anyone, feel free to contact us outside of these meetings with any questions, suggestions or issues. I think that I speak for the rest of the GGC that we aim to be transparent and engaging with the community at all times

__Ckeci__: Ok, any more topics ?

__Ardocrat__: Gn all

__Wiesche__: Gn

__Wayne George__: GN

__anonymous__: Also leaving, thanks all 👋

__defistaker__: Good nite

__Ckeci__: ok, meeting 🔨, but open discussion can continue. Thank you all. Gn


**TO DO List**

* GGC 4/7  Multisig process.
* github re-organization.
* Synch/PMM2:


**Meeting adjourned**