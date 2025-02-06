# Community Meeting Notes April 9, 2024

Community Council (CC) meeting held in keybase grincoin#general channel chat. Meeting duration not explicitly stated, but inferred to be around 45-60 minutes.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_

* anynomous
* cekickafa
* anymous
* yeastplume
* trintiron
* tromp
* ardocrat
* renzokuken
* scilio
* phyro
* syntajax


# Short Summary

- Open discussion regarding various topics, including personal updates, a new web app using the Tradeogre API, and a new merchandise shop.
-  Discussion on consolidating Grin development channels and an update on the GUI wallet with an updated `iced-rs` library.
-  Debate about deprecating Tor support in favor of slatepacks and payment contracts.
-  Exploration of Gate.io's current HTTP transport method for Grin and its implications.
-  Discussion on the use of memos in slatepacks and potential solutions for exchanges.

# Agenda Points & Actions

*   No formal agenda was specified.
*   Discussion regarding Grin development channels.
*  Update on the GUI wallet using latest iced-rs.
*  Debate on the future of Tor support.
*  Discussion on Gate.io's withdrawal method.

## Open Discussion and Personal Updates

__anynomous__: No topics for today, so it's an open discussion. How was your day @cekickafa? My day was a bit tiring, running through endless Python environment issues.

__cekic__: Well, this month was extremely tiring for me because of social issues. Tomorrow is a feast here. I will return to normal :)

## New Web App and Merchandise Shop

__cekic__: Did you see at TG, some guy making a sort of web app using Tradeogre api?

__any__: No, that's new to me. Mmm, interesting. So a web wallet like [https://easygrin.org](https://easygrin.org) but with integrated buying and selling?

__cekic__: It looks like something.

__anynomous__: Which Grin channel is this exactly?

__cekic__: Main room. [https://t.me/grinprivacy/1](https://t.me/grinprivacy/1)

__anynomous__: Thanks, Also nice to have a new Shop for goodies: [https://www.redbubble.com/people/transatoshi/shop](https://www.redbubble.com/people/transatoshi/shop)

## Grin Development Channel Consolidation and GUI Update

__yeastplume__: We might think about rolling up some of these team channels, 'teams.gui_dev, node_dev, wallet_dev' etc. I realize I'm throwing updates into the gui_dev channel sometimes, and loads of people aren't even in it. Maybe we should just have a single 'dev' channel for everything for now at least? This is what I'm working on at the moment and why, by the way. I should have a new version of the gui out soon with updated iced-rs, which we need to be able to do stuff like enter seed phrases: .png
+scilio,phyro,ardocrat, sytajax

## Tor Deprecation Discussion

__trintiron__: @yeastplume Do you have a gut reaction to the notion of deprecating Tor out of Grin and going slatepack only? Now, next year, whenever. Just thumbs up or down to the conceptual direction.

__yeastplume__: I personally don't like the use of Tor that much anymore. I'd like to go towards slatepack + contracts and a few preferred ways of exchanging them. I don't intend on putting Tor support into the gui at the moment, anyhow. +hurra tirnitron

__anynmous__: If tor is dropped altogether, the main downsides would probably be that 1) Grin would be delisted by Gate.io and others and a few mining pools would stop and 2) it would decrease privacy, although perhaps users could simply use tor browser to interact with parties they do not trust to exchange slates.

__tromp__: My preference is slatepacks with payment proof and payjoin (except when sending to empty wallet obviously)

__yeastplume__: Yes, I wouldn't go out of my way to remove it without some sort of community agreement and RFC, but we can continue to develop other approaches that will hopefully become more popular. @tromp quote
agreed, this is what I'm working toward Then I'd like to see some more (completely optional) off-chain message-board/relay type approaches to slate exchange, like were being bandied about in the early days (like Grinbox)

## Gate.io Transport Method and Slate Memos

__ardocrat__: gate is showing http as transport method at withdrawal now, they dropped tor support before all maybe @cekickafa

+1 cekickafa

__cekic__: I am not sure if this is old httsp method but this section didn't exist before.

__ardocrat__: So I guess it's time to add HTTP transport to support gate xD HTTP is even easier, not needed to validate SSL certificate but not 100% anon for sure. Manual method is minimal and clear, not sure what is the problem for gate to add it


__anynmous__: Best for Gate.io to use slates, so users can withdraw with tor browser if they want to. I never quite understood what the real bottleneck is for exchanges to support slates. I mean they have user accounts, add a paste text box for slates, and you are done on the UI side, the rest is just a normal API call.

__ardocrat__: memo idea is not good here, they could use hd wallet and generate unique address, but they need to unite balances for large withdrawals with a lot of small deposits. slatepack has no additional info support for memo currently @renzokuken made some research here :) TradeOgre has no problems without addresses anyway.

__anynmous__: If I am not mistaken, slates have a memo field, you can put anything there, user ID, or message. The current Gate.io "memo" system should be called a transaction barcode or something, the name memo is confusing since it is just a hijacking of the transaction amount. Many small deposits to large withdrawals is no problem, they can run a self-spend now and then to merge those many outputs into a more useful distribution of output values at minimal costs.
+1 syntajax ,ardocrat

## *TO DO List*

* Discuss consolidate development channels.
* @yeastplume: Release a new version of the GUI with updated `iced-rs` library.
* Community members: Engage in further discussion about Tor deprecation.
* Community members: Discuss potential solutions for memo functionality with slatepacks for exchanges.



**Meeting adjourned.**