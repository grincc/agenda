 # Council Meeting Notes January 04, 2022

 Community Council (CC) meeting held @ 15 UTC in grincoin#general channel on Keybase. Meeting lasted 90 min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

<br/>

### _Community attendance:_

* __dtavarez__
* __sheldonth__
* __phyro__
* __cekickafa__
* __defistaker__
* __yeastplume__
* __jankie1800__ 

</br>

# Agenda Points & Actions


* Last meeting notes [here](https://github.com/grincc/agenda/blob/main/notes/21-12-2021-council-meeting-notes.md)
* Current meeting [agenda](https://github.com/grincc/agenda/issues/31)

</br>

## 1) Organizing community for extending grin ecosystem

__dtavarez__ : @__defistaker__ any brief introduction about the first topic?
* __defistaker__ : Well. it came up on the video meeting that mcmmike held. In the meeting, nagini had expressed some ideas to increase grin's public interest. @mcmmike suggested to continue discussion in today's meeting; I think nagini has not joined the meeting yet.

__defistaker__ : He(nagini), talked organizing a team of 10 people for twitter, then start to twit in an organized way at the same time so that it would have a more powerful effect
* __dtavarez__ : mm nagini isn't here though

__phyro__ : I think a lot depends on who's handling the social media. Positive content for a project done the wrong way can deter people from even looking at it - that's what makes me not even look at 99% of the projects. You'd need a high level of maturity and a good way to present things. I think Paouky was an example of someone doing good tweets. I'm not sure I'm explaining this well tbh, but I hope you guys know what I mean


__dtavarez__ : My opinion is that I think things will flow with more active contributors. We tried to create sub teams before and I'm not sure if that was successful.

__jankie1800__ : there are many exciting developments happening in the ecosystem; something of interest may be bringing back the 'Grin Community Project Day'; a place where developers can demo, showcase, and talk about their projects,receive feedback etc; perhaps even use the video conference platform. (idea [sourced:](https://github.com/mimblewimble/grin-pm/blob/master/ecosystem/03122019-community-project-day.md)). examples would be grinvention/ grinnode live speaking on their ongoing projects. Also wallet devs speaking on their projects. Just something to think about :) and I like the additional ideas, anything to boost engagement I am all for
* __dtavarez__ : I'm not sure we have enough contributors to do that
  * __defistaker__ : I agree
        
__dtavarez__ : my opinion for extending grin ecosystem is that we need in person meetings all over the world, we need to grab a beer or two and talk about crypto

__sheldonth__ : I would host an in-person meeting in NYC someday soon if people are interested or nearby

        
__defistaker__ : I think we can postpone this issue, come back later if nagini decides to join
* __dtavarez__ : I agree 

</br>

## 2) Update on groundskeeper work and the clear delegation of items

__jankie1800__ : just a quick update on workflow. Defistaker and I agreed on delegating newsletter and meeting transcription over to my tasks; while Mr.staker will continue to update the ongoing agenda items. I think this will allow for a more transparent workflow, and bit more more efficiency through a more focused process.

__defistaker__ : I will be more involved with website and other tasks

__jankie1800__ : before we were juggling these tasks back and fourth, and like defistaker says this will allow for more focus on our individual workflow

__dtavarez__ : what about the finance report? any idea when are we going to publish the CC spending?

__cekickafa__ : grin spending reports not published too I think

__jankie1800__ : this needs to be addressed certainly. I can commit to working out best how to organize this into the GrinCC github
* __dtavarez__ : are you guys going to manage that too?
  * __jankie1800__ : at this point it has been unaddressed, but i think we all agree it should be a priority

__dtavarez__ : can we confirm is publishing the spending reports is part of the tasks?
* __jankie1800__ : if you don't mind Mr.Staker. I can tackle this?
  * :+1: _defistaker_, _cekickafa_ 
    
__dtavarez__ : probably by the end of this would be nice to have a report. can that be a potential estimate? end of the Q1 2022?
* __jankie1800__ : agreed.
  * __dtavarez__ : thanks! any other updates?

__jankie1800__ : just a note; This adjustment doesn't change our collaborative workforce as I believe we remain committed to working together through assisting each other when and where needed while further communicating ideas and strategy.

__defistaker__ : I have added a [council info to grincc docs](https://github.com/grincc/docs/pull/6). I will add this to home page of website, if approved/corrected
I have done some fixes on website, only the dark mode problem is left, I am dealing with that right now. Google chrome somehow converts black color in grincc logo to white in dark mode...

__dtavarez__ : at the end I think it is important to have transparency on what we have been doing, a place where anyone could go and read the meetings notes, the spending, agenda, etc. that's my opinion.

__dtavarez__ : should we continue with the next topic? 

</br>

## 3) Discussion on platform for grin-wallet UI (possible frameworks Qt, Orbtk, React/Web, vanilla Web)

__jankie1800__ : redbean! but I know that it likely be too buggy for serious development

__dtavarez__ : @__sheldonth__ is here, right?

__sheldonth__ : I am, yes

__dtavarez__ : cool, would you mind to introduce the topic?

__sheldonth__ : Yes, so on this topic, which I know is a bit of a hotbed for debate since there other very nice GUI wallets live in the field at the moment, but I wanted to see if we could coalesce around a possible tech stack for a UI on the rust grin-wallet code. We had discussed this with yeastplume a few weeks ago, and he mentioned that in a historical context he felt like it was a mistake not to have a GUI on the reference wallet.<p> John Tromp had recommended a project called redbean, which I am just digging into this morning, but it's a fabulously elegant want to have a truly run-anywhere double-clickable web powered UI (must like electron) but significantly more lightweight that looks really nice.@__jankie1800__ I just watched a youtube video from the project author who says this thing is ready for production use and she does not look like the type of engineer that would make such a claim lightly. There is some serious software engineering under the hood in redbean. I like it a lot</p>
* __jankie1800__ : that's an incredible product, really is. I did notice that near the end she mentioned something about read/write not being fully functional on windows at the moment

__dtavarez__ : what about Tauri?
* __sheldonth__ : I still need to look into Tauri - perhaps this meeting is more about assembling a list of options. I could do an indepth research project on each of them before the next meeting.

__dtavarez__ : or Orbtk?
* __sheldonth__ : Yes, that's another. There was some discussion that Orbtk might not have enough a future maintenance schedule around it for our needs. Like, it has just a few authors and they seem not so active.

__phyro__ : one question I have is how do 0-day browser exploits affect the tech
* __dtavarez__ : not much because what is been distributed is the engine not the browser

__sheldonth__ : I concur, I don't think 0-days in the UI are of too much concern. Well, can we all concur we aren't interested in electron? It's so heavy, so dependency laden, I think it just doesn't feel right for us.

__jankie1800__ : @__sheldonth__ are you thinking of including the node built into the ui as well? because if I'm not mistaken that would set this apart from the already developed wallets.
* __sheldonth__ : so i'm picturing a system where you can elect to connect to a remote node (live grinnode.live) OR you can choose to have the UI spin one up locally, yes. But yes, jankie, I'd like a little feedback there too. I'm thinking that this UI does have the ability to spin up a node for you - thoughts from the team on that?

__phyro__ : I like the option @yeastplume mentioned Monero has. You can setup a local node during the install (or maybe when setting up the wallet) or use a remote one.
* __sheldonth__ : correct phyro, that's the idea

__dtavarez__ : what do you mean with spin up?
* __sheldonth__ : fork an instance of the grin executable on the local machine, and connect to it with more interaction from the user than that, no more
* __dtavarez__ : Grin++ is doing everything you are mentioning in the post
* __sheldonth__ : correct, it certainly is.

__jankie1800__ : while grin++ has node feature I believe the point is to build out ontop of the Rustlang reference.
* __dtavarez__ : Grin++ is not supporting remote nodes, and probably it will never support them 

__sheldonth__ : @__dtavarez__ by no means is this a slight on grin++ - nor do I intend it to be. I think grin++ is great software and a boon to the ecosystem. But I also don't think it's existence precludes the undertaking at discussion here. Really, the challenge as I see it right now is choosing a tech stack. And maybe that just means we pick one and start building. If we like what we get out the other end, then we keep it - if we don't - then all that was lost was some developer hours

__dtavarez__ : I'm an advocate of people contributing with fits better for them, I just want to say that. if members find that it is time to have a UI in the <mimblewimble> that's fine

__defistaker__ : is this new wallet gonna work on mobiles as an app?
* __sheldonth__ : @__defistaker__ good question- I think aiming for mobile compatibility initially could be difficult. The aim is a single "download, click, run" executable for mac/windows/linux/freebsd/netbsd- where the Ui works on all those desktop platforms 

__jankie1800__ : sounds nice but the question comes down to man hours at some point

__sheldonth__ : Here's a proposal for moving forward: I will investigate, in this order: redbean, orbtk - and put together a very minimal proof of concept.  Let's see - can that single "download, click, run" system be built that works- If it can, we'll reconvene in some time and choose which one it seems like works better

__dtavarez__ : but why not to include niffler into the mimblewimble repo if xiaojay agrees? and improve niffler from there? and IronBelly? those two wallets are using the rust node- this is not clear to me
* __sheldonth__ : Niffler's stack is electron and react?
  * __dtavarez__ : I guess yes
* __sheldonth__ : I need to take a closer look at Niffler I'm not too familiar
  * __dtavarez__: cool

__sheldonth__ : Just as a screen cap from the redbean demo, electron is very heavy. I have an idea that perhaps it could be avoided. Okay, so let's table this discussion until some more investigation of the possibilities is completed.

__dtavarez__ : I think it will be totally unfair in my opinion
* __sheldonth__ : What's unfair? 
  * __dtavarez__ : not supporting the current UIs projects; if they agree on moving the current UIs to the mimblewimble org, I don't see why not to do it- last commit on Niffler was on May 29, 2021. and @i1skn is still working alone 
* __sheldonth__ : Hmm, ok, duly noted. I will take a closer look at Niffler. Perhaps a small working proof of concept might be the best way to get the community to coalesce around a particular approach to putting a UI on the reference wallet. I will not be unfair to the technology that's already out there. I assure you.

__phyro__ :  I can't say anything about this tbh. I think this is more complex than it looks at first. We'd need to have a clear goal of what we want from a "reference wallet"
* __dtavarez__ : I though that we were not interested in UIs- but probably that changed and it is irrelevant. But still why not support ironbelly? or Niffler- and I'm sorry I don't want to bring any divisive conversations
  * __phyro__ : I think this is less about support and more about the design of what we may label a reference wallet but we haven't really had the discussion how people see this. So this is just my random thoughts design here isn't meant as UI but rather system design- It's ok, respectful disagreements are welcome
* __sheldonth__ : I agree phyro, it's system design all the way down.
* __dtavarez__ : grin is not like that, it is not supposed to be like that- there is no centralized entity dictating anything; if we want to have an agreement on something we need a RFC and all devs must follow them

__sheldonth__ : let's look at the history of bitcoin for some guidance here: bitcoin-qt was launched in 2010, and the Qt ui in it's basic form (gray, no color, just a few buttons and checkboxes) has served it well for a very long time. It's very robust and very lightweight, and Qt was a system decision that bitcoin stuck by and continues to this day. If we "bond" the reference wallet to electron - that's a system design choice that will be with grin for a long time to come. Having other wallets use electron is fine, just as other bitcoin wallets use electron, but what we call the "reference wallet" and what we use to build the UI is a system design question with some far ranging consequence for our users.
* __dtavarez__ : agree we want a reference UI, I've posted about it before, and I think that's great but a reference UI could be a set of designs and templates, nothing more. not a full GUI written meant to be run and that's what is being suggested- those are two different things
* __phyro__ : I think what sheldonth wants to have is a minimal UI on top of grin-wallet that would last for a very long time, rather than a design template.
  * __sheldonth__ : yes that's exactly correct @__phyro__
  * __dtavarez__ : and that's Niffler 

 __sheldonth__ : Okay, for the sake of time let's table this and move into the next topic at this meeting. I think this was a healthy discussion and perhaps if some other OC members read this at a later point and want to chime in with feedback that'd be great. But I'm glad we have a discussion here on the record about it
* __dtavarez__ : but still that's not true,(minimal UI) is not what is written in the forum post, but we can continue with the next topic

__yeastplume__ : Just back on the wallet for a second, we do have a reference implementation (the CLI) and we're fairly unique in that we've spent a lot of time developing an API that cleanly separates any wallet from the core implementation. This API can be called over a socket or linked directly, so there's little danger of any particular wallet becoming 'bound' to grin wallet-
It's a very clean separation at the moment. Any wallet that I'm a part of producing will keep using that API, and if any parts of the API prove deficient than the API and underlying core code will be modified. So in my mind, it doesn't matter what the UI portion of it is coded in. My choice personally would be heavily influenced by whatever is easiest for UI designers and frontend developers; it's unlikely I'd use QT or any rust based libs or anything that requires front-end developers to also know Rust or C++, it's asking way too much of an individual

</br>

## 4) Current situation of scriptless scripts 

__defistaker__ : @__philippnagel__  added this to agenda


__jankie1800__ : I wonder if it is accurate to assume that If Taproot enabling scriptless scripts with BTC then there could be some very interesting cross-chain use cases

__dtavarez__ : about [Scriptless scripts with mimblewimble](https://diyhpl.us/wiki/transcripts/grincon/2019/scriptless-scripts-with-mimblewimble/) anything else we can find out about this?

__cekickafa__ : mimblezimble phyro [posted](https://www.reddit.com/r/Bitcoin/comments/rcxgq1/the_blockchain_scripting_wars_are_over_bitcoin/?utm_source=share&utm_medium=web2x&context=3) 

__phyro__ : I'm not sure whether there was a specific question regarding these, but scriptless scripts are possible if you have Schnorr signatures, so we can still do them on Grin, but we haven't seen projects doing that

__dtavarez__ : probably we could compile more info about this on a forum post

__dtavarez__ : @__defistaker__ probably we can conclude today's meeting :) 


</br>

## *Action Points*
</br>

* GrinCC financial report @__jankie1800__ due by end Q1 2022


