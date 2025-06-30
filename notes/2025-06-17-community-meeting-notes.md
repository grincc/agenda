Community Meeting Notes June 17, 2025

Grin Governance Council (GGC) meeting held @ 22:32 UTC in Telegran public chat channel . Meeting lasted approx. 66 min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

**Community attendance:**

*   Wiesche
*   Anonymous
*   Wayne George
*   Ardocrat
*   transatoshi
*   John Tromp
*   Defistaker
*   Ckeci
*   LozengeVault
*   Yeastplume
*   Alexander (aglkm)

**Short Summary**

*   Discussion on consolidating governance structures, including merging GitHub organizations (grincc into mimblewimble) and websites (grin.mw).
*   Agreement to use the `mimblewimble/grin-pm` repository for GGC project management and organization.
*   A plan was formed to address issues and make updates to the grin.mw website, including menu consolidation and fixing broken links.
*   Deliberation on fixing Tor (Arti library) instability, with the action to first open a GitHub issue to engage with Tor developers.
*   Brief update on the new 4/7 multisig setup and the need for a Slatepack 2.0 RFC.

**Agenda Points & Actions**

Last meeting notes here: https://github.com/grincc/agenda/tree/main/notes 

Current meeting agenda https://github.com/grincc/agenda/issues/177
1.  GGC Organizational Setup (GitHub, Websites, Project Management)
2.  Tor Transactions and Partnership


**GGC Organizational Setup: GitHub and Websites**

_Wiesche_: 👋🏻

_Anonymous_: Lets take 1 minute to check the agenda, see if there are topics anyone wants to add.

_WayneGeorge_: There's a lot that we can discuss. Let's decide on the most important

_Anonymous_: I think the most important think is to get the Grin Governance Council (GCC) up and running. That means for example on deciding where on github to combine information such as project overviews, wish lists etc. What do you think would be most important?

_Wayne George_: I'm not too familiar with the TOR topic
Yes, I agree that organisation is most important. It should be our foundation to build upon

_Anonymous_: Are @johntromp and Yeastplume in the house? Because I want their opinion on whether we should move governance to a subdirectory of mimblewimble or keep it separated for now.

_Ardocrat_: Arti Tor lib needs to be integrated into grin-wallet for stability later

_WayneGeorge_: Yes some OC views would be very welcomed

_transatoshi_: What about using the kanban boards built in to github?

_Anonymous_: O, cool, I did not know they had that. Is it a plugin?

_WayneGeorge_: At the moment there are two organisations on GitHub. Should we just have one? I think so

_transatoshi_: We can track project progress with those

_Ardocrat_: https://github.com/orgs/mimblewimble/projects

_anonymous_: We should have just one, a new one. We can merge and move all relevant documentation there. For many parts, e.g. spending guidelines, there is no major difference between the OC and CC, so combining them for the GGC should be nor problem.

_WayneGeorge_: I think we can manage access within the org so not everyone can touch core code for example

_Ardocrat_: Github is social network, but for coders, important for Grin to attract more devs
We can adopt open-source ethos here with enough manpower :D

_Wayne George_: So abandon mimblewimble/grin?

_anonymous_: Well, manpower has always been the bottleneck 😉

_WayneGeorge_: I'd say that should remain and we add projects to it

_transatoshi_: Not abandon, but the member list needs fixing

_Ardocrat_: need to actualize members list

_anonymous_: no, we keep everything more or less as is. But some stuff from the Community Council github we merge or move to mimblewimble/some_directory

_WayneGeorge_: Yes we could revamp everything
Including the grin.mw website

_Ardocrat_: http://grincc.mw/

_transatoshi_: Ugh, that sites CSS is a MESS
It's all on one line

_WayneGeorge_: I think we should unify everything as we are doing with the council

_anonymous_: I would not change the website, it has a very unique house style that sets it apart. Same for the logo, we had quite some discussions about it.
Ok, well if you can fix it, go ahead 😁

_Ardocrat_: here some dead links

_John Tromp_: just got here

_anonymous_: 👋
What would be your opinion on where we can best put all the Grin Governance Council files on github.
See discussion above.

_WayneGeorge_: I don't mind the grin website though

_John Tromp_: where is it located now?

_defistaker_: So are we gonna combine grincc.mw and grin.mw?
I agree with @transatoshi_grinminerdotnet , it would be hard to modify grin.mw

_anonymous_: We want to prioritize getting everything organizationally setup. So have a place at github to put files, project overviews, canvas boards etc. CC is now on https://github.com/grincc/

_John Tromp_: oh, i think grin.mw makes more sense than grincc.mw

_Ckeci_: We can keep both. What is the harm ?

_John Tromp_: ah, a decentralization fan!

_anonymous_: And for github, should we just make a governance subdirectory for github.com/mimblewimble, what does the OC have there.

_transatoshi_: I can try adding some pages to grin.mw for the GrinCC info, not to shutter grincc.mw, but to have all info consolidated

_Wayne George_: I think for simplicity so everyone knows where to go to find out what's happening across the entire project

_Ardocrat_: just update info :D

_anonymous_: Just from a practical point of view, might be easier to have one simple website with governance information that can be easily updated, main website is more of a hassle I think. So keep that for everything non governance related.

_Wayne George_: A single place to keep updated
A single org containing different projects

_John Tromp_: i think grin cc can be considered part of https://github.com/mimblewimble/grin-pm/tree/master

_defistaker_: grin.mw is older/official. It is a no-brainer if we keep one

_transatoshi_: DM me what info and broken links need updated and I'll do it

_anonymous_: Can you give all GGC members access there, we can start moving/merging governance related documents to there
Only we also have Grin Hub
https://github.com/grincc/hub
I think somewhere there was something similar but not updated on github.com/mimblewimble. Perhaps we need to merge that as well.

_Wiesche_: I agree

_anonymous_: We need some information on how easy or hard it is to update and add information to grin.mw.
Preferably it would be semi automated, e.g. edit a markup file, push update to the website

_Wayne George_: Good point

_John Tromp_: i'm trying to figure out who has commit rights on grin-pm

_Ckeci_: lehnberg

_Wayne George_: If someone is told to go and look up Grin, we want them to be able to find signs of life lol

_John Tromp_: Yeastplume as well

_transatoshi_: I've updated it a couple times. It's not difficult as long as you don't need to touch the CSS.

_anonymous_: Ok, well I see no need to touch the CSS unless there is a bug.
Since you have most experience on this, as well as other websites, can you see if there would be a way to make it easy to push updates to a specific governance section on grin.mw @transatoshi_grinminerdotnet? Or is already as easy as editing a text or markup file?

_Ckeci_: Grin.mW most important section is Download part, recently i updated. Other forum link, newsletter uptodate. Keybase link will be removed.

_transatoshi_: It's as easy as updating the HTML files

_anonymous_: To summarize:
https://github.com/mimblewimble/grin-pm/tree/master will be our new home.
@transatoshi_grinminerdotnet will for now do the website updates, since I think she is the only one who knows how 😉.
I will look into where to put Grin Hub, perhaps we can also make it a new subdirectory of github.com/mimblewimible.
@johntromp can you together with Yeastplume look into getting the permissions set for GCC members?

_Wayne George_: Could we review the menu? I don't think we need so many tabs

_anonymous_: I do not think it is an issue, perhaps on Mobile it is too much, but on Desktop this is quite normal.

_wayne George_: Not the quantity but the confusion

_anonymous_: For example, you could remove GitHub, but for developers and die hard crypto enthousiast, github is all that matters.

_Wayne George_: Community and Forum are the same thing for example

_John Tromp_: isn't it enough that any of them can make Pull Requests? If Yeastplume needs help reviewing them we can add another member with commit access

_transatoshi_: Mobile looks okay

_defistaker_: I agree, Research can be moved under docs, but all other links are fine

_transatoshi_: Okay, so I'll move research under docs, and forum to the community page. How about I add the main telegram group to community too?

_anonymous_: Perhaps, but if for example if we have Grin hub under mimblewimble, I think it is ok to give everyone access to it.

_Wayne George_: Last blog was 4 years ago

_Ardocrat_: external links can be separate

_John Tromp_: sure, but i don't know how fine grained commit rights can be. whether they can be applied to subdirs. for a separate project, it would be fine to add more members with commti right

_Wayne George_: Removing unused links would keep things looking smarter

_anonymous_: In the Community Council we also had it that multiple reviewers needed to agree on changes to for example security (4) related documents, but for documentation (2) and finances (2) , a bit less, for hub (1) , everyone can edit.
Yes, they can be fine grained I think, not on the file level, but on the directory level.

_John Tromp_: i'm not that well versed in git management:-(

_Wayne George_: I think pull requests only for now would work as long as the reviewing doesn't take long due to work load

_anonymous_: I am also not well versed in git and github, unfortunately.
Yes, for now it is fine, we can smooth things out over time in case reviewing would become a burden.

_Wayne George_: Yes I think we should add the Telegram but under community?

_transatoshi_: Will do

_Ckeci_: can we have info about Merging funds/ multisig process situation ?

_Wayne George_: FYI, I get different menu options on mobile than I do on desktop

_Ardocrat_: need to show hash https://grin.mw/download

_transatoshi_: Can you screenshot it?

_Ardocrat_: link for hash can be malicious
0ab24691608bd06abdcdab1dc545cbc034c9b51540cd3d559325822ff4fef822

_transatoshi_: Oh, blog is on mobile
not big
I see it
I'll axe that

_Wayne George_: Blog is Forum on desktop


_transatoshi_: Someone else automated that in JS, I don't really wanna fuck with it

_Ardocrat_: I told ya, its like sabotage

_anonymous_: Don't change it, I think it automatically links to latest version on github, saves time in manual updating.

_Ardocrat_: when github not show unicron
external links
bro
can be local link
or text
more trust

_anonymous_: In any case, if github is down, users cannot download grin to begin with, so I doubt they will need the hash
Perhaps we need to think a bit if it is worth changing this.

_Ardocrat_: so you think we can launch own Git, I have experience with Forgejo, I push here and Github is mirroring automatically
https://gri.mw/code/explore/repos
also mirrored some Github repos from MW here

_transatoshi_: So docs.grin.mw is a whole other docker based animal, I'll remove research from Grin.mw and work on getting in on the docs site later

**Tor Transactions and Partnership**

_anonymous_: Considering the time I think we should move to our second agenda topic for now. This discussion can continue when the meeting has ended.
2) Tor transactions and partnership.

_Ardocrat_: CI can be done for release builds, I made before at Github, but do not trust 3rd parties anymore, cause once had problems with Github as well
*DO NOT STORE SECRETS ON GITHUB*

_Wayne George_: What's the gist of the Tor topic?

_anonymous_: But a hash is not a secret right, it is a proof.
This topic was added by Alice

_Wayne George_: Is no Tor restricting use?

_anonymous_: @ardocrat can say more about it. I think problems with instability of tor.

_Ardocrat_: for iOS/Android build you need private keys for example
possibly

_anonymous_: Well, give it shot 😛

_Ardocrat_: now we wait Arti forward progress, I can not launch Onion service behind proxy

_transatoshi_: Does using orbot get around this?

_anonymous_: O, so are we now using Arti, but it is not working behind a proxy?

_Ardocrat_: the only restriction I found
you can send request but not accept
need to contribute here
open problem
maybe we can contact Tor devs
give them BTC for this :D

_anonymous_: Ok, is that a small thing to tacke or not. If it is important but not too big, we could consider putting a bounty on it. This is typically one of those things that require zero integration in grin or grin-wallet itself, just new function to the library.

_Ardocrat_: Tor is living for donations

_anonymous_: I agree on this, I think it is the most pragmatic approach, let those who are experts on it fix it.
But I do not know if others agree...

_LozengeVault_: lol

_Ckeci_: well it is very good idea. Tor collaboration.👍

_Ardocrat_: yeah, grin is very integrated here
mwixnet works with tor
we can attract devs from Tor possibly

_anonymous_: Who knows, perhaps they can solve our peer to peer issues

_Ardocrat_: they also have experience with POW
Tor uses POW at load
maybe they can try Cuckoo
:D

_John Tromp_: cuckoo is less suitable for such applications

_anonymous_: Anyhow, @transatoshi_grinminerdotnet @waynegeorgeh @johntromp @aglkm Yeastplume @sled_dogs, do you think it makes sense to let the tor team fix this issue in the Tor rust/arti library, and we can make a modest donation?

_John Tromp_: because you need to search many graphs to find one cycle

_anonymous_: So easy to verify, hard to calculate

_John Tromp_: for blockchain pow that doesn't matter, since there are tons of miners
but for e.g. antispam protection, having to search many graphs is a nuisance

_Ardocrat_: But it can be used to make tx to protect API endpoint from DDOS right?
https://github.com/mimblewimble/grin-wallet/issues/44

John Tromp: equihash has an advantage in having 2 expected solutions per instance

_Ardocrat_: user can mine and wait to make request

_wayne George_: TBH honest I don't fully understand the issue but if members think it's worth it for the wider community then yes. If it's only a minimal use case then perhaps not

_anonymous_: I also do not know how widespread the issue is, but if it is considered important by some, it is worth some support.
What do you think @johntromp, did the OC ever support library implementations or similar that were used by Grin as project? Of course we are a new council, so we can decide to do things different than we did as CC and OC before.

_John Tromp_: the only library i think we supported is a custom version of secp256k1 with Pederson Commitment primitves

Yeastplume: 👋

_John Tromp_: welcome, Michael!

_Yeastplume_: evening! fashionably late

_Alexander_: I remember @ardocrat complained in other tg group about lack of functionality in arti library he needs for Grim, but we, as CC, need to understand what's the issue first and then make any decisions.


_Ardocrat_: can not launch tor service behind proxy

_Yeastplume_: will catch up on convo

_anonymous_: I think since we are at least giving it some serious consideration, we should turn it into a forum discussion. So discuss the option of donation/bounty for Arti (tor rust) upgrade to work behind proxies.
We need to see if this is just changing one line of code or a lot of work for someone.
We need to know what the expected functionality is that we want or are asking for.

_Ardocrat_: discuss or just contact them and easy subscribe problem :D

_amonymous_: We can also do both, perhaps they know of the issue, perhaps they will just fix it out of their own initiative.

_Alexander_: I would open an issue on arti github about it, then wait for their feedback, and then we can decide what to do. At least we'll have a documented issue we can refer in future.

_anonymous_: Just to make sure this results in an action, who will open the issue, you @aglkm or @ardocrat?

_Ardocrat_: issue is they are using native tcp, it goes directly to system
same for p2p now

_anonymous_: Perhaps you can open the github issue @ardocrat, you know clearly most about this topic.

_Ardocrat_: Issue can be good start 👍

_anonymous_: When you made a github issue, can you share a link here, so we can all follow and join the discussion on the github issue.

**New 4/7 multisig setup, Slatepacks 2.0**

_anonymous: I think with that we can close the official part of this meeting, plenty to do. Feel free to continue the discussion.
Thanks for being here all 😁

_Wiesche_: One question about NEW multisig 4/7 setup

_anonymous_: O, well to give an update. We are nearly ready to create the new MultiSig (4/7). When we have it setup, I will update the security repository to show the address for the new GCC Bitcoin wallet.

_Ardocrat_: I introduced before Beam Core developer @vlad_gelfer can work on this, we just need to form RFC, step by step, Beam also has no multisig, only at dapps level

_Ckeci_: Thanks, previous follow up topics..mentioned.

_anonymous_: And we need another RFC for Slatepacks 2.0 (to support multi party interactions and things like script hashes, perhaps some other fields), I will see if I can help there, but only as support. There are more knowledgeable people on this topic.

_Ardocrat_: Marek worked on them at Python implementation, maybe we can attract old devs too :D
https://t.me/grinventions

_anonymous_: O cool, I did not know Marek worked on extending Slatepacks 👍😎
A I see, just regular slatepack support. Still very important. Python is ideal to play around and modify to test new concept versions.

_Ardocrat_: everyone can write python
rust can be behind python even
https://github.com/PyO3/pyo3

_Yeastplume_: yes, pyoxide, really popular, rust is really being accepted by python developers as a better alternative to performance-intensive libs than c

_anonymous_: I also use rust wrapped libraries where possible. On average I get 1.5-2x the speed compared to wrapped C++ libraries. Rust is really the best. Unfortunately I still find it challenging to program in Rust as easily as in Python.

_Ardocrat_: building time is faster on Air M1 than on x86 Pro
for cross-platform Zig linker only works, not native :D
https://github.com/rust-cross/cargo-zigbuild

_anonymous_: I will put this in a note tomorrow, need to explore this more. For now, 🥱😴

_Ckeci_: Meeting 🔨 👋🏽

**TO DO List**

*   _Grin Governance Council_: To investigate where to host the Grin Hub within the `mimblewimble` GitHub organization,set permissions for GGC members on the `mimblewimble/grin-pm` repository.
*   _Grin Governance Council_: To provide an update on the new 4/7 multisig creation and update the security repository with the new wallet address once ready.
*   _transatoshi_: To update the `grin.mw` website, including consolidating menu items (moving Research, adding Telegram links), and removing unused pages (Blog).
*   _ardocrat/aglkm_: To open a GitHub issue on the Arti (Tor) repository regarding the inability to launch an onion service behind a proxy and share the link with the GGC.
*   _GGC_: To create a forum discussion about a potential donation/bounty for the Arti library fix after getting feedback on the GitHub issue.
*  

**Meeting adjourned.**