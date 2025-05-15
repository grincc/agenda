# Community Meeting Notes 06 May 2025

Community Council (CC) meeting held in Keybase. Meeting duration approx 1 hour 40 minutes 

Notes are truncated, and conversations are sorted based on topic but not always strictly chronological. Quotes are edited for brevity and clarity.

### _Community attendance:_

*   waynegeorge 
*   defistaker
*   anynomous 
*   transatoshi
*   bobo123grin 
*   cekickafa

# Short Summary

- The meeting covered several key areas. Initial discussions focused on peer connectivity issues between Grin++ and Rust nodes, with plans to log and submit an issue. 
- Follow-up items from previous meetings were reviewed, including pending actions on Grincoin.org donations, Groundkeeper funding, and payment proof testing; the GrinCC website update was noted as completed.
- The main agenda items included an exploration of Nym integration for enhanced privacy and connectivity
-  Grin fund disclosure and wallet history management, and a request for reimbursement of past server costs for the GrinCC.mw website, which was approved pending verification.

# Agenda Points & Actions

*   Follow-up on previous action items:
    *   Donation to Grincoin.org
    *   Groundkeeper voting for funding request
    *   Payment proofs fix
    *   Update GrinCC website
*   Fixing peers, grin++ node bans Rust nodes.
*   Exploring Nym integration/usage with Mwixnet, TOR peers, Tx flow.
*   Disclosure of grin funds.
*   Request for server cost Grincc.mw site.

## Fixing Peers: Grin++ Node Bans Rust Nodes

Discussion initiated by agenda point.

**defistaker**: I checked the c++ code, could not see anything specific to rust nodes. I think it just bans the nodes because of timeout, and I believe Ardocrat is working on rust implementation.

**transatoshi**: I've discussed with him that there are some big issues with the P2P implementation of the nodes at least on testnet. Basically the nodes will sync but can't find peers after being shut down then restarted.

**transatoshi**: Not yet, he has more info than I do, but I will shut down and restart a node later and log and submit an issue.

**anonymous**: I also looked at the code, the only difference is that they ban peers when they are delayed by for example sending late since the node is busy preparing a zip file. Perhaps on mobile with unstable connection this can lead to a lot of banning. So basically when in lack of peers, the node should start unbanning peers. Also seed nodes should be exempted from banning.

**anynomous**: Ok, I think we know a bit better now what needs to be done to improve Grin++, those are not major issues but in certain circumstances such as poor network stability, it can become a big issue.

## Follow-up Items Review

**anynomous** outlined the status of previous follow-up items:
*   **Donation to Grincoin.org**: Nothing has been done, prioritised other issues within the CC.
*   **Groundkeeper voting for funding request**: Still a lack of response here, yet community wants up to date administration…
*   **Payment proofs fix**: We need to test the contract branch that contains these proofs.
*   **Update GrinCC website**: Thanks to @defistaker the website was updated.

**transatoshi**: I'll update the meeting page dates on the grincc site in a bit and submit a pull request. Anything else need done on the site?

**anynomous**: Nothing that comes to mind right now. But perhaps soon, we are discussing major changes to the CC after all.

## 1) Exploring Nym integration/usage with Mwixnet, TOR peers, Tx flow

**anynomous**: I know nothing about Nym, does anyone has anything to say about this topic?

**cekickafa**: @ardocrat idea but he is not joining as well.

**defistaker**: It says it is a paid service https://nym.com , would we need to pay for running nodes?

**anynomous**: Looks like some sort of payed VPN, that works a bit like tor but then with a fixed path of 3 nodes. But David Chaum is the inventor, he is no slouch.

**waynegeorge**: Just Googling Nym now. Has someone mentioned how it would help Grin?

**cekickafa**: Mesh network. In case Tor banned in certain places.

**anynomous** (quoting Nym docs): "While Tor may be the best existing solution for general-purpose web-browsing... mixnets are better than Tor for message-passing systems such as cryptocurrency transactions... The Nym mixnet provides superior privacy by making packets indistinguishable from each other, adding cover traffic, and providing timing obfuscation... uses incentives to both scale and provide censorship-resistance."

**waynegeorge**: I suppose if someone has the enthusiasm to experiment with it, I'd support that.

**anynomous**: It looks promising, but to be honest I do not think it is something we can help much with as Governance body. If anyone needs funds to implement it… yes we can help.

**defistaker**: It seems to be opensource, at least libraries. (Referencing Nym's licensing: GPLv3 for applications/binaries, Apache 2.0/MIT for libraries, Apache 2.0/CCO-1.0 for documentation).

**anynomous**: Ok, so in summary. We all support the idea of any endeavour to test the use of nym in grin wallets if such a request is brought forward. With that I think we can close this topic.

**bobo123grin**: If ardocrat agrees nym topic, I agree.

## 2) Disclosure of grin funds

**anynomous**: I think it was requested who runs the CC grin node. First I thought it best to keep that information within the CC, since it is a single wallet and not a multisig... But after reconsidering, who care, its value is not much anyway. So when the CC was started me and Hendi both started a copy of the grin CC wallet, we both have a backup of the seedphrase. I run the node and wallet on a Raspberry Pi400 and since then I had to reinstall at least 3 times the complete OS. I think the issue is because it uses an SD card for storage which is not that stable.

**transatoshi**: I don't like the idea of using cloud hosting for the node by principle, but don't think there needs to be disclosure where it is or who runs it.

**anynomous**: Now if this was any other blockchain, restarting from seedphrase would not be a loss of data, but for grin it is. Because your wallet only scans for unspent outputs and does not remember or recover history of spent outputs, not even when running an archive node.

**waynegeorge**: By trust I mean a way for a donor to see that their donation gets added to the CC pot. Maybe, sadly perhaps, there isn't a need for a grin donation wallet.

**bobo123grin**: I put forward this topic, but I think grin funds is transparent, I have checked the spend history.

**cekickafa**: Grin funds is not transparent. Bitcoin fund is transparent.

**anynomous**: Yes, but the problem is that my node gives me a different number than the accounting we have. The reason is that accounting using grin wallets is a pain. Since after a restore you lose information... So the grin CC wallet history is in shambles. I asked Hendi to send me a backup of his transaction history since his node did not have so many failings as mine since he uses a normal computer.

**anynomous**: The long term solution is in my opinion to implement a separate scan command for archive nodes that builds the chain state based on the full history... Still having the dates and values would be incredibly useful if you need to piece together the transaction history for a freshly restored wallet.

**anynomous**: It takes a lot of time to do this bookkeeping, it is all manual basically... Probably my time is better spent if I fix a bug in the grin-wallet code or build a new feature.

**bobo123grin**: Agree. When grin price €100, you have to spend the time for bookkeeping.

**waynegeorge**: Would be good to create some form of automation. If a transaction appears in the wallet history, a commit to the CC site is made, perhaps even pushed.

**anynomous**: In the coming meetings I will update if we get the grin wallet administration fixed or have more clarity. That would be nice, there is a lot of things that can be improved IMO.

## 3) Request for server cost Grincc.mw site

**anynomous**: @defistaker the floor is yours.


**waynegeorge**: I saw the quote of 456 Euros. Why so much?

**defistaker**: Well, I had been hosting grincc for a period of time, but at one point, site is moved to another server. It had been running over three years. On a shared CPU plan of 12 Euro/month. It was only for GrinCC, it is a 2GB small vps.

**transatoshi_mw**: I'm always available to host anything people don't want to pay to as long as it is Grin related. Why not github pages or S3 hosting for free? It's a static site, right?

**defistaker**: It is a react/next site, so there was a node server running. I did not pick 1GB plan because it was running out of memory on build etc.

 

**anynomous**: I think it is fair to compensate the costs. Yes they are quit a bit since things accumulated over time. I am still checking with @future3000 if he did not inform you at that time, I think he simply forgot to do so.

**waynegeorge**: (Initially concerned about cost, then understanding it was for ~40 months) Oh I see, sorry. Makes sense to reimburse then.

**bobo123grin**: €456 for 40 months is ok.

**anynomous**: Ok. I think with that we can close this topic. We will reimburse when the CC is up and running again and able to sign, either with old or new members.
**defistaker**: Thank you @anynomous.

**anynomous**: Thank you all for joining today, it was nice to have so many people joining for a change.

**Meeting adjourned.** 

## *TO DO List*


*   **anynomous**: Follow up with Hendi for a backup of his CC grin wallet transaction history to aid in accounting.

*   **anynomous**: Verify with @future3000 whether @defistaker was informed about the GrinCC.mw website hosting move.

*   **Grin CC**: Reimburse @defistaker for the 456 Euros server costs for GrinCC.mw site (once CC is able to sign transactions).


