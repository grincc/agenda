
### _Community attendence:_

* __anynomous__ 
* __jankie1800__
* __mark_hollis__
* __dtavarez__
* __cekickafa__
* __defistaker__
* __vegycslol__
* __tromp__
* __phyro__
* __joltz__

<br/>



# Short Summary

- [Funding request](https://forum.grin.mw/t/request-for-funding-davidtavarez-nov-jan-2021-22/9265/8) for  __dtavarez__  (€5,000/month  Nov-Jan 2021/2022) is approved.

- [Funding request](https://forum.grin.mw/t/community-action-and-agenda-working-with-the-groundskeepers/9233/14) for * __jankie1800__ and * __defistaker__ (€1,000/month  September-Nover 2021 is approved.

- There is a possibility we can still get G1 miner, * __anynomous__ will inform the community after it is clear.

- Gene will be paid for May to June's work ASAP, and his work in June will be reviewed after a post from Gene

<br/> 

# Voting Results 

* Voting for funding request of __dtavarez__ Non-Jan 2021/2022 is *__approved__* with 5 Votes in favour   (__anynomous__, __mcmmike__, __future3000__,  __defistaker__, __joltz__,  __phyro__,  __cekickafa__, __tromp__,  __vegycslol__, __jankie1800__).



* Voting for funding request of __jankie1800__ and __defistaker__ Sep-Nov 2021 is *__approved__* with 5 votes in favour (__anynomous__, __dtavarez__, __mcmmike__, __future3000__, __cekickafa__).

<br/>


<br/>

# Agenda Points & Actions

* Last meeting notes [here](https://github.com/grincc/agenda/blob/main/notes/28-09-2021-community-meeting-notes.md): 

* Current meeting [agenda](https://github.com/grincc/agenda/issues/18)

1) [Request for funding](https://forum.grin.mw/t/request-for-funding-davidtavarez-nov-jan-2021-22/9265) @davidtavarez Nov-Jan 2021/22.
2) [Groundkeepers task list finalization](https://forum.grin.mw/t/community-action-and-agenda-working-with-the-groundskeepers/9233/14).
3) Situation of Purchasing G1 MİNİ Asics.
4) [Atomic swap funding payment delay](https://forum.grin.mw/t/request-for-funding-gene-adaptor-signature-atomic-swaps-grn-btc/8632/17?u=davidtavarez)

<br/>

##	1) Request for funding @davi* __dtavarez__ Nov-Jan 2021/22.

https://forum.grin.mw/t/request-for-funding-davidtavarez-nov-jan-2021-22/9265

* __anynomous__ : Maybe @* __dtavarez__  can shortly summarize this request

* __jankie1800__ : progressing the G++ experience benefits end users in a very real way. I'm all for it  

* __anynomous__ : Same here, wallet development and improvement is never ending, there always is a better use experience beyond the horizon.

* __dtavarez__ : This is a request for a 3 months period (November 2021 - January 2022). During this period I want to focus on improving Grin++, specially the Android version. I also want to invest time on improving the support of Grin++t for Raspberry Pi.

    There are a lot of stuff that I’m planning to work on, but I feel that it is better if I focus only in one thing at a time.

    more details here https://forum.grin.mw/t/request-for-funding-davidtavarez-nov-jan-2021-22/9265

* __anynomous__ : Although I support the proposal, I would like to point out that I still would have liked the task list to be in bullet point style.
I am looking forward to see your ideas for the improvement of the GUI.

    Is there anyone who would like top propose changes or has suggestions for this funding request?

* __dtavarez__ : the first thing is to solve some annoying bugs regarding the UI due to the different implementations of each manufacturer, specially on Samsung
after that:
    * Let users use the wallet without waiting for the node to sync. The Node is running as a Service in background, but still I'm blocking the App until full sync.
    * Currently, I'm supporting multi-wallet on Android, but it doesn't make sense for mobile users. What I want to do is to have a more standard experience like other wallets.

* __anynomous__ : You need some automatic scaling in the GUI I guess, does Ironbelly also have these issues?

* __dtavarez__ : IronBelly is using a different framework, I guess they face another types of issues

* __anynomous__ : Hope it can be tackled in a systematic way

* __defistaker__ : is it react native?

* __dtavarez__ : Grin++ mobile is written using Xamarin, which is C#
.net standard 2.0

* __defistaker__ : Yes I checked grin++, I asked IronBelly's framework

* __dtavarez__ : IronBelly is React Native, correct

* __jankie1800__ : there are interesting new hw options available like the pinephone,librephone etc running on ARM architecture. After dev for android and Pi would it be feasable to use this code on this platform as well?  The Open source hardware comunity may tie well into the grin ecosystem is why I ask.

* __dtavarez__ : C# is robust enough to let dev migrating cryptographic routines into the mobile app directly in the future.

* __anynomous__ : 👆 Not sure if a pinephone is beefy enough.
For now I think we can take back a step from the technical aspect.
Would anyone like to add or change something to the proposal before we continue with voting?

* __dtavarez__ : that's why I want to also improve the ARM branch

* __joltz__ : Have been hacking a bit with a pinephone. @__dtavarez__ if you are interested I'll get you one to test with, just pm me

* __dtavarez__ : that would be perfect!
I'm using qemu, maybe it is possible to run pinephone on qemu idk

* __anynomous__ : Hope it would work out, it would finally give me a reason to buy a pinephone, been searching for a reason for a while 😆
For now, lets continue with voting, unless someone wants to add something to the proposal.

* __joltz__ : it's good to have the hardware to test

* __dtavarez__ : true

* __anynomous__ : I would like to vote in favour of funding this request:

    I also have asked @mcmmike amd @future3000 who gave me their votes in favour of funding this request.

* __defistaker__ : I vote in favour 

    👍 ( __joltz__,  __cekickafa__, tromp,   __vegycslol__,   __jankie1800__)

* __phyro__ : 👍

* __joltz__ : @__dtavarez__ is a legend, lucky to have him

* __anynomous__ : Since @* __dtavarez__ himself is excluded from voting, that gives us a quorum in votes from the Grin Community Council members as well as votes in favour from the community.
Hence, I would like to declare this Funding Request Approved.
🚀Congratulations @* __dtavarez__

* __dtavarez__ : Thanks!!!

## 2) Groundkeepers task list finalization.

https://github.com/grincc/agenda/blob/main/notes/31-08-2021-council-meeting-notes.md

* __anynomous__ : On 31st of August we approved the funding of the Grin groundkeepers: 


* __jankie1800__ : I propose that we agree to finalize this task list and then expand on additional individual contribution in a single 'work forum post'. That way we set the Groundskeeper work and also clearly expand on our single projoects.
i . Bi-Weekly Newsletter Community updates.( A future forum post will be created to organize and facilitate new-releases )
ii . Maintaining Community meeting agenda and notes for community review
iii . Remaining available to expand on and meet work requests from the community
iv. Design and maintenance of grincc website
v. - Contribution to official web site (Based on community requests assist to fix an issue/ add a feature or help when a new blog post text needs to be converted to jekyll template, and make pull request)

* __anynomous__ : Yes, the above task list was never 'officiated' in a grin community council meeting. Hence we would like to ask here for feedback and approval by the community.

* __jankie1800__ : also would like to point out numeral iii.Remaining available to expand on and meet work requests from the community

    It is fortunate that there are 2 Groundskeepers. this allows us to remain flexable and still remain open to new creatives

* __anynomous__ : I think the above list is fine, but indeed I would encourage to have some individual projects to work on for efficiency. No doubt new tasks might pop-up that come with the work, hence having the 2 of you is beneficial since there is a more diverse pool of skills available to tackle them.

* __phyro__ : it seems that 5. is captured already by 3., no?

* __defistaker__ : Somehow, yes

* __phyro__ : in the sense that if the community requests X, then you are available to work on it

* __janki1800__ : please note that this proposal adds a 'work-update' forum post from Stakervali and I so the community will be clear on these 'individual' work initiatives.
I see this as being continually updated so we need to set the baseline on timeframe of expecation.
what does the community think is an efficent time frame to communicate 'work-update' post timelime?

* __anynomous__ : True, there is a bit of overlap, but I asked them to be somewhat explicit in their tasks, makes it easier to asses what they will be working on.

* __defistaker__ : I am more concerned on website, while jankie wants to work on dev outreach and other public relationships.

* __jankie1800__ : it is my understanding that to keep updated assets such as github, and website would be the responsibility of the goundskeepers.

* __phyro__ : I think it would be good to have some more objectively measured tasks e.g. deliver CC website, deliver bi-weekly updates, etc.

* __jankie1800__ : I think bi-weekly updates through the 'work-update' forum post  would clarify these matters no?
to be clear. I am also capable of coding so I do/ will contribute to asset maintence.

* __anynomous__ : That would be good, as well as maybe think a bit about long term objectives for yourself, e.g. overhauling the website in the 1st quarter.
Anyhow, we have to find the balance, not over defining but as well having some measurable outputs.

* __phyro__ : I suggest we agree on the changes to the website before we start making them just to avoid any work going into something that people wouldn't agree on

* __defistaker__ : I think certain deliverables are a good idea. I can promise for the grincc website as a deliverable, but some comumunity tasks may take too much time.

* __anynomous__ : I agree with that, there are many who love the website as it is, hence big changes might be not welcomed by some community members.

* __jankie1800__ : you and I may work together to be efficent in our work Staker. I am committed to assisting you in doing our job :) 

    (__defistaker__  👍)

* __cekickafa__ : i think it needs changes.at least website something better change.Grin stagnate

* __anynomous__ : For now, can we vote on this task list, with the prospect of having some more defined tasks and deliverables on the forum later on.
O and lets not over-define, there are some dangers in that.

* __phyro__ : agree. Let's also explain a bit through which methods we plan to reach other devs etc.

* __defistaker__ : Just want to be clear about website, we are working on grincc website which mainly have meeting notes, documents and etc. related to grin community council. We are not proposing an overhaul change for official grin site

* __anynomous__ : In that case no one will object, plain github versus rich github webite is a no-brainer 🙃

    I vote in favour of the task list as discussed above. 
    (👍   __cekickafa__ )

    I also have @future3000's vote. 

    Agrees with the funding of the groundkeepers. 
    "My main point is that we make all payment request votes public, so we have a record, and the community knows what’s going on."

* __cekickafa__ : ok. Community is here 😀

* __anynomous__ : I agree with Mac that we should have a quarterly open voting on continued funding like we have for any other long term funding request.

* __dtavarez__ : I also vote in favor.

* __anynomous__ : and your other vote?

    Also to clarify, with this vote we are also voting to approve/confirm the first funding round of 3 months from september-novermber.

* __dtavarez__ : it is also important to keep the community posted  with everything regarding our work and the funds

* __anynomous__ : This can be part of the newsletter, as well as via github updates after payment and forum post or keybase news.
 
    but @* __dtavarez__ you still should give @mcmmike vote, he gave it to you right?

* __dtavarez__ : correct

    __@mcmmike__ words: "I am fine with the work of Stakervali as I coud judge him last 6 months. Definitly we should do it on a max 3 month basis and then re-evaluate."
    he's on the road right now that's why he is not here during this meeting.

* __anynomous__ : Perfect, then herewith I would like to approve the task list as discussed here as well as the requested changes.
With it we approved the funding of ther period September-November for @* __defistaker__ and @* __jankie1800__.
Congratulations, your pigy banks will soon be filled

* __defistaker__ : thanks 🙂

* __jankie1800__ : thank you. I am very appreciative to be working with everyone

* __cekickafa__ : Congratulations * __defistaker__ and jankie


## 3) Situation of Purchasing G1 MİNİ Asics.
 
* __anynomous__ : After contact with NHash, there is a chance we can get a G1. If so should we go again with the original proposal of 1 G1 and 12 G1 Mini?

    So basically, there is a chance we can go back to the original plan of 1 G1 and 12 G1 mini's, I would be in favour of that (I mean it is what we decided on in the first place), but what do you all think.

* __janki1800__ : logistics. who, where, how.

* __dtavarez__ : if we can still accomplish the original plan, I think we should try it

* __cekickafa__ : G1 is big and noisy and electric cost.But g1 mini electric cost wont be much problem. G mini instead of G1 is more logical?

* __anynomous__ : That is my main problem with 42 G1 mini's, the logistics, who, where how. I do believe we can get them distributed in the community, but the logistics, checking of the payments etc. it would just create quite some overhead, I rather spend my energy or the energy of the groundkeepers on something else if possible.

    The mini's are more decentralised, but they do actually consume more energy per grin mined. So as long as we find a good location for it, G1 might be preferable @* __cekickafa__

* __cekickafa__ : Reasonable

* __anynomous__ : Yes, if the G1 does not push through (it is not certain yet), the alternative of 42 G1 mini's will still be fine, we will adapt as community.

* __jankie1800__ : would a forum post to gauge housing the miner be progressive here?

* __anynomous__ : I asked before on the forum, there were some volunteers, not yet enough for 42-12 (council members) = 30 G1 miners.
Until it is clear if we can go back to the 1 G1 + 12 G1 mini's I would like not to put it on the forum, since we are flipping between plans all the time. Once it is final, I will post there again for whichever miners we could get.
 
 
## 4) Atomic swap funding payment delay

* __joltz__ : Gene reached out last night saying that he had not received payment for May or June. I asked him to make a post so we could review the data since it had been so long to refresh memory. 

    While he never reached out over the last several months asking for payment I still take responsibility for not being more proactive. Will resolve his May and June payments asap. I really hope this did not negatively impact his contributor experience here too much. 

    In the future we should all make sure that we have capacity for review in coordination with funding requests to help prevent these gaps in the request -> approval -> review -> payment cycle.

* __anynomous__ ; Our capacity to review code and RFC's is to limited as far as I see, hence I think a 'sub-team' that focusses on contacting old and new grin contributors would be great.
@__jankie1800__ and I will be on this subteam and I hope others might join.

    The objective is to create a better overview of the latent capacity we have in the existing grin community as well as in new developers and cryptographers who might be available on demand.

    But great that you are taking care of this @* __joltz__ I think there is not much else to discuss here then. Maybe it is time for some quarterly Grin OC meetings?

* __dtavarez__ : while we work to bring more contributors to Grin, in the future we should all make sure that we have capacity for review the work

    unfortunately there is no easy way to solve this imo

* __jankie__ : @* __anynomous__ looking forward on expanding on this

## Closing

* __anynomous__ : Since we reached the end of our agenda. Is there anything else that we should discuss today?


* __cekickafa__ : @* __mark_hollis__ posted an update. öaybe he has words?
i saw him at meeting joined

* __mark_hollis__ : Hi, I don't have extra points to mention at the moment.

* __dtavarez__ : Is there anything we could do to support you?

* __mark_hollis__ : At the moment I can't think of anything yet. I am translating my C app into Rust now, so that's my focus at the moment. But there will certainly things I will have to ask yet.

* __anynomous__ : Then lets get to work 💪
Thank you all for being here today, and see you in 2 weeks hopefully

## *Action points*
- Keep community updated with mining equipment purchase developments.
- Gene will be paid for May to June's work ASAP, and his work in June will be reviewed after a post from Gene.
- jankie and defistaker will create work-update forum posts for reporting their

<br/>

__Meeting adjourned__








