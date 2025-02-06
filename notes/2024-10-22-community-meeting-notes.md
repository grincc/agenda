# Community Meeting Notes October 22, 2024

Community Council (CC) meeting held in keybase grincoin#general channel chat. Meeting duration not explicitly stated, assumed to be around 30-45 minutes.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_

* anynomous
* cekic
* yeastplume
* jdavies (mentioned)
* ardocrat (mentioned)
* syntajax (mentioned)
* circusdad (mentioned)
* natsuni (mentioned)

# Short Summary

-   Update from @anynomous on his Python wallet tool development, noting progress and the potential benefits of slatepack support in `mimblewimble-py`.
-   Discussion about SeedSigners for Grin and the challenges of offline wallet functionality and cost.
-   Update from @cekic on DIY SeedSigner assembly and the need for better bulletproof multisig for a Grin-specific SeedSigner.
-   Update from @yeastplume on integrating MWixnet comsig code into the master branch of `grin-wallet` including the json-rpc API.

# Agenda Points & Actions

*   Update on personal Grin projects and development.
*   Discussion about SeedSigners for Grin.
*   Status update of MWixnet integration in `grin-wallet`.

## Python Wallet Tool and SeedSigner Discussion

__any__: No agenda for today. So I will just give an update, anyone can chip in about what they are doing/Grin related or not.
I have had little time lately but still am working on my Python wallet tool when I can.
[Very much work in progress] [https://github.com/Anynomouss/grin-wallet-tool](https://github.com/Anynomouss/grin-wallet-tool)
Renzokuken has released a new version of mimblewimble-py with slatepack support 🚀 which will probably make my life in making that tool a lot easier.
I also have been pondering about the use of SeedSigners for Grin. They are cool, but them being offline might make things complex since the connected wallet would probably need to use rewind_hash functions (something similar to public keys only wallets in Bitcoin), to know the state and funds of the wallet. Also I was a bit disappointed with their price, basically they are as expensive to buy as Ledger or Trezor Hardware wallets that support a lot more coins.

+ jdavies, cekic , ardocrat
How was your week @cekickafa?
I hope we can find some new meeting times that will allow other CC members to join our biweekly meetings to spice things up.
My time is nearly up, I have to go in 3 minutes
Ok, I am of 👋

__cekic__: Sorry  anynomous. Disconnected and Keybase crashes. I was away from comp 3 weeks.
That seedsigner DIY may lower the cost. I ordered parts separetly and assembled. Do we need better bulletproofs multisig for making grin custom seedsigner ? Hardware assemble part is more easy, firmware is the unknown.

## MWixnet Integration Update

__yeastplume__: I nearly have the mwixnet comsig code properly integrated into the master branch of the wallet. Just a few tests and bits of documentation then we should be ready for a new build including it
[https://github.com/mimblewimble/grin-wallet/pull/726](https://github.com/mimblewimble/grin-wallet/pull/726)
and it will also be available in the json-rpc api
+cekic, any, syntajax, jdavies , ardocrat, circusdad, natsuni



## *TO DO List*

*  Continue development of Python wallet tool, utilizing slatepack support in `mimblewimble-py`.
*  @yeastplume: Finalize testing and documentation of the MWixnet comsig integration into `grin-wallet`, including json-rpc API.
*  Community: Discuss and propose better meeting times to encourage more CC participation.


**Meeting adjourned.**