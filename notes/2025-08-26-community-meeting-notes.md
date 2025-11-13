**Community Meeting Notes August 26, 2025**

Grin Governance Council (GGC) meeting held in Telegram @ 22:30 UTC. Meeting lasted approx. 55 minutes.

Notes are truncated, and conversations are sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

**Community attendance:**

*   anonymous
*   Cole
*   Ckeci
*   Ardocrat
*   Alexander
*   Vladislav G
*   Wiesche


**Short Summary**

- The discussion reviewed follow-up items, including the slow progress on Grin++ peer issues and payment proofs.
- A major topic was the funding request for converting the Cuckatoo reference miner to Rust, with discussion on the approval process amidst low GGC member participation.
- Vladislav G confirmed he is ready to start working on the Grin MultiSig RFC.
- The bounty amount for the Umbrel/EmbassyOS Grin node was confirmed.
- The meeting concluded with a discussion on the ongoing challenges of managing GitHub organization permissions and repository access.

**Agenda Points & Actions**

Current meeting agenda https://github.com/grincc/agenda/issues/187


*   Follow-up on Pending Issues (Grin++, Payment Proofs, GitHub Org)
*   Funding Request: Cuckatoo Reference Miner Conversion
*   Grin MultiSig RFC Update
*   Funding Confirmation: Grin Node on Umbrel/EmbassyOS
*   GitHub Repository and Permission Management

**Follow-up on Pending Issues**

__anonymous__: We are on short supply of GGC members today.

# Follow Up.

- Fixing peers, grin++ node bans Rust nodes.
- Payment proofs fix.
- Grin Github organization.

Any news on these?

I can only say that I tried to setup the Github organization access to find out that ofcourse as regular member I do not have the permissions to add members.

__Cole__: I should start converting task ?

👍 wiesche, cekic

__anonymous__: If it is up to me yes, but I do not think we had enough GGC members official approve that task. Let me check.

__Ckeci__: Since last year still same. Peer problem and payment proofs...

__Ardocrat__: Payments proofs, will check at September, part of contracts branch, have some problems with keychain crate, will pick changes from this branch as discussed with Yeastplume privately.

👍 anonymous, wiesche

Nobody stops you from contributing bro

__Alexander__:
> Monero is mined using standard hardware like CPUs, so if the network were shut down, the hardware would still be usable for other purposes. In contrast, Grin relies on ASICs for mining. If the Grin network were to fail, those ASICs would become useless, resulting in a loss of the money invested in them.

## Funding Request: Cuckatoo Reference Miner ##

__Cole__: I set the milestone and shared to forum

👍 ardocrat, anonymous

__Ardocrat__: Open source Rust miner is must have

__anonymous__: @colasouda Regarding converting the mining software, in the thread I only see an 👍 from me, and I think from @johntromp although he does not explicitly say so.

We need more GGC to approve.

I can ask them in the GGC group to make their reply publicly on the forum. I see no reason to wait, they agree, or they don't but they should voice their opinion.

👍 wiesche

__Ckeci__: what if they dont?

__anonymous__: If they do not agree they should provide good arguments, so far we only have seen people cheering this idea on, no one saying it was a bad idea.

👍 wiesche, ardocrat, wayne

__Ckeci__: I dont see participation here. Forum votes count as much as key holders.

__anonymous__: They do. I think many are still in the holiday mode, myself included. Hence the participation of GGC members is a bit low at the moment.

__Ckeci__: No need to sideline with bureucratic mechanism still, this is publlic chat, proposals on public forum, staying silent and = obstructing means in my book.

__anonymous__: I just asked them, so I think we can soon expect their replies to this topic.

__Ckeci__: Not joining GGC meetings in a row is unacceptable and disrepect to community as well. More than 3-4 meeting missing without excuse should be enforced. Holding key and GGC member is a voluntary duty but that doesnt mean unresponsive like old CC.

__anonymous__: I think it is a bit early to say people are slacking off 😛. This is just holiday business. It is meant to be break.

__Cole__: I've received some positive responses, but there's no indication of any intention to get started yet.

__anonymous__: Lets move on to the agenda:

# Grin MultiSig #

__Ckeci__: i personally give you go ahead, and Tromp, anonymous, ardo and few members support it. So ignore the noise and start.

👍 nobodydntknow, wiesche, ardo

__Cole__: Got it
and then where should I push the code ?

__Ardocrat__: Waiting for @vlad_gelfer response, he said he is ready to start to work on Grin

__anonymous__: I think probably it is safe to start, but don't burn me if it is not.
Regarding payments, I think we can group the deliverables in two parts, and make two payments.
...assuming of course everyone will indeed agree to support this request.
The idea is that this is 4 weeks of work right @colasouda, so payments biweekly ?

__Cole__: No

__anonymous__: o, can you shortly reiterate how long you expect it to take approximately.

__Cole__: https://forum.grin.mw/t/request-for-funding-cuckatoo-reference-miner/12033/4

__Vladislav G__: I'm ready (more-or-less).
I understand, I should start from RFC or something similar, right?

👍 nobodydntknow, wiesche, anonymous

__Ardocrat__: Yeah, with document we can start implementation, I want to help as much as I can in Rust

👍 cekic, wiesche

__anonymous__: Yes, exactly. The RFC is needed to avoid wasting time, making sure the solution you work on is exactly what we all need and want.

👍 aglkm

I can help review the RFC, but only as an extra, I am not a real cryptographer.

__Cole__: Thanks, You are good at Rust ?

__Ardocrat__: Hopefully Tromp will come back


__anonymous__: I hope he can at least review the RFC he is one of the few people capable of reviewing that.

👍 wiesche

__Wiesche__: You get a yes from me

👍 cole,anonymous


__Ardocrat__: Also Beam has no Multisig, only at contracts level, I guess this development can be shared between projects..
💯 wiesche, anonymous

__anonymous__: Absolutely, Grin sees the bigger picture. Similar for the Rust reference miner, I see that as an investment not only for Grin but for the greater good of the crypto space and beyond.

👍 ardocrat

__Ckeci__: I pinged Tari admin and devs about it but they dont answer and refrain themselves using 'mimblewimble'' word

__Wiesche__: He is present in the forum

__anonymous__: Pinged them about MultiSig, or something else?

__Ckeci__: multisig. Explore the MimbleWİmble cooperation.

👍 anonymous

__Wiesche__: Sorry for the delay, first week at work is stressful.

👍anonymous, cekic

__anonymous__: No worries, glad you could join.
I think we can move on to our next agenda topic.

## Funding request Grin Node meets UmbrelOs, EmbassyOs ##

__anonymous__: https://forum.grin.mw/t/funding-request-grin-node-meets-umbrelos-embassyos/11928/7
Wiesche Did you count how many GGC members supported this?
Wait, was this not already approved 🤔

__Wiesche__: I started with the implementation.

👍 anonymous

__Ckeci__: Approved but bounty prize not decided.

__anonymous__: A... that was it.
A yes. I guess we have to make that a vote in the GGC channel. I think we did settle for 7.5K right?

👍 wiesche

Just to make sure no GGC members post delivery start saying they did not agree with the amount.
But I guess this will not be an issue.

__Wiesche__: We have proposed 7500 euros
Ok

 ## Code, Repos, and Access ##

__anonymous__: We already discussed the 3rd point on our agenda, the Request for funding Cuckatoo reference miner.

Is there anything more we need to discuss?

__Ckeci__: No, that is all

__Wiesche__: Sourcecode
https://github.com/wiesche89/grin-node-docker

__Ardocrat__: Good night

__Wiesche__: one Moment

Just this is good to hear. You are starting Vlad now, agreed?
Access mimblewimble git ?
And
Grim into mimblewimple repo
Also the miner
Also important for future work on multisig

__anonymous__: Arranging access to the mimblewimble git is up to any of the owners in this list.
https://github.com/orgs/mimblewimble/people

From those who have owner permission, I think yeastplume, Tromp are the only active ones. Phyro and Quentin might be available if really needed, but I think they took a break from Grin.
So, it is not something I can help arrange unfortunately.
Regarding moving Grim to mimblewible. I think this is something between @ardocrat and Yeastplume to arrange. I can understand if it is preferred to move Grim to the contract branch since this includes all great new things worked on.

__Wiesche__: There was a PR, who created it and who can merge/review it?
https://github.com/mimblewimble/grin/pull/3810

__anonymous__: I am not sure. I am only a team member for grin-pm, which makes sense since this is the part I want to work on. I think similar team assignments and permission should be given to all GGC members.
Perhaps adding more active owners would be wise, but I am not sure who. I am no Github wizard so I think it is fine for me to just be a member of grin-pm.

__Wiesche__: So it makes no sense to give other users owner rights?
Does anyone know ljluestc?

__anonymous__: No.

__Ckeci__: No.

__Wiesche__: Interesting
I might have I might have seen @DavidBurkett as well. At least then we can create repos faster and drive the administration forward

__Ckeci__: What matters is that code, is good for Grin, outside contributors had been before and will come also. If it is worth then review> merge.
You mean apart from Yeastplume @johntromp and @phyro and @quentin ?

__Wiesche__: We just need someone who can do it
Maybe you can have a look over it @ardocrat
Yes

__Ckeci__: Yes, we have github owners, normally they do it who has keys and capacity🤷‍♂️. Suppose that yoursel reviewed it and wanted it to be merged. It leads to same road.

__anonymous__: Ok, I am off. Thank you all from participating and please continue the discussions where needed
👋

__Alexander__: Comments are open to everyone. Anyone can review the PR.


👍 wiesche, cekic, anonymous

But that PR looks like AI generated

__anonymous__: If more would participate in reviewing, that might also more easily lead to owners merging PR's

__Wiesche__: True

__Ckeci__: So this anyone can be an outsider as well and approve also. What matters is trustable personas contribute i guess. Even the most old ones cant be tursted %100 anyway. So multiple people needed for review before merging. In theory 4 key holders defacto trusted and they also review before merging.
Ai is a fact anyway, people use it.




**TO DO List**
*  Fixing peers, grin++ node bans Rust nodes.
* Payment proofs fix.
* Grin Github organization.
* Multisig RFC

🔨 

**Meeting adjourned**
