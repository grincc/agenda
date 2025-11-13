**Community Meeting Notes September 09, 2025**

Grin Governance Council (GGC) meeting held in Telegram @ 22:30 UTC. Meeting lasted approx. 60 minutes.

Notes are truncated, and conversations are sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

**Community attendance:**

*   Ckeci
*   anonymous
*   Ardocrat
*   Wiesche

**Short Summary**

- The discussion reviewed the status of several ongoing projects and issues.
- Updates were provided on the Umbrel/EmbassyOS node project and the Cuckatoo reference miner conversion. 
- Lack of progress on a MultiSig implementation and the the possibility of setting a large bounty for the MultiSig RFC and implementation.
- Grin node persistent synchronization problems,the causes of slow Initial Header Sync.
- A  bounty idea to analyze and fix P2P networking and storage bottlenecks.

**Agenda Points & Actions**

   https://github.com/grincc/agenda/issues/188

*   Follow-up on Pending Issues & Project Updates
*   Discussion on  MultiSig Implementation
*   Deep Dive: Grin Node Peer and Sync Performance Issues
*   Proposal: Bounty for P2P/Sync Improvements

## Follow-up on Pending Issues & Project Updates ##

__Ckeci__: No topics. Same follow ups remain.

__anonymous__: **Follow Up**

    Fixing peers, grin++ node bans Rust nodes.
    Payment proofs fix.
    Grin Github organization.
    Grin MultiSig
    Funding request Grin Node meets UmbrelOs, EmbassyOs
    Request for funding Cuckatoo reference miner

There are only updates on the last two topics.

__Ardocrat__: Good night 😁

__anonymous__: 
>@wiesche "Unfortunately, I was in the hospital last week and had surgery.
But everything went well.
However, there has been progress.
I put the package together in a Docker container and created a Docker Compose.
I am currently configuring a volume for the blockchain data.
I have ordered some hardware on which I can run UmbrelOs so that I can create an image for testing.
The web UI currently has the following functions:

    Status
    Connected peers
    Configuration of settings (server.toml)
>@wiesche 
Next steps
As soon as the environment with wasm and the C++ client in Docker is working in UmbrelOS, I will implement all API endpoints.
After that, I will be happy to provide the first image.
The whole thing is currently running with Rust Node. I still need to take a look at Grin++ (API)."
-Wiesche on the forum:
https://forum.grin.mw/t/funding-request-grin-node-meets-umbrelos-embassyos/11928/25

Regarding the " Request for funding Cuckatoo reference miner"
-Thomas has been hard at work but he should not rush too much. He is often asking for review while he has not checked himself whether his validator produces correct output by comparing it to the reference implementation in Rust/C++

__Wiesche__: I bought a Raspberry Pi 5, which should hopefully arrive tomorrow.
My proxmox server is Full 🤪

__anonymous__: Do you also know how to compile for the Umbrel Home? I have no experience with cross-compiling, but I can help test on my Umbrel Home if needed.

__Wiesche__: Docker with nginx, c++ => wasm

__anonymous__: Well, as long as you know how to do it... I don't have to 😁

__Wiesche__: Workflow for deployment
https://github.com/getumbrel/umbrel-apps

__Ardocrat__: https://umbrel.com/
Can work as VM?

__anonymous__: It basically runs everything as Docker/VM. I think you can run the OS it itself also as VM

__Wiesche__: I think it's good that he's working on it.
If he keeps at it, it'll work out.

__Ardocrat__: Sadly can not run Docker directly on OpenBSD :)
I use Alpine VM for this

__anonymous__: Takes about 4 GB in overhead as run as VM:
https://git.iko.soy/getumbrel/umbrel/wiki/Install-umbrelOS-on-a-Linux-VM
O no, 4GB is just what is recommended. So probably half of that, 2 GB

__Wiesche__: And many users
@ardocrat gri.mw is back? 😍

__Ardocrat__: Only front
Need to setup CI.
Forgejo runners.
It can even use macos.
For release builds.

**Discussion on Stalled MultiSig Implementation**

__Wiesche__: Have you had a chance to talk to Vlad yet?
Ios would be awesome.

__Ardocrat__: I guess he is busy now

__Ckeci__: then we have to define a big bounty Bitcoin prize amount and look for other candidates

__Ardocrat__: Yeah, miner
Good for decades.
Grin can launch satellites.
No fund in Grin.
No multisig.

__Ckeci__: Grin fund surpassed its marketcap, it is a shame!
really? so govts gave you permission to throw satellite for a privacy coin ?

__Ardocrat__: We need this for whole MW ecosystem @vlad_gelfer 🙏
DEXes integration, post-quantum maybe

__Ckeci__: vlad is not interested obviously
now narrative changed from inflation to quantum ?

__Ardocrat__: Privacy before quantum
with a superior emission and without scripts
in the best case there will be a post quantum equivalent to pedersen commitments, preserving MW, and only losing some simplicity and efficiency

__anonymous__: Ok, but we can deal with that in ....50-150 years from now. O and then you still would need a quantum leap in development, qbits at the moment appear not to scale at all.

__Ckeci__: quantum . This is nonsense excuse, excuse me. As if we gonna all die, why should we sleep and eat.
now

__Wiesche__: So it's out of the question for multisig implementation?

__anonymous__: Quite that, quantum computers at the moment is just nonsence. Someone should wake me up if they can do more than quantum compute 7!, which is 7*6*5*4*#*2*1... something you can even calculate from the top of your head 🙃

__Ardocrat__: Conversation is open

__anonymous__: Lets see. It all starts with someone writing an RFC (Request For Comments) proposal for MultiSig.

##  Grin Node Peer and Sync Performance Issues ##

__anonymous__: Did anyone have time to look into grin node peer issues or speeding up Initial Header Sync?

__Ckeci__: 2019, 2020 multisig roadmap planned? https://github.com/mimblewimble/grin-pm/issues/385
it is 2026. 7 YEARS

__Wiesche__: Unfortunately, no....

__anonymous__: Yep. Without developers who can tackle some of these issues (like MultiSig which is complex), we can have as many wishlists as we need without achieving our targets.
Other things on that list do have been acchieved, like PIBD. I remember the first time I tested it, it was a mega improvement in speed, most time was just consumed by Header Sync which was not part of PIBD.
But since then it became more problematic, I think because people on purpose are creating bad peers to create sync problems. It is the only explanation of something that worked quite well, becoming much more frequently not working well.

__Ckeci__: What is your opinion about this anonymous? why Grin dont have developers?

__anonymous__: I honestly do not know why there are not more developers. Some reasons I can think of:
a) Grin is complex and not a low hanging fruit to work on
b) Crypto is highly competitive
c) we do not pay for time but for output. This reduces the risk for the project, but it does create a threshold or filtering of only truly interested and capable developers joining the project

__Wiesche__: We would need to work on prioritization and the ban.
How fast is the exchange between two local nodes 1:1?
To do this, only one mode needs to be fully loaded.

__anonymous__: I do not have the right setup to test 1:1 node syncing. I do know that it actually becomes faster, so fewer peers is faster. This is another reason why I wanted to look at the peer management, there is some bottleneck that should not be there.
All file sharing systems speed up with more peers, Grin, the opposite.

__Ckeci__: it was 6-8 peers lst year, now cant pass 2 -3 peer. It takes 1 day to load a 4 gb blockchain

__anonymous__: It simply does not make sense. There is a que or waiting time somewhere, like wait for peer A to send, before contacting peer B. According to Yeast it is parallel, but I think it is not truly.

__Wiesche__: 10h

__Ckeci__: with start and stop 10-12. Continous restart the node.

__anonymous__: In the past I managed to download full chain within 1 hour with multiple peers. Now many slow peers that increase waiting time like crazy.

__Wiesche__: Interesting point, I can test it with two nodes when the Pi arrives.

__anonymous__: What I do know is that even if evil actors actively sabotage the network, if we get grin working on Umbrel nodes, we can at least significantly improve both the ease of setting up a Grin node as well as increase the speed. The Umbrel Home, which many people use is actually quite beefy and way faster than a Raspberry Pi 5. It has vastly supperior memmory bandwith (10x or so) and a very fast build in SSD.

__Ckeci__: something is not adding up. A silent sabotage i fear maybe. I am not expert but if it works like a duck it is a duck

__anonymous__: Still, this is no excuse not to tackle the software side, I just lack both time and expertise in P2P part of node. For now I am picking up my old pull request to fix config generation, that is all I can handle.\
Where is that recorded? Could very well be fake numbers.

__Ckeci__: i am talking it as a whole. Not only peers. That % 70, %100 hashrate jumps and downs is not normal.
how is that fake numbers? multiple mining sites, grincoin.org. Check yourself.

__anonymous__: I just had a look at it.
Ok, probably it is real. It appears to correlate a lot with price, so probably high end GPU miners joining the Grin fray. Grin is quite lucrative to mine 😁

Is grin++ faster without pibd?
Yes, they use very strict banning and only a single peer.
I do not think it is a good system, PIBD is the way to go. We just have to find that !@#$@# bottleneck.

__Ardocrat__: A lot bugs can be reproduced on testnet
P2P needs rewriting 😁

__Wiesche__: Is there a P2P points system for exchanging peer information?

__Ardocrat__: So everyone will be able to share p2p port for sync, even mobile

__anonymous__: Yes, for header sync it is very much flawed. It is not major complex code, even I can partly comprehend it while I am just a beginning Rust dev.
No point system, that would be an improvement. Now there is a lot of waiting for peers, then ask another peer and only in very rare case give a time ban and in very extreme case (obvious false state send) full ban.

__Ardocrat__: FlyClient solves problem with headers, less data to download
Beam has this, we can adopt this for grin too, discussed with @vlad_gelfer

__Wiesche__: What if the bottleneck is not P2P but storage?

__Ardocrat__: Storage too 😁

__anonymous__: I did check with the storage buffer, increasing buffer size gave some improvements, but there are still major bottlenecks. E.g. if a peer does not respond, it takes a while to ask a new peer.
You can find my initial finding here:
https://forum.grin.mw/t/fine-tuning-grins-parallel-independend-block-download-pibd/11613/3

__Wiesche__: Sounds serial

__Ardocrat__: Jetbrains provides nice debugger

__anonymous__: I think there is a problem with how the parallel system works, basicaly it is a loop with too much waiting.
Perhaps it is also running checks too often. What I mean the node is always checking in what state it is, then after some test move to header sync and request peers. I think instead it should have a loop to ask many peers and only ocasionally fall back to the loop where it checks if it should still do header sync or move on to PIBD,
When I was looking at the code I was even wondering if it was made by design to be slow :/

__Ckeci__: lol
i dont wonder

__anonymous__: Anyhow, best thing is a) complete rewrite of Header sync b) improving peer management with a scoring system c) selecting fast peers for initial sync

## Proposal: Bounty for P2P/Sync Improvements ##

__Wiesche__: Let's create a bounty for analysis and bug finding. That's an important point.
Or should we really define milestones for multisig and write sums on them?

__anonymous__: Yes, it does makes sence to define a bounty. We should very well describe the conditions, because we do want to keep multi peer syncing and althoug we can revise peer blocking, we should not be too strict towards slow nodes.
Perhaps we can start a discussion on the forum for a bounty to improve Header Sync (preferably PIBD like implementation) and improve overal sync speed by fixing bottlenecks in P2P messaging + writing to discs + proper peer banning rules
I think this is way more doable than MultiSig which requires a cryptographer.
Someone decent in Rust might already be able to vastly improve sync speed.

__Ckeci__: So pay with Btc or GRin ?

__anonymous__: Whatever people ask for I would normally say, a bit harder with Trade Ogre down/gone, but we can probably still pay in Grin if asked by a developer.
But I think it would be best to denominate any bounty for now in BTC since it is more stable.

__Wiesche__: I believe that once the error has been found, it can be remedied relatively easily.

__anonymous__: I think so, honestly, I do not think it is even hard... I am just that poor in Rust.

__Ardocrat__: Python can use Rust

__Ckeci__: No need to carry this unnecessary burden of fear quantum shit. Multisig bounty should be declared with a BIG Bounty and implemented.

__Ardocrat__: 1 BTC?

__anonymous__: We can discuss within the CC if we are open to create a bounty for MultiSig that does include a) submitting and b) approving an RFC.

__Wiesche__: I would probably like to continue working there in the long term.

__Ckeci__: you are very generous. i think it should be no less than 5 bitcoin. As you fear quantum thing, a solid work must be done

__anonymous__: 1 BTC sounds right, but perhaps @johntromp or Yeastplume can better estimate a suitable bounty. First we need to openly discuss whether we will for the first time pay, or request the submission of an RFC as part of that bounty.
It would be a first.
Ok. I am off for tonight. Great chatting with you all. It is always great to talk with others who wish Grin well and want to move the project forward.

__Ardocrat__: Scientific work
Easier to implement with RFC, need to know what to do

__Wiesche__: Thanks for the chat, have a good night.



**TO DO List**
*  Fixing peers, grin++ node bans Rust nodes.
* Payment proofs fix.
*  Multisig RFC bounty submission.

🔨 

**Meeting adjourned**
