
# Community Meeting Notes October 25, 2022

Community Council (CC) meeting held @ 10:00 UTC in grincoin#general channel on Keybase. Meeting lasted 40  min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_

* yeastplume
* cekickafa
* phyro
* defistaker
* vegycslol



# Short Summary
 
- [Release v5.2.0-alpha.2 and testings](https://github.com/mimblewimble/grin/releases/tag/v5.2.0-alpha.2) focus on future testing and upgrade to V.5.2.0 

# Agenda Points & Actions
 

* Last meeting notes here: https://github.com/grincc/agenda/tree/main/notes

* Current meeting [agenda](https://github.com/grincc/agenda/issues/70)







First agenda point:



##  1) Release v5.2.0-alpha.2 and testings


__cekickafa__ : We have one topic.     #1) Release v5.2.0-alpha.2.

__defistaker__ : Congrats on new release 🎉🎉

__phyro__ :  perhaps @yeastplume can give a brief description the state of the release and whether we want some testing done etc.

👍 cekickafa

__cekickafa__ : Meeting is about Release v5.2.0-alpha.2 and testing. @yeastplume has words imo.


__defistaker__ : Yes, please. 
For testing, I would like to ask if it should be synced fully in archive mode before dropping the connection for one week?



__yeastplume__ : Sure, well I don't have too many other words other than what I've already said above. The 5.2.0-alpha.2 release has fixes, all of the changes for PIBD enabled on testnet only, and updates seeds for both testnet and mainnet
So please test syncing nodes from scratch on testnet, as well as resuming them after leaving them offline for more than a week. The only problem is that testnet isn't moving at the moment, so that's going to impact testing
We're also very close to being able to start implementing and testing transactions on the gui wallet, but of course it would be very helpful to have testnet moving in order to be able to support that.

👍 cekickafa, johndavies, anonymous, satoshcrat

__cekickafa__ : Well those test miners will be shipped but it will take some time, customs, shipping etc. So it might take couple weeks. Do we need that test miners urgently ? Do we need to turn on some miners for testing until those miners arrive?

Is there any test mining  at the moment i dont know. All down?

__yeastplume__ : it's not super urgent, there's other things can be done on the gui but it affects testing overall. the last block was sept 30th.

__cekickafa__ : 👍 yes, sooner better.

__yeastplume__ : I'll also just point out this again https://grintools.revcore.net/seedcheck/

__cekickafa__ : we need 7?

__yeastplume__ : those are the seeds in alpha.2, I just want to know who prokapi is and whether we should remove them

__cekickafa__ : Can be @hendi ?

__yeastplume__ : possibly, that would be a good guess.

__cekickafa__ : well i DM'ed him about testing but he didnt reply. He might be at vacation, etc.

__yeastplume__ : sure, if you could just let us know when he does reply.

__cekickafa__ : Ok, sure.
So we need 7 for main and 5 for testnet. When test miners arrive, it would pass 5. And it is enough ?

__yeastplume__ : Yes, that would be plenty, I think.

__cekickafa__ : Ok. Lets search community  for main seed then :)
Anything more ?

__yeastplume__ : all good here

👍 cekickafa

__cekickafa__ : Again Congratulations on v5.2.0-alpha.2  new release 🎉. Thanks for efforts  @yeastplume

👍 mably, yeastplume ,satoshocrat

__vegycslol__ : What kind of transaction building will the new gui implement? Contract or as it is now?

__yeastplume__ : as is now, but I think we want to play with both

👍 mably, phyro 

__cekickafa__ :  Thats all i think. Thank you all 👋

__vegycslol__ : 👋


## *Action points*


* Get testnet miners functional asap.
* Test syncing nodes from scratch on testnet, as well as resuming them after leaving them offline for more than a week.


**Meeting adjourned.**