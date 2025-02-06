# Community Meeting Notes December 3, 2024

Community Council (CC) meeting held in keybase grincoin#general channel chat. Meeting duration not explicitly stated, assumed to be around  45-60 minutes.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_

* anynomous
* cekickafa
* aglkm

# Short Summary

-   Finalization of the Grin Telegram Bot bounty, with updates posted on relevant forums.
-   Announcement of testing efforts for Grin GUI and MWixnet, with a call for community feedback.
-   Discussion about the removal of SHA256 checksums from the Grin website download links, with clarification on the rationale behind using GitHub links.

# Agenda Points & Actions

*   Finalization of the Grin Telegram Bot bounty.
*   Discussion and announcement of testing efforts.
*   Clarification on website download links and SHA256 checksums.

## Grin Telegram Bot Bounty Finalization

__anynomous__: Link to today's agenda: [https://github.com/grincc/agenda/issues/150](https://github.com/grincc/agenda/issues/150)
Let's take a minute to read the agenda, if anyone wants to add anything, they can propose to do so. Let's start with today's first agenda topic:
1) Grin Telegram Bot bounty finalization.
Done. I posted an update on the bounty page and on the forum thread where Marek shows his progress regarding the bounty.

## Testing Announcements

__cekickafa__: 2) Testing announcement made via forum and newsletter. Hope we can get some feedback.

__anynomous__: Now the real work starts, testing.

__cekickafa__: :)

__anynomous__: If I can find time, I will do some testing myself. I have unfortunately a lot of running projects right now, and with Christmas breaking coming on… I do not think I will be able to do much of anything basically. Anyhow, that is also not the job of the CC, but we do not have a limited number of community members who... So, I would not be surprised if in the end it turns out a lot of testing will be done by CC and OC members.

__cekickafa__: I tweaked GUI a bit. I am not sure if I can run this mwixnet. But I will try.

__anynomous__: I can compile and run it probably, but then there needs to be multiple online, and then running quite a few tests. Probably I will start with some contract flow testing.

__aglkm__: @anynomous Probably I start with some contract flow testing. I'm going to test and play with contracts too

## Website Download Links and SHA256 Checksums

__cekickafa__: And topic about Grin links, removed sha256, content can be changed via link.

__anynomous__: Grin links, you mean the error I got with the Seed check (also something about a link file) or are you referring to something else like SHA256 checksum of binaries?

__cekickafa__: Main site download link with JavaScript. Sha256 removed, a member warned me.

__anynomous__: O ok, that is new to me. I do not know who maintains the website now. Was that in a DM, or can you link here to the message?

__cekickafa__: DM. I mean we need to see the hash, not the file.

__anynomous__: O you mean see the hash directly and not the link to a hash file?

__cekickafa__: Yes, link content can be changed.

__anynomous__: Actually, I think that might be the reason they gave the link. The website can be compromised, but the link leads to the GitHub page which is harder to change since there are very strict admin privileges as well as any change being noticed easily since it requires a commit. Same for the download, it all leads to the GitHub page. So basically for both, as long as it leads to [https://github.com/mimblewimble/](https://github.com/mimblewimble/)… something, you know it's official and correct. Let's say they would host it directly on the website and put the hash there as text, well, one only would need to hack the website which is easier than hacking or faking GitHub pages.

__cekickafa__: Ok, I just put this for hesitation, to be careful about breaking main site reputation Grin. Concern is heard publicly imo. Thanks for clarification.

__anynomous__: The above is just my assumptions, we can check with whoever maintains the website. They must have their reasons.

__cekickafa__: Sure. Little things can catch off guard.

## Meeting Conclusion

__anynomous__: Yep, I think testing contracts is a bit easier for me. So I'll start with that. Ok, I think we can call it a day. Or are there any more things we should discuss?

__cekickafa__: That's all topics.

__anynomous__: Thanks for being here all today, let's see if we can find some time in our busy schedules for testing. Also for CC members who were not present, I assume that is because they are busy running tests already.


## *TO DO List*

*   Community: Start testing Grin GUI with contract flow and MWixnet as per the forum and newsletter announcements.




**Meeting adjourned.**