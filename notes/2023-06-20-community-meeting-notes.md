
# Community Meeting Notes Jun 20, 2023

Community Council (CC) meeting held @ 15:00 UTC in grincoin#general channel on Keybase. Meeting lasted 28  min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_


* ardocrat
* anynomous
* cekickafa
* waynegeorge




# Short Summary
 
- Bounties proposals has been discussed with benefit and costs.
- Bounty idea for an opensource HD wallet is being opened for discussion.
- Current state of PIBD testing and more testing by community has been discussed.

# Agenda Points & Actions
 

* Last meeting notes here: https://github.com/grincc/agenda/tree/main/notes

* Current meeting [agenda](https://github.com/grincc/agenda/issues/92)








__anynomous__ : Lets take 1 minute to read the agenda
First lets have a look at the TO DO's from last week:
### TO DO 1: Forum discussion about considering removing/ electing/ adding new members to GrinCC.

https://forum.grin.mw/t/grin-cc-member-review/10572?u=cobragrin

@future3000 created the post. Lets just say I am not to happy with the amount of discussion we got going there, especially from CC members. As a CC we are planning a meeting this week to discuss issue, like the activity of CC members and the need for some of us to step down and bring in new blood or otherwise have change.

👍ardocrat, cekickafa, johndavies, future3ooo


### TO DO 2 Review of Financial PR
https://github.com/grincc/finance/pull/14#pullrequestreview-1488371206
We need more CC members to review here, again it shows the problem at hand with CC activity.


Now for our first agenda topic of today:

## 1) New funding governance proposal with a) "Funding proposals" & b) "Bounties with milestones and conditional upfront payment"

https://forum.grin.mw/t/funding-proposal-1-parallel-initial-block-download/10584

https://forum.grin.mw/t/funding-proposal-1-parallel-initial-block-download/10584/8#bounties-with-milestones-and-conditional-upfront-payment-1

IMO opinion these two new methods to go from proposals to funding makes it easier for developers and at the same time guards funds and deliverables very well while also allowing upfront payment of trusted community members and developers.

It got some feedback, also negative, the negative feedback mostly had to do with some community members liking there to be more bounties in general, which is understandable.


__cekickafa__ : My personal opinion, i think bounties can get us new developers. That is the main problem since years. That is why i am fan of it.

👍ardocrat



__ardocrat__ : I like bounty idea at all, cause it is easier to check deliverables and control the budget, also I think it is more motivational :)


👍 anonymous, cekickafa

__anynomous__ : I like bounty idea at all, cause it is easier to check deliverables and control the budget, also I think it is more motivational :)

👍ardocrat


__waynegeorge__ : In terms of the funding proposal, it seems very fair to me. I think with a breakdown of milestones, it wouldn't take long for a new developer to build trust without them going far unfunded

__ardocrat__ : I have only one idea for now it is Hardware Wallet as Bounty

__anynomous__ : I was also thinking about that one, I already gave my specifications for an interesting community hardware wallet here:
https://forum.grin.mw/t/grin-hardware-wallet-development/10541/37?u=anynomous

👍ardocrat

But to be honest, I do think it can wait till the BTC price is above 30k
But even that we can specify in the bounty 😁

__cekickafa__ : What if BTC doesnt it 30k ? Grin development suspends?

__ardocrat__ : 

>__anynomous__ : But to be honest, I do think it can wait till the BTC price is above 30k. But even that we can specify in the bounty

It is rule for all funding or only bounties?

__anynomous__ : No, basically pay-out can be denominated in dollars and we say, we can only pay when BTC price or the 1 month average which we use for paying, is above 30k

👍 cekickafa

__waynegeorge__ : I really like the idea of an open source hardware wallet and think it's worth the development costs.

__anynomous__ : Maybe we can make this a #TO DO, I will create a new discussion on the hardware wallet to create such a conditional bounty.

👍 cekickafa 

__waynegeorge__ : I don't think that BTC price should affect development at this stage.


__anynomous__ : We need more input though on the formfactor, chipset, etc. Also there might be some limitations. For example, the one I showed runs micro-python, which would probably require a minimal python implementation of the wallet.

__ardocrat__ : 

>__waynegeorge__ : I don't think that BTC price should affect development at this stage.

Sure, I think at beginning we can use existing hardwares and try to build something on them. Like custom firmware with Grin support.

__anynomous__ : 

>__waynegeorge__ : I don't think that BTC price should affect development at this stage

Unfortunately it should, since we have to weight costs against benefits for the community. A hardware wallet like this is a bonus/extra, we already have ledger support. So I think most would argue we should not spend to many funds on it.

__baumhaus_nomade__ : Hello everyone, I am new here, happy to find new things here

👋 cekickafa, vegycslol, anonymouos, waynegeorge, ardocrat

__anynomous__ : Welcome, always nice to see a new face/avatar

__cekickafa__ : 

>__anynomous__ : A hardware wallet like this is a bonus/extra, we already have ledger support. So I think most would argue we should not spend to many funds on it.

i think Ledger last events, changed everythnig. I wouldnt touch Ledger from a mile.

__ardocrat__ : 

>__cekickafa__ : i think Ledger last events, changed everythnig. I wouldnt touch Ledger from a mile.

I never touched too, only Trezor :)

💯 cekickafa

__anynomous__ : Yes, it most definitely damages the trust in Ledger. Still, it would probably be more cost effective to implement Grin in an existing hardware wallet such as Trezor or Bitbox.
Anyhow, this can be part of the discussion on the forum.

👍 waynegeorge

__waynegeorge__ :

>__anynomous__ : A hardware wallet like this is a bonus/extra, we already have ledger support. So I think most would argue we should not spend to many funds on it.


I'm not sure about the Ledger works yet as I haven't checked for any validation of the code. As I understand you need to install an unofficial MW app


__ardocrat__ : 

>__anynomous__ :

I was also thinking about that one, I already gave my specifications for an interesting community hardware wallet here:
https://forum.grin.mw/t/grin-hardware-wallet-development/10541/37?u=anynomous

at your last message you sent a device on RISC-V, it was hard for me to compile Rust Grin on it, I tried once :) but micropython should work for sure without pain

__anynomous__ : O cool 😎 , you tried. Was looking up against it but also was planning to try to compile it.

In any case, lets continue this discussion on the forum. Perhaps this would be a nice next bounty.
A little warning, I have less time today (beer date with some friends), so I will rush the agenda a bit.

## 2) PIBD current state and Testing on mainnet

__anynomous__ : Nice testing @ardocrat 

💓ardocrat, cekickafa

🚀 Also thanks to @noobvie

__ardocrat__ :  Last time I am seeing more and more peers with 5.2.0-beta at my peer list :D

👍 cekickafa

__waynegeorge__ : Is there anything additional to be done to assist testing on mainnet? Would it help to have more testers?

__anynomous__ : Yes, I am happy to see more people involved in the testing. In this way, development can be so much faster and more effective
@waynegeorge Yes, it does really help to have more testers who report bugs and create logs. I will try the new beta once it is released.

__ardocrat__ : 

>__waynegeorge__ : Is there anything additional to be done to assist testing on mainnet? Would it help to have more testers?

Just more cases, like updating from non-PIBD to PIBD and losing PIBD peers when sync is restarting. Last case is harder to test.

__anynomous__ : I tried to compile on Sub Systems for Windows, but it sucks a bit

__cekickafa__ :  Windows really sucks, it blocks all Grin related.


__waynegeorge__ : I'm planning to spin up some nodes.

🚀 anonymous 👍 ardocrat


__anynomous__ : Probably it would work if I would compile for main windows, it is specific for the subsystems for Linux which normally works super duper well, but apparently not for rust compilation.

__ardocrat__ : 

>__ardocrat__ : Just more cases, like updating from non-PIBD to PIBD and losing PIBD peers when sync is restarting. Last case is harder to test.

I will try last case with fixed amounts of peers from list at config, will disconnect my PIBD peer and see what is going on, I think @noobvie caught this thing.

__anynomous__ : Nice
Guys, I have to go, there are cold 🍻 waiting for me as well as a thunderstorm, so I need to be lightning fast and get to the pub before this thing blows

👋 cekickafa, ardocrat

__ardocrat__ : Have a good time :)

__anynomous__ : Thank you all for a nice and informal meeting. Leets keep things up with bounty proposals/discussions and PIDB testing.

👍 ardocrat, cekickafa, waynegeorge

__cekickafa__ : Thanks @anynomous



👋 cekickafa, ardocrat, waynegeorge, anonymous.







## *TO DO List*


* Forum discussion about creating bounty for HD wallet.

* Feedback for GrinCC member review.



**Meeting adjourned.**



