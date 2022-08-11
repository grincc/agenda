# Council Meeting Notes July 19, 2022

Community Council (CC) meeting held @ 15 UTC in grincoin#general channel on Keybase. Meeting lasted 82  min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_

* dtavarez
* yeastplume
* cekickafa
* defistaker
* phyro
* deeev
* MCMMike


# Short Summary

-  Status of current GRIN Testnet  is discussed.
-  Running a Faucet for testnet purpose is discussed.
-  Number of seed nodes is discussed.


 

# Agenda Points & Actions
 

* Last meeting notes here: https://github.com/grincc/agenda/tree/main/notes

* Current meeting [agenda](https://github.com/grincc/agenda/issues/61)
  
  
  1) GRIN TESTNET

  2) Open Discussion

 
 
## 1) GRIN TESTNET


__dtavarez__ : Hello! One minute to review the agenda https://github.com/grincc/agenda/issues/61

if anyone has other suggestions, now is the time
suggestions for today's agenda.


__deeev__ : Whats the deal with grin testnet? Block production is unstable?


__dtavarez__ : 3 things.

1- Seeders

2- Faucet

3- just make sure we keep mining Testnet

__phyro__ : so what's the topic of discussion now, the seeders first?

__yeastplume__ : we have a list of seed nodes. I was going to merge them into the next alpha release (but I'd like the couple of outstanding issues that are filling up resource descriptiors or causing nodes to stop to be addressed first(

 👍 phyro

__phyro__ : there was also one PR opened https://github.com/mimblewimble/grin/pull/3710

__yeastplume__ : sure, but I'm going to run through the list closer to release time and test them all

👍 dtavarez

__phyro__ : yes, i agree.

__MCMMike__ : 
>_yeastplume__ : we have a list of seed nodes. I was going to merge them into the next alpha release (but I'd like the couple of outstanding issues that are filling up resource descriptiors or causing nodes to stop to be addressed first(

you mean the mainnet seed nodes or testnet , as we from Grinnode will provide some relyable test-nodes soon as well. 
We are already in the DNS seed for mainnet and could provide some stable nodes for testnet also
btw 👋

👋 cekickafa, deeev

__yeastplume__ : nodes for both testnet and mainnet
will be changed/updated on the next release
https://grintools.revcore.net/seedcheck

And at the moment, there are no working testnet seeds at all
I can test and merge what we have into main anyhow so at least those building from source and testing will have it. We just want to make sure the list is finalised before the next release.

__dtavarez__ : We could ask again in the forum for seeders
but as long as the seeders shipped in the code works, we should be fine.

__phyro__ : as far as I understand, the seeds hardcoded in the last release don't work, you'd have to modify the code with new seeds (e.g. from the PR above), build it and then it would work.

__dtavarez__ : what amount of seeders do you think should be included? 5? 4?

__phyro__ : I don't have a strong opinion on this, 5 sounds good

__yeastplume__ : as many as we can get.

__dtavarez__ : that's then a goal.

__yeastplume__ : 5 sounds like a good goal

__dtavarez__ : awesome :) next... the Faucet...
last time I checked the faucet run by Quenntin was not running.
I think it would be good to have one running.

__cekickafa__ : @hendi was running a one?

__phyro__ : haven't used the faucet for a long time so don't know if it's working now or not. It's definitely good to have one available.

__dtavarez__ : I think we could continue to encourage the community to test heavily the wallet and the node.
last time I checked it was not working.
what I want to achieve is a healthy testnet playground.
last time we ran a QA "campaign" as a success I think we would need to do it again soon. The more eyes the better. And having a healthy testnet is the first step IMO.

💯 mo5itoo

__cekickafa__ : well, it became weird when there is 2 meeting simultanously i think:)

__dtavarez__ : to wrap up this one; the minimum amount seeders (testnet) to be hardcoded is then 5.
thank you for your time.
I'm out 👋

__yeastplume__ : woah, no we're not hardcoding a number of seeders, we're aiming for at least 5
if we don't have 5 we don't have 5.
sorry, read that as 'hardcoding 5 as the number of seeders'

__cekickafa__ : So the action point is to have at least 5 seed nodes.

__yeastplume__ : a goal, if possible

👍 cekickafa, dtavarez.

__cekickafa__ :  There is open discussion, has anybody words? or end meeting for note keeping?
ok. thank you all 👋

👋 cekickafa, deeev , renzokuken , satoshocrat , yeastplume.



## *Action points*

* Goal is at least have 5 seed nodes.
* Encourage the community to test wallet and node.
* Have running Faucet for testing. 




**Meeting adjourned.**






























