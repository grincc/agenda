# Community Meeting Notes September 24, 2024

Community Council (CC) meeting held in keybase grincoin#general channel chat. Meeting duration not explicitly stated, assumed to be around 30-60 minutes.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_

* cekic
* anyn
* aglkm
* findfood

# Short Summary

- Discussion regarding the status of Niffler wallet.
- Agreement to potentially remove Niffler from the main Grin website, while keeping it on the GitHub hub with a warning.
- Update on @cekic's Grin-related project, with parts on order.
- Detailed update from @anynomous on his "Grin Wallet Tool" project, including features for various wallet types and output formats.
-  Idea of "voucher wallets" as a key feature of the tool, enabling easy "gift card" style transfers.
-  Enthusiasm about the potential for easy interoperability with Grim Wallet via SeedQR.

# Agenda Points & Actions

* Discussion about Niffler wallet maintenance and its future.
* Updates on community member projects.
*  Detailing of "Grin Wallet Tool" project and its features.

## Niffler Wallet Status

__cekic__: Hi, anonymous. U tried ever niffler on windows? It works also with external node option. Last updated to v5.0 node. Do we need to remove it?

__anyn__: I think I installed it in the past, but never active used it since I was hooked to Grin+.
I am not sure. If it would come with an updated node it could still be used.
it would not be too much work, but I think @xiaojay has no plan to update or maintain it.
What do you think?
One argument for removing it is because the seed_node list is outdated, meaning that if you download it now you can find zero peersI think I installed it in the past, but never active used it since I was hooked to Grin+.
I am not sure. If it would come with an updated node it could still be used.
it would not be too much work, but I think @xiaojay has no plan to update or maintain it.
What do you think?
One argument for removing it is because the seed_node list is outdated, meaning that if you download it now you can find zero peers

__cekic__: I didnt know that. I used it wirh grinnode.live and grincoin.org. It was working.

__anyn__: Which would be a bad first user experience for grin users. Perhaps we can contact @xiaojay to ask if and what his plans are for niffler.
Updating it with the new node should not be a big issue, but for some weird reasons my PC has troubles with the wallet talking to the node, so it is not something I can test.

__cekic__: Ok. Let me try it then.

__anyn__: On [https://github.com/grincc/hub/](https://github.com/grincc/hub/) we can leave it, but add a warning that you need to update the seed list or use grinnode.live.
I think for the main page, if we or @xiaojay cannot update it, we should remove it simply because otherwise you get first users trying and then abandoning because of the bad user experience.

## Community Project Updates

__anyn__: @cekickafa how is your grin project coming along?

__cekic__: I ordered some parts. Waiting them to arrive.Hoe is yours ?

__anyn__: I outlined the plans for my little grin project.
[https://github.com/Anynomouss/grin-wallet-tool/](https://github.com/Anynomouss/grin-wallet-tool/)
I will put the first code soon.
My PC does have a working node but not a working wallet, because of some weird API issues the wallet cannot talk to the node. That is a bit frustrating since it makes it harder to test. The last week I mostly overhauled the general ideas of how to implement the code.
When it is done it will be a lot of fun I think. The tool will unlock more advanced wallet options:
    1. normal wallets
    2. bip39 password protected wallets
    3.  voucher wallets
    4. brain-bip39 password protected wallets
And will allow output of wallet files, mnemonics or SeedQR. So it will be possible to generate any of these type of wallets and just load by scanning the QR code.

+1 aglkm findfood

## Grin Wallet Tool and Voucher Wallets

__cekic__: Voucher wallets interesting. Like gift cards?

__anyn__: Yes, indeed . And since you can output them as a QR code, someone can just scan and swipe them to top up their wallet.
The tool also will have a load and deposit option, so you can generate a wallet in one command and either load grin funds on them directly, or swipe them to your main wallet. So it is like a AddOn to the normal Grin wallet.

__cekic__: Cool💛 Well thats a feature really. Top up like gift cards. Very good for daily real uaagw
*usage

__anyn__: I think so as well, also it just makes using Grin a lot of fun! I think people often forget that that is a very important aspect of any crypto project 😁
It is also nice since Grim wallet is planning to implement SeedQR, meaning you can create a wallet with this tool and just import it in Grim with a single click.. So when Grim implements this, vouchers will be really easy to use. No need even for normal users to use my tool. Advanced users can generate vouchers, regular users only Swipe them for funds.
I have to go now unfortunately.

## *TO DO List*

*   Test Niffler wallet, focusing on external node connection.
*   Contact @xiaojay regarding the future of Niffler wallet.
*   Community: Further discussion on how to promote easier usage of Grin for daily transactions.

**Meeting adjourned.**