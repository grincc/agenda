



# Community Meeting Notes September 26, 2023

Community Council (CC) meeting held @ 10:00 UTC in grincoin#general channel on Keybase. Meeting lasted 38  min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_

* waynegeorge
* yeastplume
* ardocrat
* anonymous
* cekickafa
* future3ooo





# Short Summary

-  Mwixnet last status and on going process of integration to GUI wallet mentioned by developer @yeastplume. 
-  Grin++ final status info has been forwardd by developer @DavidT.
- GRINCC election officially ended. New members; @Trab and @Trinitron collected most votes. 

# Agenda Points & Actions
 

* Last meeting notes here: https://github.com/grincc/agenda/tree/main/notes

* Current meeting [agenda](https://github.com/grincc/agenda/issues/106)





__cekickafa__ : Ok, i will start if you dont mind.


 ### FOLLOW Ups,

### Grin++ Tasks
I talked about Grin++ tasks with Davidt, and he informed me that the current status is as follows;
I'm preparing a beta release right now. Linux and macOS are kind of buggy. The v1.2.9 binary in crashing on macOS and Linux. On Windows works just fine so far. CLI version written on Python is working OK using the new API. I'll release it on [flathub.org](https://flathub.org/)

I've been testing several distribution methods for that. The documentation will be auto generate since it is an inline documentation. I think by the end of this week I will be able to do it.
I'll remove the unsafe code before release. The code regarding the bug when someone sends all balance, which is causing that the transaction is not updating the status of the transaction. The fix I didn't commit it because it isn't safe. I need to find an alternative.
Also unsafe code from Python will be remove it. Hopefully I think I can release a Beta by the end of the week.


He also said he would be unable to attend Keybase meetings and would have to take three to four months off due to family matters.

### Mwixnet status;

I pinged Scilio, if he can join the meeting. As much as i check from [github mwixnet](https://github.com/mimblewimble/mwixnet/pull/20) 

Multi-server support & Generate ephemeral pubkeys randomly for each server has been merged by @yeastplume in order to make the code easier to work with for a basic wallet integration_, so currently testing by @yeastplume & @phyro's reviewing still continues and scilio is preparing for 3rd milestone to complete the Coinswap implementation.

👍 syntaxjax, future3ooo, JohnDavies


__waynegeorge__ : Thanks. So sounds like DT has an update at some point and mwixnet is still in progress. for mwixnet, is there a completion percentage?


__ardocrat__ : ready when ready :)


__cekickafa__ : It is completed more than %60 i think, final phase. I am not expert tough i cant estimate:)

__ardocrat__ : percentage can be counted if we will have Kanban board with tasks

👍 cekickafa

There is no such tool..

__waynegeorge__ : I guess it's also worth tracking activity along with completion progress. Otherwise a project could sit at 95% for a year
Github Prjects has a kanban that could be used

__cekickafa__ : i agree. The thing is it is very technical stuff, and community members dont participate in testing, reviewing phase.

__waynegeorge__ : Perhaps GK could add something
Then anyone at a glance could see the status of active projects

__cekickafa__ :  yes, this Kanban method mentioned earlier, maybe we should do it.

__waynegeorge__ : Perhaps in the grincc org on github
There could be a kanban view and a roadmap view perhaps. It could start simple just to get something going and for it not to feel to much work to maintain.

__cekickafa__ : Well anything which will help developers is worth to try &do imo.

__yeastplume__ : I'm putting the ability to make requests to MWmixnet into the wallet, here. Plan to integrate this (as well as all the other work been done over the past few months on contracts and early proofs) into the GUI wallet experimentally over the next couple of weeks.
https://github.com/mimblewimble/grin-wallet/pull/696

👍 cekickafa, waynegeorge, anonymous, 🥳 future3ooo

then there is going to be a lot for the community to test, tweak and feedback on, we could very much use people looking into mwmixnet and trying to run a server network.

__cekickafa__ : That is ok. Noted.

__waynegeorge__ : I remember a bounty competition once that was very active and seemed a sucess. Perhaps something like that could be done again to get people interested

__cekickafa__ : For mwixnet or ?

__waynegeorge__ : yes and for anything else, g++ even.

__cekickafa__ : Mwixnet is already a bounty itself, and Grin++ current tasks is funded upfront.

__waynegeorge__ : I think it was a competition to resolve issues of varying difficulty actually.
I think on grin code.
Any other topics to discuss or talk about? Is it worth discussing the election at this point?

## 1) GRINCC Election Ended.


__cekickafa__ : Well, o. Maybe new Grincc members will join and bring new ideas and dynamism to governance, so they are absent. Nothing to discuss, just for the record Election Period ended.

👍 ardocrat

__ardocrat__ :

>__waynegeorge__ : I think it was a competition to resolve issues of varying difficulty actually.

Bug bounty can be good idea

💯 cekickafa

>__cekickafa__ : Well, o. Maybe new Grincc members will join and bring new ideas and dynamism to governance, so they are absent.

Yeah, will be cool to have them at meetings :)

👍 cekickafa

__waynegeorge__ : Cool, so trab and triniton are now CC menbers?
I assume

__cekickafa__ : As i can see @Trab collected most of the likes/votes. 2nd @trinitron and 3rd @Danila.

👍 future3ooo, waynegeorge, anonymous

__ardocrat__ : Danila is CC member? :D

__future3000__ : After all that only 3 candidates 😅 We need to make an announcement.

👍 cekickafa, ardocrat.

__cekickafa__ :

>__ardocrat__ : Danila is CC member?

No, trab and trinitron.

👍  ardocrat

__waynegeorge__ : Is there an official length for these meetings or just when their done.

__cekickafa__ : No officialy but topics covered. So it is almost done. Open discussion goes on.
thanks all 👋

__waynegeorge__ : thanks
👋

__future3000__ : Thanks for your efforts @cekickafa 🙏

🙏 cekickafa


 
## *TO DO List*

* 




**Meeting adjourned.**



