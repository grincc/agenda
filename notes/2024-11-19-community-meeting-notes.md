# Community Meeting Notes November 19, 2024

Community Council (CC) meeting held in keybase grincoin#general channel chat. Meeting duration not explicitly stated, assumed to be around 1h-45 minutes.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_

*   yeastplume
*   aglkm
*   trinitron
*   cekic
*   trab
*   anony

# Short Summary

-   Discussion about recent development efforts and new feature requests, including BIP39 passphrases, offline signing, Tor integration, and a seed checker.
-   Debate on the necessity and feasibility of a DEX for Grin, with an emphasis on improving core functionalities and privacy features first.
-   Discussion and vote to renew the Telegram bot bounty, changing the denomination to USD in BTC.
-   Initial discussion on a Grin seed signer bounty, followed by concerns about its complexity and necessary research.
-   A call for testing of Grin GUI with contracts workflow and setting up MWixnet nodes.
-  Discussion of MWixnet payment proofs and challenges with generating them.
-  Discussion of Grin GUI and its limitations, particularly data location.

# Agenda Points & Actions

*   Discussion of New Development Items.
*   Vote on Telegram Bot Bounty Renewal
*   Initial discussion of Grin Seed Signer Bounty.
*  Testing of Grin GUI contract flow and MWixnet nodes.

## New Development Items

__yeast__: I don't know if I'll be around for that, but I just wanted to point out that there's a lot of work gone in recently that I'm hoping other people will pick up on now. It should be easy to put together a test version of an mwixnet now after all the work done on putting together docker-compose files to run it, and the main branch of the wallet has been updated with new functionality to create mwixnet requests. I'm happy to see us coming out of a crypto winter, and Grin trading price going up for the sole reason that a better market price leads to a fairer and more secure network. At the moment I'm doing bits and pieces, but happy to have discussions about what people want to see next.

__aglkm__: Hey @yeastplume 👋 Since you asked about new development items for you. Here is the list of features I would love to see in Grin.
BIP39 passphrases. Holders have very limited ways to securely store their coins. Passphrase would help them to store seeds in a plain text without much worrying leaking it offline, since it will be protected with the passphrase.
Offline signing. This is another feature to level-up security of holding the coins. We need a functionality to be able to sign transactions, in a such way that we have a cold device holding a seed phrase and signing transactions and a hot device broadcasting these transactions without access to seedphrase. Such as seedsigner, krux, jade and etc. in Bitcoin ecosystem. I know we have ledger cold wallet for grin, but it's not implemented into core grin wallet and if such functionality is going to be added, then I would like see it working with the devices built on common hardware and communicating via QR codes.
Tor node. As I understand, Grin node is not able to run on tor network natively, so that would be a nice feature to have.
Tor mwixnet. As I understand, mwixnet is not able to run natively on tor network as well. Should be a useful feature for those mwixnet node operators wishing to run it privately.

__trinitron__: grintools seed checker fix if you can 😬

__aglkm__: I remember there was a website which allows you to enter IP and PORT, and then it tracks if your service is online, if not it will send you an email. Would that work for you? Or you want to track the health of all seed nodes in general?

__trinitron__: The seed checker is special because it confirms not just that the port is up but that it is responding to grin protocol requests correctly. I can check that myself by logging onto the nodes but the public checker is really convenient. Not necessary, just highly appreciated.

__any__: Working on a tool that also support BIP39 Grin wallets, only for experts. Yes, indeed we we are. Welcome, the agenda can be found in the link above, here copied again for convenience: https://github.com/grincc/agenda/issues/149 @trab_grin, the reason why we do it via chat is so it can be a) open for all, b) private for all since we can use whatever identity we want. is @cekickafa also around?

__cekic__: here i am

__trab__: Just with alt season coming up, I’m wondering if there’s something we can do to support improved liquidity. Maybe DEX development? I think Grim wallet is thinking about DEX integration maybe?

__yeast__: i've been thinking I might just add this functionality to the grin executable directly, like a grin seedcheck command or grin --testnet seedcheck.

__any__: That sounds very sensible. Better to include it in the node than adding a new tool.

__trinitron__: That's interesting and good if that's your preference but for me personally I just liked the convenient way to check my node from my phone from anywhere

__any__: Well, if its in the grin node, it can also be easily integrated in for example Grim wallet that runs on your phone.

__trinitron__: True. But I'm an iOS user 🙂

__yeast__: I'd like to decouple it from anyone in particular having to run a service somewhere, so if I put in there it should make it easy for any grin user to use and anyone could create a convenient service out of it as well

__trinitron__: Everyone's probably heard this from me by now lol but I don't think anyone will use a dex.

__anony__: The problem with DEXes and Grin is that as far as I can tell there is no really straightforward way to integrated Grin. Meaning some extra complexity will have be there, such as using BTC colletoral.

__cekic__: Dex is future.

__trab__: That’s fair enough. But seeing Haveno for Monero has definitely changed my tune on it. Once TradeOgre goes down, there is literally ZERO liquidity in Grin, right? Or is there another way to get it that I don’t know about

__anony__: Perhaps if the originally intended atomic swap for Grin can be implemented...

__yeastplume__: Make grin more useful and that will follow. Start running mwixnet nodes, collect fees. Make grin even more private, etc. +1 trab, anony

__trinitron__: TO delisting or disappearing could be terminal, yes. But imo a dex wouldn't change that.

__TRAB__: Yea, I also would like us to support Grim’s iOS development. Since IronBelly is out of commission now. Not sure how to help, but maybe we can at least pay a couple years worth of Apple Developer fees?

__AGLKM__: If it will be available via rpc call, I could easily integrate it into grincoin, so @trinitron will be happy 😁 +1 Any, trnitron

__yeastplm__: sure I'll think about how to do this.. it's not really core node functionality and it's a very expensive and intrusive operation, so I was thinking about leaving it way up the stack (as in the top-level grin crate,) but perhaps it can be added to the server's owner API as well

__anonym__: Probably we need to indeed just focus on the core for Grin as @yeastplume suggested and the rest will follow slowly. Good products tend to sell themselves. +1 trab

__trinitron__: iskin never responded to my pleas to take funding to maintain otherwise I'd be the biggest proponent for that. I have doubts about any other developer maintaining true to form it unless a really motivated and impressive one pops up.

__trab__: Ardocrat and Renzo both have their own ambitious roadmaps. Both seem interested in the long term +1 trnitron

__trab__: Ardocrat told me a while ago that he figured out how to get the Apple developer account. So theoretically we could just gift him some BTC to pay some fees. Just an idea +1 anynm

__trnitron__: In the end I do think a core windows client is actually important than iOS for adoption and use, so my hopes are really all in on grin gui now. I really need to try out the current version I haven't done so since early beta.

__yeastplume__: well, honestly grim is already much better than what I've been doing on grin gui

__trnitron__: And all respect for ardocrat but I'd have to see the prototype to believe it. iskin had a special understanding of the user experience imo.

## Telegram Bot Bounty Renewal

__cekickafa__: Since members are here. For the agenda, we better vote for Telegram bot bounty renewal. Sorry, diving in. Messages are coming late to me. Keybase :(

__anony__: Yes, still Gin GUI might come in useful one day, perhaps we should "Ice it", pun intended 😆

__trab__: Grim is still very early no doubt

__anony__: But yes, we are 21 minutes in and still need to start the agenda. Perhaps we can use these discussions to find topics for our next agenda.But yes, we are 21 minutes in and still need to start the agenda.

__trnitron__: @yeastplume I have an irrational affection for core clients is my problem. It's the trust level that comes with them.

__yeastplume__: Sure, well depending on how grim development goes, there might be an argument for auditing it and giving it 'core blessing' somehow, (but that's very theoretical at this stage) +1 trnintron, trab

__anonymous__: Ok, for our first official agenda topic for today:
1) Discussion Grin Telegram Bot.
Current status: https://forum.grin.mw/t/telegram-bot-progress-thread-by-renzokuken/9882/34
TL;DR, bounty of 10.000 Grin, status, development was halted due to some issues with the wallet API.

__trab__: I asked if the telegram bot would use Renz’ python sdk. Didn’t hear back. Wondering if it would be a rewrite to use that

__anonym__: Since then, the "invoice flow bug in the wallet owner API" has been fixed, so technically there is nothing stopping @renzokuken from completing the bounty. However, since then the value of Grin has tanked significantly, meaning the bounty is rather underwhelming now since we denominated it in grin and not in BTC or USD. +1 cekic

__trininron__: I have to oppose the Telegram bot on principle because I believe tip bots etc. come about organically to serve community excitement and it's cargo cult or cart before the horse to develop them prior to that. +1 trab

__anony__: @trab_grin No, the Telegram bot was designed to interact with grin-wallet. The API calls between grin-wallet and Grin++ are identical, only connection method differs. So in theory it should work both with grin-wallet or Grin++ wallet in the back, to my understanding.

__cekic__: I strongly support telrgram bot bounty renewal. Bounty is already there.

__anonym__: For now that is our main target, discuss making the bounty at least somewhat rewarding and attractive.

__cekic__: It is voted. It will be completed just.

__anon__: I think at the time of creation the bounty was worth a lot more, e.g. 2000-2500$ at least. Since we do not mine Grin anymore as CC, I would propose to this time make the bounty either a certain amount of BTC, or simply say a certain amount of $ in BTC.

__cekic__: yes

__trab__: Tbh I think it would be more beneficial if such a bot did run on the new Python SDK. It would serve to shore it up and prove it out. Of course it’s up to Renz or whoever how exactly it is implemented. But I agree with @trinitron it is cart before horse. When we can send slatepacks in telegram DMs, what is the point exactly?

__trnintron__: You can even send slatepacks in public chat! If the people don't mind the clutter. I think it's really cool though that you can transact in the open like that.

__cekic__: Did you ever read the bounty? This topic is set 2 weeks before, you better have to check it to give an opinion but you reject firmly.

__anonymous__: Let me explain, the Python SDK is now a wallet that can be easily called from within Python, but it does not have an API, it just runs as a library within Python where with direct calls you can create wallets and make transactions. So sure, the bot could directly talk to a python wallet, but having support for the API would be more beneficial IMO. Also because we need more examples of tools that run on the API.

__trab__: @trinitron What do you think would not be “cart before horse”? Wallets?

__trinintron__: Good question and yes, basically just wallets. I think the number one thing that needs to be ready for a newcomer is a reliable, endorsed, and trustworthy windows gui wallet for them to receive their grins that they got on Tradeogre.

__trab__: @cekickafa I am not firmly rejecting the bounty btw. By all accounts, the bounty has already been planned and agreed to. The CC should keep their word! I’m just saying idk if I would have approved it when it was originally set out

__@trinron__: Agree. Right now, it’s actually NOT a smooth experience to simply acquire Grin. And that’s the main problem +1 trinitron

__trinitron__: And to clarify my position: The 10k bounty exists so we honor it. But I oppose any increase based on my opposition to the concept.

__aglkm__: Just a reminder. CC has huge amount of funds and zero (currently) developers wishing to claim them 😉 +1 cekickfa, trinitron

__anonym__: Let me give an example of direct usefullness of such a bot. 1) it can answer FAQ questions, 2) direct people down the rabbit hole, 3) directly point aspiring devs to the right information, 4) Anyone who requests for example testnet grin could request a slatepack to the bot. All good and fun, but also usefull. Indeed, I get the sentiment and agree that the core functionality is actually more important, however we can afford some fun bounty projects. Also because they make good examples for anyone who wants to build a project on top of grin or grin-wallet.

__trab__: @aglkm There was seemingly no issue finding a developer for the telegram bot bounty. So do we just need to write up bounties?

__anony__: As far as I can see, it would be kind of sensible to just write the bounty in a better denominator, so @renzokuken can finish the project when he wants to without getting 0 in return. So yes, thats all, we just need to update the bounty.

__cekic__: I agree. Update the bounty.

__anonym__: @trinitron The bounty is 10k of grin, so now a value of around 300$. We intended it to be worth around 2500$. So that was the intend. IMO we can just switch it to a 2500$ bounty, paid in BTC using a 1 month moving average like we always do. Basically the choice to pay it in Grin was just not so well though through, especially with a bear market starting 🤣

__cekic__: Shall we vote? Enough members here now.

__anony__: I am ok with a vote. For me it is just an update of the denominator, we do not need to change anything to the bounty. But.... we can additionally request if he can make a version that also runs on mimblewimble.py. Just because it makes a nice example of a project that runs on Python. Does, 2500$ sounds about right? +1 cekic

__cekickafa__: Logical.

__aglkm__: @trab If it would be a random person just appeared in the community, then I would be neutral on the bounty. But funding @renzokuken would benefit Grin community long term.

__cekic__: For sure. He is a long term committed

__anonym__:Ok, lets just put it to a vote.

Please upvote or downvote the following use 👍 (yes) or 👎 (no).
Proposal: Nothing changes in the description of the bounty, only the denomination of the bounty is changed from 10.000 grin to 2500$ paid in BTC using a 1 month moving average. Additionally we will inform @renzokuken that it would be extra cool if it can run directly on mimblewimble.py, but only if he thinks his python package is ready for that.

+1 anony ,cekick,trab,yeastplume,aglkm, future3000, -1 trinitron

__trab__: Thank you for facilitating this so well @anynomous I know it’s not easy

__anony__: No problem, it is easy enough and motivating enough when others are around. If its only me and @cekickafa... well the motivation becomes lower over time, not that I do not appreciate your company @cekickafa 😉

__trinitron__: Yes iirc if I voted yes on it the first time that was contingent on the bounty being locked in grin.

__anonym__: Also, just good to mention non CC members can also vote @aglkm and @yeastplume , we do take all feedback into account even though only the CC votes are counted to get to the threshold for any spending decisions (4/6) 👍 are needed.

__yeast__: Speaking of bots I've actually been thinking about something more bold along those lines that might add some relevance to Grin, and I'd like to hear people's reactions, once there's nothing else in agenda.

__anony__: Sure, I am not sure if we get to that today. But I see @trinitron is against updating the bounty, can you elleborate why you are against it?

__trab__: @trinitron I totally understand. But also since BTC is up, the CC can spend less of it

__@anony__: Indeed, we can afford it.
Well. If needed we can put these voting results in the CC chat and see if we can get a 4th yaay there.

__trinitron__: A fourth can probably be found. I'm sure that I stay a no. As grumpy as I realize that is.

__anony__: Due to lack of time we finalize the vote in the CC priority Telegram chat. For now we move to the second and last agenda item.
We will just refer to this discussion, then the other CC members can make a well informed decision.
Our second agenda item
2) Grin Seed signer Bounty discussion.
https://forum.grin.mw/t/grin-seedsigner/11371
TL;DR, we want to work towards a bounty for a SeedSigner that supports Grin. Everything is DOI in Hardware, software is Open Source, so it could be a great addition for Grin as HW wallet.

## Grin Seed Signer Bounty

__trab__: iirc, there was work done on hardware wallets in the past and it got literally zero usage +1 trinitron

__trinitron__: I'm gotta go drive to get lunch now so I'll spoil the surprise right away: I'm a no on the seed signer bounty. Same reasons as always. +1 anonym

__anonyms__: Mutliple components of such a bounty, such as SeedQR, we can reuse for things like Grin paper wallet, grin-vouchers etc. I actually agree with @trinitron that I do not expect a SeedSigner to be a game changer, but still, its cool, its realist and much easier to implement if you ask me then for Ledger or Trezor,. I only have some technical concerns, maybe @yeastplume can shed some light on them.

__trab__: That’s cool, but isn’t that stuff more used after the basics get so good people get bored and want to tinker? I just don’t think we’re at a point where we have such a good UX with the basics that we want to tinker on random things

__yeastplume__: I like the idea of seed signers but bounties are hard. Software (and hardware/firmware) needs commitments to be maintained actively, and bounties don't address that at all.

__trnitron__: One can already theoretically transact from an airgapped computer right? You use the offline computer to generate a wallet and then receive a slatepack by manually typing it back and forth. Then you destroy the computer and you have a paper wallet. Just a lot of effort and you have to trust that the system works cause you never get to check the balance in the client.

__anonym__: My main concerns are 1) Grin wallet is interactive, is easy to link a hardware wallet with software wallet and share pubkey or other system to scan the chain? 2) libsecp256k1 v0.6.0 now has MuSig2 Support, does this work for Grin? The reason I am asking is because it might make sence to make a SeedSigner a 2 our of 2 MultiSig for Grin.

__yeastplume__: Also, technically don't forget grin's signing process is multi-party and involves complicated primitives that aren't used elsewhere. Offhand I'd say this is a non-trivial undertaking though I haven't looked into in specifically

__anonym__: See my questions above @yeastplume So yes, those are basically my concerns.

__yeastplume__: Right, so offhand I'd say it needs research +1 anonym

__anony__: So 1) you have the challange that you would need to sign also receiving transactions using SeedSigner, 2) you need to somehow communicate enough information to the software wallet to scan the chain (Pubkey or rewind hash... I wish I understood those better).

__cekic__: Seedsigner is a must for merchant adoption. Qr codes, payment with it. Airgapped..

__trab__: What makes you say that? Most bitcoin merchants are just using BTCPay server and that’s it. Or a third party handles it all

__aglkm__: @trnitron And when you are going to spend the funds or accept other funds, you will have to connect the wallet and node, so your cold wallet is not that cold anymore. Cold storage is essential for holders, without it do not expect people take grin seriously.

__anonym__: Transmitting Slatepacks through QR codes completely makes sence if you ask me, also its trivial. The real challanges are the ones I outlined above. Not sure if it is easy to send for example a rewind hash to your software wallet, also I still do not understand why pubkeys do not work for Grin. I though pubkeys or part of it were embedded in the range proofs, allowing a wallet to scan for outputs belonging to it.

__trab__: So maybe just table this for a while

__anony__: In any case to summarize my opinion on SeedSigners and a bounty for it.
1) Yes, I would like to see one (in the future)
2) I think Seedsigner fits and makes sense for Grin
3), We need to do more research, also because we really really cannot say how much work this actually would be right now...

__yeast__: there's data in the rangeproofs that can only be read if you have the owner's seed

__anony__: Crap, pardon my English

__yeast__: mostly to avoid the need to grind outputs to find yours when restoring a wallet, though it's not core to the protocol and it's possible to create outputs without that info

__anony__: Is it a single piece XORed for all range proofs, or unique per output?

__yeast__: there's a few bytes of data xored, I'd have to remind myself of the exact structure

__aglkm__: @yeastplume But we have ledger for grin... Could the work done there be useful?

__yeast__: yes, it could. But a bounty would not be the way to do this (or any significant research/development in my mind)

__anonym__: Basically, the question is. Can it be derive in some way (e.g. pubkeys) and shared safely without leaking the seed....

__trinitron__: @anonym Yes, very useful and very trivial. Just waiting for organic interest to bring that into existence someday. I pre-oppose any bounty for it lol.

__yeastplume__: agreed.. Grin will survive all crypto winters until that happens pray trinitron

__aglkm__: @triniton: what is the reason of opposing it?

__trinitron__: Cart before horse. When the time comes, these things will get done just for fun. @trab +1

__yeastplume__: can't say I disagree with that sentiment.. when Grin's use becomes evident, these things will follow

__anonym__: Some parts of it yes, but a significant project requires significant dedication of time and resources, not everything needs to be completely free.

__yeastplume__: also agree with that. it's complicated.

__anonymous__: Let me say it in another way. I do believe in organic growth, but no I do not think there will be outside financial stimulate for major projects, so going somewhat halfway and at least compensating people for there efforts to some extend is not wrong.

__trab ginr__: We don’t even have a wallet with a smooth payment proof UX…
laugh: trinitron

__anony__: Yes,... those are actually more pressing issues 🫣

__trab__: The only thing the CC can do is provide incentive. We can show our priorities by showing what we do and do not incentivize

__yeastplume__: I'd like to see someone from the community focus on getting a mwixnet up, I think that would be more useful to the core experience.

__aglkm__: @trab UX Yes! I forgot to put that into my wishlist of features for @yeastplume Another essential functionality for grin wallet. As I understand, so far we can generate proofs if we use Tor grin address, but for manual slatepacks there's no way to generate it.

__Anony__: That is indeed important. @yeastplume Perhaps you can make a public call for it on the forum with links to the relevant documentation. @yeastplume Is it true that when purely sending slatepacks you cannot generate a payment proof?

__yeasptlume__: The contracts branch of the wallet has V2 payment proofs, and they can be generated in any instance. @anony I'd need to check what the cause of this is, it's been a while

__@anony__: It does not matter as long as the contract branch will go main soon, but... wil it?

__yeast__: But the contracts branch isn't in wide use... correct. Well, not without more interest and testing

__anony__: I thinkt its a bit chicken and egg there. What I mean is, testing starts when its released on the world. I did not know it was waiting for more testing.

__yeast__: it's been all egg and no chicken the past few years (or vice-versa, I guess). As I say, I'm hoping we're emerging from a crypto winter now

__trab__: If we had a core grin gui wallet with the latest transaction flow…. that would be so nice

__yeast__: we do have one if you install grin-gui and select contracts workflow from the settings tab

__anonym__: Maybe we can make two for  calls. 1) for testing Grin GUI with contract flow and 2) One for setting up MWixnet nodes. And @cekickafa we can include those in the newsletter.

__yeast__: That would be great, yes.

__cekic__: ok.noted.

__anonym.:__ Does Grin GUI also have a console to interact with? I cant remember.

__yeast__: no, the base wallet package has all the console you could ever want though

__trab__: Does it allow you to specify where to save the data? I can’t use it if it will only use my C: drive for example :/

__yeast__: You should be able to link any wallet directory to it (but again there's a lot of testing that hasn't been done)

__anony__: I know that sounds contradicting, but I love wallets that like Bitcoin Core are both visual and have complete console. Its something I miss in Grim wallet as well.

__trab__: Grim wallet is awesome, but I think Ardocrat just wants freedom to implement whatever they feel like. Understandable +1 cekic

__anony__: True, but I think he is open for request/suggestions.

__trab__: Is contract V2 intended to be the new default moving forward? After testing I mean

__anony__: Hopefully with the coming bull market more people are interested and flush enough to dedicate some time testing for Grin. For me I always envisioned contract flow to become the new default. Just because it simplefies things, universal payment flows, universal payment proofs, safe-cancel. No more SRS and RSR discussions, ... I might miss them though. O and it better fits complex features like multisig.

__yeast__: I need to head off, but good discussion so far, hopefully we can keep it going over time

__cekic,trab,anony,aglkm__ +1


## *TO DO List*
* Testing Grin GUI with contract flow.
* Setting up MWixnet nodes.
* Announce on newsletter about GUI and Mwixnet testing by community.

**Meeting adjourned.**