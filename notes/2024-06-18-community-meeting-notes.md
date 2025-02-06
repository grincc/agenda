# Community Meeting Notes June 18, 2024

Community Council (CC) meeting held in keybase grincoin#general channel chat, meeting duration not explicitly stated, assumed to be around 30-45 minutes.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_

* waynegeorge
* anynomous
* cekic
* ardocrat
* phyro

# Short Summary

-   Discussion about the general activity of the Grin community and development teams.
-   Updates on ongoing projects such as Grin-GUI, MWixnet testing, Python Grin, and Grim Wallet.
-   Clarification on Grim Wallet's platform (native Rust app, not browser-based) and its future platform expansion.
-   Exploration of the Grin project wishlist and critical development needs, especially multisig and safe cancel transactions.
-  Update on safe cancel implementation status, noting it is a work in progress on the contract branch, not considered implemented yet.

# Agenda Points & Actions

*   General check-in on Grin development and community activity.
*   Discussion on active projects and their status.
*   Review of the Grin wishlist and critical development needs.

## Community and Development Activity

__wayne__: How's things with the Team in general?
I check in on the forum from time to time. I haven't used telegram for a while

__any__: Not very active in the case of the CC, but signing for milestone 3 of CoinSwap was fast and efficient.

__wayne__: In terms of active development, I think they are grin-gui, mwixnet testing, python grin. Is that right?

__any__: And also Grim wallet. Cross platform browser based wallet if I am not mistaken, do you know @cekickafa ?
Have not tested it yet, but the screenshots look good.

__cekic__: Not browser.it works on egui, Rust
Desktop ,android and ios coming..

__wayne__: Sounds really good

__cekikc__: It runs really smooth. Very good, thanks to @ardocrat

## Grim Wallet Details

__ardocrat__: Hello, yes it's native app in Rust, drawing triangles everywhere, even in browser, if it can be possible to compile wallet libs in wasm, currently I am working on release build in platform specific format for easy install (dwg, msi, deb) and patch storage for Android devices with low RAM amount, thx for testing.

## Grin Project Wishlist and Critical Needs

__wayne__: Is there anything that the CC are actively seeking developers for? Or is it a case of welcoming ideas? I remember there being a wishlist somewhere

__cekic__: There is wishlist since 2021 yes.

[https://github.com/mimblewimble/grin-pm/issues/385](https://github.com/mimblewimble/grin-pm/issues/385)

__wayne__: thanks. I found one on this page too [https://www.grincc.mw/projects](https://www.grincc.mw/projects)

__cekic__: That is the backbone of wishlist. As you see P1 section is critical/ must HAVES

__ardocrat__: multisig +1

__cekic__: i think these are core teams part, in the name for informing community about these wishlist items, multisig or safe cancel . Maybe they have word?

__any__: Safe cancel is WIP, only a test version implemented on the contract branch: See here a more up to date version of the Wishlist:
[https://github.com/grincc/hub/blob/main/wishlist.md](https://github.com/grincc/hub/blob/main/wishlist.md)
O and PIBD.

__cekic__: RFC looks open. i remember some fixes about it but there was sometihng double the amount after resending_ i couldnt recall.
[https://github.com/mimblewimble/grin-rfcs/pull/71](https://github.com/mimblewimble/grin-rfcs/pull/71)

__any__: Multisig is not implemented in any way.
(except 2 out of 2 multisig, basically every standard grin transaction is a 2 out of 2 multisig 😛)

__cekic__: In Gui wallet i remember tested cancel option but i dont have info contrat branch, not tested @waynegeorge

__phyro__: I did a quick proof of concept safe cancel on contracts branch, but it shouldn't be seen as implemented. It's an unfinished and unreviewed work for now.

+1 cek

## *TO DO List*


**Meeting adjourned.**