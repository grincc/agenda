# Community Meeting Notes May 7, 2024

Community Council (CC) meeting held in keybase grincoin#general channel. Meeting duration not explicitly stated, assumed to be around 45-60 minutes.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_

* anynmous
* wayne
* scilio

# Short Summary

-  Updates on the completion of MWixnet Milestone Three, with pending funding release due to minor test failures on Linux and macOS.
-  Discussion about a new open-source block explorer.
-  Discussion about the inner workings of MWixnet (CoinSwap) 

# Agenda Points & Actions

*   Updates on MWixnet, block explorer, mobile wallet removal, bulletin board, and static site.
*   Discussion on MWixnet and interactive crypto in general.

## Community Updates

__anynmous__: Let me start with a few updates, for whoever missed them on the forum:
Updates:
1) MXixnet, milestone three completion. Release of funds is pending on the vote and some last issues compiling and running one test.
Windows ✅
Linux ❌ (one test fails)
Max OSX ❌ (one test fails).
These test issues are minor, so should be solved any time assuming Scilio has time.
2) Very cool new block explorer, thanks to Bruges [https://forum.grin.mw/t/grin-bulletin-board-discussing-four-options-and-select-one-for-bounty/9822/34](https://forum.grin.mw/t/grin-bulletin-board-discussing-four-options-and-select-one-for-bounty/9822/34)
-OpenSource, Dashboard showing supply, relative supply, fee per block, fee per hour, mining profitability – Link to raw block data, searchable by kernel or block number
3) No more mobile wallet in Appstore 🥲 [https://forum.grin.mw/t/no-more-grin-wallet-available-on-google-play/11046/4](https://forum.grin.mw/t/no-more-grin-wallet-available-on-google-play/11046/4)
4) Bulletin Board discussion added a fifth option, the transaction "Buddy System" 👅
[https://forum.grin.mw/t/grin-bulletin-board-discussing-four-options-and-select-one-for-bounty/9822/34](https://forum.grin.mw/t/grin-bulletin-board-discussing-four-options-and-select-one-for-bounty/9822/34)
5) Created a static site, explaining Grin for programmers and visual thinkers – work in progress: [https://anynomouss.github.io/grin-for-muggles/grin_for_muggles_and_aspiring_wizards.html](https://anynomouss.github.io/grin-for-muggles/grin_for_muggles_and_aspiring_wizards.html)

__wayne__: Amazing

## MWixnet (CoinSwap) Discussion

__wayne__: Is MXixnet the same as coinswap?

__any__: yes, it is. It all works when I test in on Windows. I tested on Ubuntu and on NixOS, everything works except one e2e test.
Johh tested on MacOSX, he has the same test failing. So that needs to be checked by @scilio

__wayne__: I'd love to see how that works.

__any__: Me to. To be honest, I never really got the time to look in detail how the crypto behind it works, I just understand enough of it to see that it is rather amazing since only one mix node needs to be trusted, and the mixing comes with no additional cost as far as I can see. Well, one kernel per day cannot be deleted since it involves many outputs, but that is only 100 bytes a day😛 Really amazing crypto, only possible because Grin is interactive.

__wayne__: I watched a video this morning of someone demonstrating a bitcoin coinswap proposal with a decentralised protocol. In opposition to the Samauri wallet shutdown
Perhaps the grin community could make some demos

__any__: Interesting, the Samurai swap issue is bad news for Bitcoin. Thank god (crypto gods), that Grin has so much better privacy by default.
In a distant future, Bitcoin could go extension blocks and just have Grin/mimblewimble for all its magic in this extension blocks.
This would however still be inferior to Grin itself, since Grin has more to offer, its minimal, fair etc. So in a way you could say Grin does not really need Bitcoin to make it interesting.
Recently I am spending less time on governance and more diving down the Grin crypto rabbit hole 🐇 🕳️ 💊 .
The more I learn, the more I realize how awesome interactive crypto is. Still so many use cases to explore.

__wayne__: It seems that privacy coins are no1 enemy to the states so I expect a lot more resistance in future

__any__: Perhaps. I think it is a good thing that grin will not be the number one enemy of the current system of fiat and those who like to control everything.
As long as Monero and Zcash have slightly better privacy (even though at great chain cost, complexity cost etc.) Grin can just do what it wants and needs to do, be good fair, fungible, privacy preserving digital cash,

## MWixnet Test Failures and Implementation Details

__scilio__: I'm still looking at it. It's not clear why it's failing. It fails when calling into grin-wallet, so I'm not even sure which project needs fixed.
I expect to have it figured out soon though
+2 any, wayne

__any__: Ok, if there are more ways I can test or provide more explicit error information, let me know @scilio
+1 scilio

__wayne__: As it stands, is the coinswap only useable in grin-wallet? So it'd be command line based?

__any__: Yes, to my understanding it is only possible in this way because Grin is interactive.
But I have to admit I really should investigate more the inner workings, perhaps @scilio knows better if it could work for Bitcoin.

__wayne__: I think a gui version would be most helpful to learn what goes on

__scilio__: Right now, I have it coded so that the mwixnet server operators would use grin-wallet, but consumers could use any grin wallet
+1 any

__any__: But it cannot work for something like Bitcoin right?
I mean it rellies on interactive crypto as far as I understood it.

__scilio__: It doesn't rely on interactivity. It just relies on the structure of grin transactions (i.e. the pedersen commitments)

## *TO DO List*

*  @scilio: Investigate and fix the MWixnet test failures on Linux and macOS.
*   Community: Discuss and propose ways to improve the user experience of MWixnet, possibly including a GUI version.



**Meeting adjourned.**