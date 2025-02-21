# Community Meeting Notes January 28, 2025

Community Council (CC) meeting held in a Keybase chat. Meeting duration not explicitly stated. Open agenda format.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_

* waynegeorge
* cekickafa
* anynomous
* trabgrin

# Short Summary

- Open discussion regarding Grin GUI (Grim) development, payment proofs functionality and UX, a funding proposal for PIBd implementation, learning Rust and bug fixes for grin-wallet, and the potential for decentralized exchanges (DEXs) with Atomic Swaps.
- mimblewimble/docs repo update

# Agenda Points & Actions

*   Open discussion, with topics emerging during the meeting.

## Grim and Payment Proofs

__waynegeorge__: I can't find the agenda doc

__cekickafa__: [https://github.com/grincc/agenda/issues/154](https://github.com/grincc/agenda/issues/154)
+1 waynegoerge

__anynomous__: Its an open agenda today, so any topics are welcome.

__cekickafa__: No topic added. Open discussion

__wayne__: Cool. What were @ardocrat 's ideas around Grim about?

__anynomous__: I do not think he is around.
Did he say anything on Telegram about his plans? I know he wants to rework the design of Grim a bit. I have to wait for that before I give more detailed turorial instructions in the Grin docs.
All pending pull request were merged for grin docs, except one since I did not agree with the requested changes

__wayne__: Also. I've heard missing payment proofs being mentioned on the forum but I thought that they were implemented
[https://github.com/mimblewimble/grin-rfcs/pull/31](https://github.com/mimblewimble/grin-rfcs/pull/31)

__anynomous__: I think the new payment proofs are implemented in the contract branch, but maybe there is some bug that the senders tor address is not properly provided to the payment proof function.
I might be wrong, but I think it is a quite small thing, the functions are there, just some mistakes in how the parameters are handled.
O, the payment proofs from Burket are different.
They work great, but the problem was it did not work for RSR (so receiver initiated payment flows).
Hence a switch to the new payment proofs:
[https://phyro.github.io/grinvestigation/bidirectional_paymentproofs.html](https://phyro.github.io/grinvestigation/bidirectional_paymentproofs.html)

__wayne__: Thanks for clarifying that

__trabgrin__: It’s also about the UX for proofs. It should be a very common use case to both retrieve an old proof and send it to someone and to input a proof you’ve been given. For a private currency, this is a very important and foundational user journey

__anynomous__: It is, I was surprised they were not working everywhere by default.
Sure, we do not have many stores yet excepting grin, but that it not actually the point, in all cases you should have proof by default.
I think also in Grin++ they are not on by default, does anyone know?

__trabgrin__: As of now, I think people just rely on the fact that Grin is not often used. So they can say “I sent you 47 grin last week” and the other user can say “yeah i see it”.
But that doesn’t cut it in the real world, so to speak

__anynomous__: Indeed, it should just work. Andi in GUI they can simply put an extra question to the user for any incomming as well as outgoing payments (contracts), "do you want a receit/payment-proof".
+1 trabgrin

__anynomous__: Anyhow, we are close to that I think. Just need to fix the reported bug, @ardocrat for sure would not mind integrating payment proofs properly when it works in grin-wallet..
@cekickafa There is one #TO DO to add to the minutes, we have to pay bluimes for the explorer, I keep on forgetting.

__cekickafa__: yes, noted.
+1 anynomous

## PIBD Implementation, Rust Learning and Bug Fixes

__anynomous__: Apart from initiating this Funding Proposal:
[https://forum.grin.mw/t/funding-proposal-pibd-implementation-in-grin/11583](https://forum.grin.mw/t/funding-proposal-pibd-implementation-in-grin/11583)
I am taking it a bit slower with governance since I am trying to get into Rust and bug fixes for grin-wallet

+1 ardocrat, cekickafa

__cekickafa__: very cool.

__anynomous__: For now I am still quite useless since I am still learning both Rust and the wallet code, but I think I might become adapt enough over time to handle small bug fixes and small changes in the code.

## Decentralized Exchanges

__waynegeorge__: What do you guys think about DEXs? I remember the BISQ exchange not having much interaction. I do wonder whether having atomic swaps on a coin such as Solana may bring some more interest

__anynomous__: Atomic swap would be great. I think the best thing would be to have it with either Bitcoin as chain, or a chain that specializes in Swaps, like Bisq, Like Komodo, Like Verus. I am not sure if Solane is a good chain for that. Also Monero was working on a Dex I think, but I am not sure how far that is in development.
The main problem is that we need a good cryptographer to take that on. The idea was there, I think gene started working on it, but he chose a different design than the one that was requested and specified by Tromp.
I have to go now, I will read up later
bye +cekickafa, trabgrin, waynegeorge.

**Meeting adjourned.**

## *TO DO List*

*   Cekickafa: Draft payment for Grincoin.org  explorer donation.
*   Anonymous: Review and update mimblewimble/docs.