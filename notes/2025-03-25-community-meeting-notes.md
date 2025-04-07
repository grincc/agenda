


# Community Meeting Notes March 25, 2025

Community Council (CC) meeting held in Keybase, starting around  19:30 UTC lasted approximately 52 minutes.

Notes are truncated, and conversations are sorted based on topic but not always strictly chronological. Quotes are edited for brevity and clarity.

### _Community attendance:_

*   anonymous
*   ardocrat
*   bobo123grin
*   cekickafa

# Short Summary

*   Discussion centered on the need for more active Community Council (CC) members and
  The funding request for the Groundskeeper (@cekickafa) was discussed.
*   Concerns were raised about the burden placed on the few active CC members due to inactivity from others.
*   Peers ban issue between Grin++ and Rust nodes,general P2P stability needs.
*   The Payment Proofs implementation is currently blocked by a bug (@yeastplume is aware).
*   @anonymous provided an update on wallet development challenges after dependency updates.

*   The status of the `grincc.mw` website hosting was briefly mentioned as needing clarification.

# Agenda Points & Actions

*   Donation payment to [Grincoin.org](https://grincoin.org/)
*   Groundkeeper [voting for funding request](https://forum.grin.mw/t/cekic-progress-and-request-for-2025-groundskeeper/11615).
*   CC governance Proof of Live check.
*   Fixing peers, grin++ node bans Rust nodes.
*   [Payment proofs](https://github.com/mimblewimble/grin-wallet/issues/730) implementation.
*   Anonymous dev update for
    *   _PR Fix for many wallet config Error_
    *   _Initial sync fine tuning and speed-up_



__bobo123grin__: good wishes for green cross the Great Wall from mainland.china,and all the best for grin user

__anonymous__: Best wishes to all our Chinese community members

## 1. Donation payment to Grincoin.org

__anonymous__: To my knowledge no one responded to that except for Mokhtar... We need at least four of us to sign, where is @futura3000 these day? ... Bottom line, we need more active CC members and more active key members... [Grincoin.org] is quite nice, it at least (if not more) deserves the very modest donation for which we have drafted a transaction.

__cekickafa__: yes, he is the one only responded so far. And you.

__bobo123grin__: Agree first agenda... I am checking grincoin.org ,it is my first time... Yes [agrees it deserves donation].

## 2. Groundkeeper voting for funding request

__anonymous__: Regarding funding for @cekickafa, this is quite inconvenient again to have so few active CC members... If you agree with the funding of our groundkeeper, can you say so in the forum thread https://forum.grin.mw/t/cekic-progress-and-request-for-2025-groundskeeper/11615/20

__bobo123grin__: Agree... Ok,I say something in forum for groundkeeper.

## 3. CC governance Proof of Live check

__anonymous__: Here is my problem, the less active CC members there are, the more the burden is on those few active, mainly me and @cekickafa... this is not something I want to spend too much time on... I do not want to spend my energy to police other CC members... It certainly is problematic if it is long term... We could make a forum thread to at least be public about the situation, but again, I simply do not have the energy or motivation... TLDR; Yes it should not be long term, but there is nothing much we can do about it. It is up to those CC member who chose to go dormant to reactive themselves.

__cekickafa__: It is not necessary to retag names; however, it is apparent that they are either busy or disengaged from Grin-related governance. While we cannot enforce them, this situation is problematic.

## 4. Fixing peers, grin++ node bans Rust nodes

__anonymous__: @ardocrat Do you know more about this? I had the issue in the past, but last time I checked it was no issue... Yes, [Grin++ devs] should come back. What is also weird is that those before active in Grin++ Telegram now tell everyone to move to Grim. This is not good, a balance between the two nodes is preferred... While Grin++ is indeed a bit too strict in banning peers... grin rust nodes are too lenient... Header sync is also very weird, the more peers, the slower it gets.

__ardocrat__: Every time. Also checking at p2p server how much g++ peers are in DB, its very low amount... We need Grin++ devs to come back simply or call someone from outside… Miners are using Rust nodes... We need to have stability at Core implementation as well, I am personally coming back to active development at April, so we can integrate contracts flow at GUI and fix weird p2p bugs.

## 5. Payment proofs implementation

__anonymous__: Payment proofs are in the Contract branch, so it is all about testing the contract branch, which is now stuck on a bug: https://github.com/mimblewimble/grin-wallet/issues/730 ... @yeastplume indicated that he would look at it, so for now I will do nothing... Indeed, I think we can just wait till he looked at a fix for it.
__ardocrat__: Grincoin.org founder created issue with proof at contracts, Yeastplume is aware.

__cekickafa__: [Links issue] https://github.com/mimblewimble/grin-wallet/issues/730

## 6. Anonymous dev update

__anonymous__: PR Fix for many wallet config Error / Initial sync fine tuning and speed-up: After I updated the dependencies, one part of my fix is not working... I can probably fix it but it means I have to make a lot of changes again... In general, I think I have been trying to be too nice not to make any large changes while in some cases it is best to break away from past design decisions... not everything in Grin's code base is perfect, nor is Rust everywhere as stable as I would have expected before.

## Chinese UI Translation Initiative

__ardocrat__: I think we will also need Chinese translation of UI, this task can be rewarded easy... We have translations at separate folder https://github.com/GetGrin/grim/tree/master/locales You can just open en.toml file and replace values with Chinese language... zh.toml I guess.

__bobo123grin__: I want to do some things for grin. be helpful for Chinese translation of UI, no need for rewarded... I will make a try... Pleasure to help.

__ardocrat__: Thank you, contact me if you have any questions.

__anonymous__: Is this something you would be willing to help with @bobo123grin ? ... @bobo123grin 谢谢你 :pray:

__bobo123grin__: Ok. be willing to help, thank u for your contributions.

## Other Updates, GrinCC Website)

__cekickafa__: @bobo123grin you know @xiaojay , Niffler wallet developer, he is a long time Grin contributor from chinese community. Recently i contacted him, he is busy atm but he says he is still involved with Grin, he will contribute... if you have questions, he can help also... he has TG [Telegram] i can DM [Direct Message] if you like.
__anonymous__: That is good news.

__ardocrat__: Nice to hear, he made good project before https://github.com/xiaojay/grin-map

__bobo123grin__: I don’t know xiaojay... Do you have a e-main or WeChat of xiaojay? I want to contact him... I don't have TG, What does the meaning of DM?

__anonymous__: @bobo123grin DM stands for Direct Message.

__cekickafa__: So there is grincc.mw issue also... the person in c
harge of hosting administration has changed. @future3000 has the accesss imo. https://github.com/stakervali/grincc-next, it is updated.

**bo123grin** leaving too tahnk you all



ardocrat,pirategrin,bobo123grin.
👋

**cekic** thnks all.





**Meeting adjourned.** 

## *TO DO List*


*   **CC Members:** Vote/comment on @cekickafa's Groundskeeper funding request on the forum thread.
* Fix payment proof/contract bug (#730).
*  Resolve `grincc.mw` hosting administration/access issue.












    



---