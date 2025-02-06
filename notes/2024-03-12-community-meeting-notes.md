# Community Meeting Notes March 12, 2024

Community Council (CC) meeting held in grincoin#general channel  keybase chat  Meeting duration not explicitly stated, assumed to be around 45-60 minutes.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_


* anonymous
* cekic
* defistaker
* waynegeorge


# Short Summary

- Discussion regarding the visibility of current Grin projects and the need for better communication.
-  Debate and clarification on the status of Nicolas Flamel's Ledger code funding request.
-  Discussion about the lack of funding requests for ongoing projects like Ironbelly and Grin++.
-  Issues with Grin++ stability, fee estimates, and API were brought up.
-  Slatepack transaction testing using Grin-GUI was discussed.
- Community website status discussed and ToDo list added.

# Agenda Points & Actions

* No explicit agenda was stated
* Website update with latest info.
* Grin++ maintenance 
* Grin GUI Slatepack issues and tests.
* Nicolas Flamel Ledger code funding status.
* Mimblewimbl.py funding is completed.

## Project Visibility and Communication

__waynegeorge__:  Hi guys. Perhaps if someone popped in after some time away, they may not easily find a summary of current projects. Grin website is great for historical info but doesn't represent current activity. Grin CC site may be obscure for some.

__anynomous__:  We do have a wishlist with some updates I think on the GrinCC github page, but not something like a roadmap on the website. I meant the Grincc website, but also that one needs to be updated ones in a while. I just checked, it does contain up-to-date list of CC members: [https://www.grincc.mw/](https://www.grincc.mw/). Perhaps I can ask @defistaker how to update the hub part and meeting part. I think it involved converting the info to a json, is there an automatic script for that @defistaker, or an example template. If not, I could write a script to do it automatically and save time in the future.

__waynegeorge__: Perhaps a "centralised" twitter account may be helpful. Just to post about news

__anynomus__: Probably it would be. Not sure if there are community members who are already doing this.

__cekcik__: There is twitter account of me. I frequently post in all channels. If he is an old user, impossible to not see.

__waynegeorge__: Amazing, thanks. I already follow you.

__anynomous__: I mean even throwing "Grin" in Google would lead you to the newsletters and github page where you see Grin GUI is developer. I mean hell, we have 1) contract flow, 2) unified payment proofs, 3) Parallel Initial Block Download (PIBD), 5) Grin GUI, 6) CoinSwap is ready to be reviewed/implemented 7) IronBelly just got updated and Grin++ were updated less than a year ago... Mimblewimbl.py updated 1 month ago and funded... and then you also have hobby projects like open Grin block explorer and recovery tool etc.

__defistaker__: I will try to update the website at the weekend. I am very busy lately but it is on my todo list.

__anynmous__: Sure no problem. Do you have script, or would it be useful if I created one?

__defistaker__: The projects section uses a json format. and also some part of meeting notes, I think.

__anynmous__: Ok. It should not be too hard for me to make a Markup Language to Json conversion script, and automatically do it for all relevant pages.

__defistaker__: I don't have any script, nor there is any backend. I think I ran a script for updating search functionality.

__anynmous__: Ok. I think a long time ago you send me an example json of how a page is supposed to look. I will have a look when I have time and see if I can make a script for it.

## Nicolas Flamel's Ledger Code Funding

__waynegoerge__: Quick one guys and forgive me if the forum post has newer info on it, but I was wondering about N Flamels request for funding for Ledger code. I recall that his quote was too high. So is it officially rejected?

__anynmous__: My personal opinion was that he was indeed asking too much, although perhaps compensating some extra costs such as a fee for reviewing by Ledger could be reasonable. But that is just my opinion. @waynegeorge I have no clue. The OC was asked on the forum, but there was not answer there from them, only some community feedbacks. I assume they had contact to discuss things... but I am not sure. @phyro do you know if there is any update on this, or something ongoing? In any case, it is not our business to meddle in.

__cekikc__: @waynegoerge Quick one guys and forgive me if the forum post has newer info on it, but I was wondering about N Flamels request for funding for Ledger code. I recall that his quote was too high. So is it officially rejected? cekic reply ledger to review the code but sometime ledger quit reviewing codes afaik.

## Funding and Development Status

__waynegeorge__: Just a thought, perhaps Grin OC and CC could take advantage of the bull runs. Just be more frivolous with requests.

__cekic__: +1

__anynomous__: In general I think we are easy going with requests.... there are just no new ones coming in 🤷‍♂️ I mean we offered to pay for maintenance update for IronBelly, no response... offered to fund Grin++ update, no response... I think now it is up to the Developers to make funding request, in what format, that is still open for debate. Indeed. But it did not hamper development, IronBelly just updated their backend, so it's up to date. Perhaps OC took care of things. With @dtavarez, not sure why he is not making any Funding Requests, but I think he is just busy with personal life at the moment Also, I am not satisfied with peers management in Grin++ at the moment. It appears to be rather unstable. So perhaps it would be good for @dburkett to work on that at some point if he has the time. I see this as sort of a critical issue for Grin++ which should be fixed yesterday IMO since Grin++ is already a mature project.

__cekic__: yes, Grin++ has a quite userbase.

__anynomous__: Indeed. Also the unified API, I think it is not yet in any stable release. For any follow-up projects, for example the Grin-voucher tool I am building, it does require Grin++ to have the same API calls to work with Grin++. So it would be important to add that to the stable release at some point.

__waynegoerge__: I did have an issue in the current version of G++ that DT was aware of relating to which outputs were selected for a transaction. I think a particular combination of outputs was causing an issue.

__anynomous__: Also the fee estimate that is shown in the GUI is incorrect. it contains 0.000005 value, which is 0.5 of the base fee, so I suspect the estimate is made by simply dividing the fees by 2, but that is incorrect to show to the user, or the fee itself is wrong. So that is another issue that needs to be fixed. So in summary @dtavarez,.... make a funding request and fix all these persistent bugs ones and for all 😉 . Enough whining from me. Grin++ still works fine most of the time, I just want it to be perfect and keep parity between Grin++ and grin-wallet/Grin-GUI.

## Slatepack Transaction Testing

__anynmous__: Talking about Grin GUI. @cekickafa you did manage to make a transaction using slatepacks right? Was that on Windows? I still got errors when I tried using alpha-5. I used slatepacks generate by IronBelly, so I want to see what the difference is in our setup. You generated a slate using XXX wallet and then send it to Grin-GUI, or did you initiate the transaction from GrinGUI?

__cekic__: i made from miner wallet to GUi. I didn't test grinn++ wallet. Yes slatepack method. TOR isn't working.

__anynomous__: miner wallet, grinmint?

__cekic__: No easygrin. A ok.

__cekic__: YOu tried grinn++ to GUİ?

__anynomous__: I will run some more tests then using grin-wallet, which I think is in the back of easygrin.

__cekic__: yes that is why i used easygrin wallet.

__anynomous__: Makes sense.

## Meeting Conclusion

__anynomous__: I think we can wrap up the meeting, or is there some else we can discuss.

__cekic__: Let me try ironbelly then. i let you know

__anynomous__: That would be great, thx 👍

__cekic__: Thank you for leading. 👋

__anynomous__:Ok, time to clear my head and then get back to coding 🤓

## *TO DO List*

*  Update the community website with the latest information.

* Test Grin GUI Wallet by community.



**Meeting adjourned.**