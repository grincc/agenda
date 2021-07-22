# Council Meeting Notes July 06, 2021

Second Community Council (CC) meeting held @ 3PM UTC in grincoin#general channel on Keybase. Meeting lasted 65  min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendence:_ 

* __mcmmike__
* __quentinlesceller__
* __mark_hollis__
* __anynomous__
* __dtavarez__
* __cekickafa__
* __defistaker__
* __ux041__
* __hendi__
* __dburkett__
* __phyro__
* __satoshocrat__
* __kurt2__


<br/><br/>
## Agenda Points & Actions
<br/>

### 1)  Status multi-sig address
<br/>

* __mcmmike__ : What is the current status ?

* __mcmmike__ : We the community council did setup a multi-sig address and we agreed on one address which we made public here: https://github.com/grincc/finance/blob/main/addresses.md

* __cekickafa__ : ** claps **

* __mcmmike__ : Any comments/ questions on this topic

* __anynomous__ : We all did a full recovery test, so for the coming years we can be sure that we all have access to our keys.
 
* __mcmmike__ : Also we will provide a quarterly signed message, for everyone to see that we have still control. 
We will make it public here: https://github.com/grincc/security

* __quentinlesceller__ : Have you tried receiving and sending?

* __anynomous__ : Yes

* __hendi__ : yes, both

* __quentinlesceller__ : On bc1qmdhmgmhd6j89225hzdh7dxqgmen3y2q0g4vgpez0tw9tkp4ae39qsqvuyl ?

* __mcmmike__ : yes both, we used a different addresss an tested everything. Full recovery + sending / receiving
 
* __anynomous__ : no that one specifically, but that is a few addresses further in the pregenerated address list so that should not be an issue. We did independently verify the address is in our wallet

* __mcmmike__ :  as you perhaps know, when creating a multi-sig adress the wallet is creating multiple addressess (pre-generated addresses) we just used one of these to test the whole process.
 
* __quentinlesceller__ : Yes, it's a HD wallet :).
 
* __mcmmike__ : also we used different methods of storing private keys internally.

* __anynomous__ : Since we just did a full recovery test, I think the first security check should be in October.

* __mcmmike__ : lets open an issue for this later.

* __dburkett__ : Any clue what the OC progress is on the key refresh, @__quentinlesceller__ ?

* __quentinlesceller__ : No progress on this end. I'll try to get things moving. 

<br/><br/>

###  2)  Fund spending guidelines review
<br/>

* __mcmmike__ : We also agreed on a base set of rules for spending and made it public: https://github.com/grincc/docs/blob/main/spending-guidelines.md  any comments / ideas etc ?

    If not you are welcome to open a PR or issues to discuss this with us anytime.

* __defistaker__ : On Decision process, maybe it should be specified, how long will it take for the mentioned project
<br/><br/> 

### 3)  Setting up a Grin Community Council Grin node with donation address.

<br/>

* __anynomous__ : So regarding point 3 on the agenda, we do think it is very important to set up a Grin node and wallet next, to have a Grin donation address ready.

* __dtavarez__ the challenge here would be making sure the wallet is always listening at least most of the time.

* __anynomous__ : Yes, for that reason a low power computer, e.g. dedicated raspberry pi should do the trick.
 
* __dtavarez__ : the challenge here would be making sure the wallet is always listening at least most of the time
 
* __anynomous__ : Yes, for that reason a low power computer, e.g. dedicated raspberry pi should do the trick.

* __dtavarez__ : and also in this case we will need to trust one person to have the wallet running
 
* __anynomous__ : Yes, that is a small issue, which I think we can manage by having multiple people with the keys, to verify the Grin is there. Secondly, we will use the Grin as much as possible for community activities, so the target is to have only a limited amount at any time in that wallet.
 
 * __dtavarez__ : if someone wants to volunteer... my question would be, how can we be transparent with those donations?
 
* __ux041__ : I guess publishing transparency reports of receiving funds would be necessary too
 
* __hendi__ : I would volunteer to have a node running 24/7, doing it anyway for mutliple purposes already
we should definitely share the seed phrase with at least one other member though

* __mcmmike__ : if needed, I can volunteer to donate a small vm within the grinnode.live infrastucture to run the wallet, but we need to come up with a transparency process for delegating responsibilities in terms of Keys and passwords, etc

* __mcmmike__ : ah ok I vote for @__hendi__ then :smile:

* __dtavarez__ : should the volunteer be part of the CC?
well, I also support @__hendi__ for this 100%

* __hendi__ : suggestion: I run it; it's my responsibility to keep it running; keys are shared with at least 1 other member of the CC, it's both our responsibility to give monthly (?) transparenty reports / confirm each other

* __anynomous__ : That sounds trustworthy enough to me. If someone donates millions in Grin, we can always build in more checks :wink:

* __dtavarez__ : I think transparency reports could be done by the CC as a team

* __dburkett__ : You could theoretically share the view key publicly. We don't currently have any tools that support view keys, but it'd be easy to code a simple one up.

* __dtavarez__ : that sounds the better option

* __mcmmike__ : ok good idea @__dburkett__ .
Then we agree @__hendi__ hosting the wallet and until David has this view key programmed we use a scond/third CC member to verify.

* __dburkett__ : I wasn't necessarily volunteering to code it hahaha. I don't have time unfortunately. But I could walk someone else through it.

* __mcmmike__ : we can fund you :)  as this is something really interesting and possibly needed for GRIN.

* __anynomous__ : @__dburkett__ No hurry, till that time comes I volunteer to double check __hendi__ did not go shopping with any Grin ;)
* __anynomous__ : __dburkett__ Yes, you can make it a funding request, but it is also ok to involve someone else if you are swamped with work.

* __mcmmike__ : @renzokuken I know you still sleeping, but this might be interesting for you when you wake up to look into.

* __dburkett__ : Cool. Glad to hear we have options.

<br/><br/>
### 4) Mining equipment purchase
<br/>

* __mcmmike__: anyone please take over here

* __anynomous__ : Sure I handled that point also last time.

* __anynomous__ : But feel free for anyone to but in since I have little news to share on this point. Mostly Mike has connections with Nhash whish should make it easier to buy equipment.

* __anynomous__ : I can facilitate the discussion, but there is not much news to share, apart from that the first batch of G1 miners is sold out, and that Mike has close contact with Nhash, so it should be easy to buy from their next batch.

    I think we can make it a task for the next meeting to contact them to see if they want to provide miners with discount to the community council as a form of sponsorship and of course marketing for them.

* __dtavarez__ : how much are we planning to buy? anyways we don't have a Grin yet :joy:

* __anynomous__ : yes, indeed

* __cekickafa__ : what you mean next batch? sales closed also this july i think

* __anynomous__ : According to the information from Mike, the first batch is sold out, that one was discounted. The next batch is sold at normal price. I did however not talk to them, so if anyone has more information, please share
 
* __ux041__ : There is a concern the devices are priced high ATM and if production of G1 (not mini!) will continue, G1 mini will taken away from network (like what happened to antminer Z9 mini)

* __cekickafa__ : g1 mini and g1 chips are same. how its taken out? G1 is= 30x mini

* __ux041__ : If there is the option of purchasing the G1, IMO it could be better option.

* __anynomous__ : In that regard I think we are flexible, since we want to buy roughly the equivalent of on G1 miner either as G1 or in lose G1 Mini's
    I agree @__ux041__, it would make maintenance and configuration easier
    What are other opinions about this, Mini's or simply go for one G1

    Let me make that a vote thing:
    1) 1x G1  (  __ux041__, __anynomous__ voted)
    2) 42 G1 Mini ( __cekickafa__, __satoshcrat__, __dtavarez__, __dtavarez__, __phyro__ voted)

    <br/>
 
* __cekickafa__ : Decentralize it

* __phyro__ : having a single miner is very prone to getting a faulty device. Having more of them averages out things

* __defistaker__ : @_phyro_, did you vote for 2

*  __phyro__ : I lean towards 2 because of the reasons mentioned above, but I don't know how much of a burden this adds to the community council members so I'll leave it up to them
 
* __anynomous__ : It depends, the power supply of G1 Mini is not that great, so G1 might be lower risk

*  __ux041__ : I guess 42x of G1 minis will need more initial money to pay as well.

* __cekickafa__ : no.almost same cost

* __anynomous__ : The big question is, how to manage, maintain and configure 42 minis, who has them (multiple people, otherwise what is the point)?

* __dtavarez__ : I don't think they will sell us 42 minis, so the problem won't be that big

* __cekickafa__ : why?

* __dtavarez__ : the production is limited, one, and two, I think they already have buyers

* __anynomous__ : Also how to handle electricity cost when deviding large number of mini's, I foresee a lot of administrative hassle. But if there are only a few, it should be manageable...i hope

* __ux041__ : Then it's just about maintaining. CC members votes matter much on this.

* __anynomous__ : Or, involving non CC members in this

* __mcmmike__ : before we make a final decision can we agree on the following:
If we as CC are starting to buy mining equipment, can we also agree to mine on a community pool which is not one of the big ones ?

* __dtavarez__ : I think we could yes
 
* __anynomous__ : Ok, so agreed, we will use the community mining power on a small pool
Any volunteers for running G1 Minis (asuming we can buy them)?

* __dtavarez__ : I think we could agree on this later I guess, I think things will change after we get a real amount of minis that they can sell us


<br/><br/>
###  5)  Grin ledger hardware wallet progress
<br/>

* __mcmmike__ : One topic I would like to ask @__mark_hollis__ about his update, perhaps you can talk a little bit about it? Update: https://forum.grin.mw/t/grin-ledger-hardware-wallet-progress-thread-by-markhollis/8670/21

* __dtavarez__ : @__mark_hollis__ 1) do you need help? 2) any support? 3) is everything in order regarding your funding?

* __anynomous__ : 4) how is your health, are you feeling any better?

* __mark_hollis__ : 4) Not really better yet.

* __anynomous__ : Just do what you can for now, without compromising your health.
And do not hesitate to ask others for help

* __mcmmike__ : if you not feeling comfortable now we can pospone these questions for another meeting

* __mark_hollis__ : It's mostly I am working on parts here and there, where I see some path to improvement. But that means now that the firmware is at the moment in progress on several parts.

* __anynomous__ : Is your funding ok for the moment?
 
* __mark_hollis__ : Funding is ok

* __anynomous__ : Ok, if you need help on any specific part, let us know.

* __mark_hollis__ : I feel like I'm too vague too often, sorry.

* __cekickafa__ : i think you work too much man. Your github is full GREEN. Take care your health.
 
* __anynomous__ : No problem, just answer any specifically if you feel the need for it. But do not forget to reach out for help if you need it. Ok, any other updates we need to share or discuss.


* __anynomous__ : Before we close the meeting, I would also ask everyone to feel free to add agenda points of your own to the agenda for the next meeting.
    The Community Council members are only representatives of the community, but we as community as a whole set the agenda and direction of Grin. So use the power you have to influence the direction of Grin.

<br/><br/>

### 6)  Council Meeting Hours
<br/>

* __mcmmike__ : Before we start with the first agenda points, I wanted to suggest changing the start time of the CC meetings. As not all of us CC members can participate. 

I am suggesting 12/13:00 am CEST for next meetings to start
suggestions?
👍 (__mcmmike__, __dtavarez__, __hendi__, __anynomous__, __defistaker__)

* __anynomous__ : Agreed

* __dtavarez__ : Agreed

* __quentinlesceller__ : That'd mean people on EST/PST timezones can't participate ?

* __anynomous__ : Yes, that might be an issue. We can alternate the time with each meeting.

* __hendi__ : We have a member from NZ who can't participate at the current time
 
* __anynomous__ : In any case there is no solution to suit all, so for now we can have alternating meeting times

* __dtavarez__ : I agree with alternating the time.

* __mcmmike__ : suggestion:  first meeting of a month at 12:00 am CEST , second meeting of a month 17 CEST.
We would include EST in the second meeting and NZ time-zones in the first meeting
@defistaker @jankie1800 please keep this in mind for setting up next meeting(s).

(( __mcmmike__, __hendi__, __defistaker__, __cekickafa__, __dburkett__, __satoshcrat__ approved. ))

* __mcmmike__ : @defistaker @jankie1800 please keep this in mind for setting up next meeting(s).
 


<br/> <br/>
## Update on GRINMINT
<br/>

* __mcmmike__ : I would like to take this opportunity also share some news about the future of GRINMINT.

    I have also some great news, after talking to Quentin and Blockcypher , we agreed on keeping GRINMINT open until October 2021 as it is now.

    After October I will switch GRINMINT into an community GRIN mining pool, which also supports GRIN projects. We hope to make GRINMINT a counterweight against the big pools in China.

    I ordered a bit of mining equipment to kickstart the pool but we could need all your help supporting us.

* __cekickafa__ : very good news!

* __anynomous__ : Great news indeed!
 
* __ux041__ : Just to say "Pools in china" problem is going to be "pools in US" problem!:D

* __anynomous__ : So we kindly ask you all here for your support on giving Grinmint substantial mining power 🙏

<br/>

**Meeting adjourned.**
 

















 


 

 

