

# Community Meeting Notes January 31, 2023

Community Council (CC) meeting held @ 15:00 UTC in grincoin#general channel on Keybase. Meeting lasted 68  min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_


* quentinlesceller
* MCMmike
* anonymous
* nicolasflamel1
* dtavarez
* cekickafa
* defistaker
* yeastplume
* phyro
* vegycslol





# Short Summary
 
- Spending policy of Grincc has been discussed for being minimalist approach or carry on same policy.
- Zkwrapper bounty payment recalculation and to be paid to @nicolasflamel.
- GrinnCC Bitcoin Fund display will be added to Grincc.mw site.



# Agenda Points & Actions
 

* Last meeting notes here: https://github.com/grincc/agenda/tree/main/notes

* Current meeting [agenda](https://github.com/grincc/agenda/issues/80)








__anonymous__ : Lets take 1 minute to look at the agenda for today. If there are any topics to add, do not hesitate to propose changes to todays agenda.


__nicolasflamel1__ : I'd like to discuss some concerns I have with the payout amount for the Python CFFI secp256k1-zkp wrapper bounty. Please add this to the agenda for today's meeting.

👍 anonymous


## 1)  Minimalism in CC spending, should the CC be more minimal in spending while the Bitcoin price is down?

__anonymous__ : For todays first agenda point:

1) Minimalism in CC spending, should the CC be more minimal in spending while the Bitcoin price is down?
https://forum.grin.mw/t/minimalism-in-spending-of-the-community-council/10228/21
I started the discussion on this topic a month ago, because I think it is relevant. We should be responsible and minimal in our spending when we can, especially if that will be in the long term interest of the projects and the generous donors who granted these funds.
From most in the community I received positive feedback on this notion, meaning they would encourage the CC to be somewhat more minimal in spending. From many other community members as well as from CC members I did not see a reaction yet on this 'proposal'.


__cekickafa__ : is this precaution conditional to Btc price ?

__anonymous__ : Somewhat, in general we should be responsible. But yes, especially in times of low Bitcoin price we should really consider if waiting a bit before the prices are higher is not in the general interest of the project. At least that is my opinion.
Some features can wait a few months, others cannot.
E.g. adding PIBD is priority. Nice to have features, like a nice coloured button for this or that, can wait.

__MCMmike__ : 



>__anonymous__ : From most in the community I received positive feedback on this notion, meaning they would encourage the CC to be somewhat more minimal in spending. From many other community members as well as from CC members I did not see a reaction yet on this 'proposal'.

I agree to be resonsible with the spending, but at the same time we also not wasting any money in my oppinion. 
We funding and paying what is nesessary currenctly.

On the other hand I would like to see more funds go towards the bigger goals.

__anonymous__ : Agreed, so for example. Funding new 'nice to have feature' in Grin++ can wait IMO, since everything works well as is.
For this discussion it might be useful to look at the post 5.0 Wishlist:
https://github.com/stakervali/grin-wishlist


__MCMmike__ : Also allocate some funds, not sure if this is soly our responsability:

- CoinSwap
- Atomic-Swap

This needs some funding as well to be completed. These two "projects"  I would categorize it as long-term projects which would require funds to be finished.

👍 cekickafa

__anonymous__ : Only Critical and Important items should be funded IMO untill price is again at 30k
Those could be categorised as Critical or Important, just like implementing PIBD also in Grin++

__cekickafa__ : So is there a distinction between GRINCC and OC funds?

__anonymous__ : No, we do not discuss OC funds, only CC funds

__MCMmike__ : We as, CC and only speak for the CC funds , but we can always ask OC at any time


__anonymous__ : PIDB implementation is funded by OC for grin rust, but when ready, I am 100% in favour of implementing it also in Grin++ as soon as possible to get the whole network to support PIBD.
If it is funded by OC or CC funds does not matter IMO, as long as it gets funded. So @dtavarez would be free to apply for funding PIBD implementation in Grin++ to either OC or CC.

👍 dtavarez

When it is ready to implement on main net.
That is just my opinion though, if others see PIDB implementation in Grin++ not as Critical or Important, feel free to say so.

__cekickafa__ : So any other implementation would apply OC or CC, python for example.?

__anonymous__ : Also, complete freedom to apply to whichever fund, CC, OC, or even an external funding, independent funding etc. No one puts restrictions. Only restrictions is that owners of repositories review and may reject code if they do not agree. But anyone can add, and anyone can apply for funding anywhere.

__cekickafa__ : Sure no restrictions, exploring just.. Spending guidelines is clear for both funds. No problem there.

👍 anynomous

__yeastplume__ : IMO funds aren't there to be conserved as long as possible, they're there to be spent on grin as the opportunities arise

👍 cekickafa

a few years ago, the value of the entire fund was down to about 150k Euro's worth, we didn't stop spending it.

__defistaker__ : I agree on being cautious on spending.

__phyro__ : that's true, at the same time, I wouldn't want it to be spent just for the sake of it being spent

👍 anynomous

__anonymous__ : I do not think conservation is the purpose, but neither is spending them, it should be a balance.

👍 defistaker, yeastplume

__phyro__ : or to feel as if we're making steps forward.

__yeastplume__ : 

>__yeastplume__ : IMO funds aren't there to be conserved as long as possible, they're there to be spent on grin as the opportunities arise

I should add, we were spending it on grin development, and the return was clear and evident

👍 phyro

__anonymous__ : Indeed, the thing is, Grin is doing well. So IMO we do not need to push, just maintain what needs to be maintained and spend where it is really important.
Yes, I think we need again have to more clear definition of deliverables and report back clearly which are achieved and which are not and why. And focus on long term large deliverables, the ones that really matter.

So for example, I am in favour of not spending much on groundkeeper work, until prices are higher (>30k$).
In any case, I think we can discuss this in much more detail on the forum as well as on individual funding requests.
Is it ok to move on? If anything needs to be said right now on this topic, please do so
For todays second topic:

## 2:) GrinCC FUND reports display

__cekickafa__ : yes, that is.. The majority of the demand and discussion is focused on the fund's final balance.
So, in order to gain access quickly, we should create a section on grinnc site similar to grin.mw.  The community members wants to see that feature.

__anonymous__ : I agree, I think that is important information to make easily accessible.

__defistaker__ : Okay, I can add it to finance section.

👍 cekickafa

__MCMmike__ : I got approached by a user, who wanted us to create a PR on /finance first and then do the payout. 
We would have to add the TX-ID later I guess to the PR and then merge it. 

Not sure if this is something we should incorporate?

- we need 4 CC members to push to the /finance repository this is a hard requirement
- also we need CC members to sign of on the transaction (mutli-sig)

__anonymous__ : It is enough to link to a blockexplorer I guess.🤔

👍 cekickafa, phyro

To avoid unneeded work.

__cekickafa__ : yes, basically this link and display is enough, from the feedback from several users.

👍 anonymous



__anonymous__ : Ok, for todays third topic @nicolasflamel1 

## 3) Concerns with pay-out system

__nicolasflamel1__ : The BTC SMA price from today's date was used to determine how much BTC to send for the bounty's payout, but I feel like it would make more sense to use the SMA price from either the date that @renzokuken verified that my code satisfies the bounty's requirements, December 26th 2022, or the date that I finished creating the GitHub PR containing all the deliverables that fulfilled the bounty, December 7th 2022.

It doesn't set a good precedent to allow the slow operating nature of the Grin CC to impact which date is used when determining the SMA price for paying out bounties. This is concerning since the Grin CC is allowed to impose additional last-minute requirements on a bounty that can further delay when its payout is drafted, such as requiring that the code is tested by X amount of people.

__anonymous__ : We always use a 1 month average at the time of drafting. Sometimes this works in favour, sometimes against the receiver. But the rules are objective and clear. @mcmmike I thought we had it documented on the github page, but I could not find it so quickly.
In this case the hold up was the final reviews.
In general we try to keep our pay-outs within a 2 weeks interval of final approval. I think the final approval, is only a couple of days old (meaning we had enough votes from CC members).


__cekickafa__ : 

>__anonymous__ : We always use a 1 month average at the time of drafting. Sometimes this works in favour, sometimes against the receiver. But the rules are objective and clear. @mcmmike I thought we had it documented on the github page, but I could not find it so quickly.

https://github.com/grincc/docs/blob/main/funding_requests.md

👍 anonymous, MCMmike

__anonymous__ : @nicolasflamel1 I can understand, you would have preferred to get paid the amount from the dip, at the time of completion, but there will be other times that this system will work in your favour. It is not perfect system, but it is the best system we could come up with without favouring or disfavouring anyone.

Another way to look at it is that you got paid much more than the $ value of 10k$ since we use a 1 months average. If we would pay-out in USDT, you would have 40% less.


__nicolasflamel1__ : The current BTC SMA price doesn't accuratley reflect the price that motivated me when I completed the bounty. It seems weird to use the SMA from today when I wrote the code almost 2 months ago.

__anonymous__ : Again, this is all speculative, we could have paid you and you might have sold at that day, we cannot take all hypothetical cases in consideration. That is why we wrote those rules. Maybe we should provide a link to the rules with the bounty.

__MCMmike__ : In essence we have to descide now if we do the payout around end of December with the SMA, correct? 
Because @nicolasflamel1 did complete the work by end of December as I did understand it when Marek did approve the code 26.12.2022.

__anonymous__ : Yes. Basically that is what it is about. But personally I am against any exceptions to the rules, it is like blockchain, it should be as objective and consistent as possible. If we make an exception now, what about next time, or previous times. For example, scilio got in value something like 40% less because the Bitcoin price dumped greatly within hours of paying his bounty.
We cannot control these external factors, nor should we try to control them or compensate for them IMO.
Consistency and clear expectations are the key.

__MCMmike__ : Did we have another meeting after the 26.12.2022 where we started we will do the payout ?


__nicolasflamel1__ : The post for the bounty didn't include the requirement of having an additional person test the code. This wasn't added until after the @renzokuken had already tested the code, and his change caused the drafting time to be pushed back by 2 weeks.

__MCMmike__ : 

>__MCMmike__ : Did we have another meeting after the 26.12.2022 where we started we will do the payout ?

@cekickafa can you double check quickly ?


__anonymous__ : Testing of the code is a requirement for approval, so it does not need to be specified, since it is about being approved.

__cekickafa__ : 

>__MCMmike__ : @cekickafa can you double check quickly ?


No. Meeting was 20 Dec and 3 january respectively.

__MCMmike__ : Did we state there we are going to draft the transaction / payout, as I was not in this meeting ?

__cekickafa__ : Ok, yes i remember mentioned. let me check.
keybase://chat/grincoin#general/56348

__anonymous__ : In the meeting of 17th we specified that we needed two testers who gave their 👍 Before approval, so conditionally approved, after that @dtavarez and renzokuken did their audit, after that we got approvals from additional community members. 
So timewise we have not been tardy, actually quite quick.

__cekickafa__ : agreed to pay at 17 january meeting.

__anonymous__ : ok, then I am fine and would agree we proceed with doing the transaction now with the current SMA.

__anonymous__ : It is already broadcasted.
So it should be fine IMO, we just followed the protocols we set out long ago, which are 100% the same as the OC if I am not mistaken.
I got to go now, @mcmmike @cekickafa could you wrap up the meeting when it is done?

👍 cekickafa, MCMmike

__MCMmike__ : lets give it a few more moments for this to finalize
--- proceeding --- 

Do we have any other topic before we close this meeting ?

__defistaker__ : I think that was all.

__MCMmike__ : I would say thanks to @anynomous for leading through this meeting.
- meeting adjourned - 

Thanks to all 👍
 
## *TO DO List*

*  Calculate SMA payment for zkp wrapper bounty and complete payment to @Nicolasflamel. 

* Add  Bitcon fund display to GrinCC.mw site by  @defistaker





**Meeting adjourned.** 🔨



