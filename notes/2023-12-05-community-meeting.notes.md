# Community Meeting Notes December 05, 2023

Community Council (CC) meeting held @ 18:30 UTC in grincoin#general channel on Keybase. Meeting lasted 15 min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.




### _Community attendance:_

* yeastplume
* cekickafa
* anonymous

# Short Summary
 
 
- Development update from @yeastplume about Gui wallet and node.


# Agenda Points & Actions
 

* Last meeting notes here: https://github.com/grincc/agenda/tree/main/notes

* Current meeting [agenda](https://github.com/grincc/agenda/issues/118)



## Open discussion

__cekickafa__ : Agenda is empty. No topic added.

__yeastplume__ : /😔

__anonymous__ : 👋  Wrapping some things up, so cannot lead this meeting. Hopefully soon I can join.

__yeastplume__ : I'll do quick core dev update

So the gui wallet now supports contracts workflow, supporting SRS, RSR and Self-spends
It also generates payment proofs by default, and I'm now adding functionality to view/copy/paste and verify payment proofs.


__cekickafa__ : RSR that is great!

__yeastplume__ : 
Then once that's all done, I'm going to clean up a few bugs and issues then hopefully issue an 'official' alpha point release of the core gui wallet with all of that experimental stuff in.
Ah, there's also support for mwmixnet in there, but it's untested and will  need some further dev

__cekickafa__ :in GUI ?

__anonymous__ : Cool, looking forward to that. The self spend is also for safe-cancel I assume.


__yeastplume__ : well, in the experimental 'contracts' wallet branch, and exposed to the GUI

__anonymous__ : I hope this new version will have less warning about future dependencies 😛

__cekickafa__ : well, will it be new year gift for Grinners ?


__anonymous__ : Not sure if it was only me, but I had a hard time compiling with the later versions of core and node on especially ubuntu

__yeastplume__ : I think I have updated warnings in the contract branch in the wallet, but the GUI is based on a swift-moving gui tech that's always changing


>__anonymous__ : Not sure if it was only me, but I had a hard time compiling with the later versions of core and node on especially ubuntu

we can look at all that, likely some packaging work once I start trying to bundle the gui


__anonymous__ : Sound challenging for development if the library underneath it is changing all the time. In any case, cargo.lock should avoid to much trouble with compiling, but I can imagine it is a hassle to fix all the code when they update the library each time.


__yeastplume__ : very much so, yes. and I think I need to do it again :D

__anonymous__ : Ouch, Hopefully not on to much of a regular basis 😅
In any case, it is all for the greater good. Perhaps the GUI for Grin also helps expose the needs for certain changes in the library.


__yeastplume__ : it's definitely led to a lot of changes and additions underneath to support it
I like it anyhow, think it works well. Not meant to dazzle anyone just be functional.

__anonymous__ : Well, that does sound like in tune with Grin's etos of minimalism and elegance.

__yeastplume__ : and runs the core node and wallet all in one, swaps between wallets and mainnet/testnet failry well

__anonymous__ : That is great, I always thought it would be beneficial to have the node and wallet bundled, with GUI even better.
Probably the most important thing for the project right now is simply that, a very solid well working easy to use default wallet/node

__cekickafa__ : it is only for windows or linux also ?

_yeastplume__ : ah, and I've tested PIBD on it numerous times.. catches up and works fairly consistently :D

__anonymous__ : Great!

__yeastplume__ : I've built this with windows as the first-order citizen, so will get to other systems in turn
it should work on others, but I haven't tested yet

👍cekickafa, anonymous

__anonymous__ : Ones it is all stable, we can even release a snap package (for Ubuntu) again. Have to ask quentin how to do that though

👍ardocrat 

## mwixnet Testing
I had some trouble. First compiling was a challenge, luckily @ardocrat helped me out with dependency issues and @vegycslol helped me out with NixOS, which works for some reason so much better than Ubuntu 22.04.
But since then I had very little time and my main computers starts having random crashes and hardware failures, which are taking priority to fix.
Did anyone else get the compilation of mwmixnet working and actually started testing?
@cekickafa Did you get around to it?

__cekickafa__ : That i couldnt started it. I am new to linux, but i will try to manage it.
are you testing it on windows?

__anonymous__ : First time I got it compiled I could not start it either, no errors during compilation, it just did not run. Then I made changes @ardocrat suggested, compilation looked like it was going well, then computer gave me a good old fashioned blue screen of death (Windows just updated the looks to include some sort of smily face, but it is as horrible as ever.

😨 chieves101, ardocrat

On virtual machines, but they do not like my hardware failing and my main OS shutting down all the time. So it is giving me some real headache.

__cekickafa__ : windows is blocking many things about Grin i suppose.

__anonymous__ : Not sure, my main issue is mostly dependenies related. So far NixOS is giving me the best experience after setting it up properly.

👍ardocrat 

__cekickafa__ : ubuntu i will try.

__anonymous__ : In any case it is a bit frustrating since I am severely time constrained and all these kind of issues block me from using the little time I have effectively.
I will continue trying though when I find the time.

👍ardocrat, mo5itoo 🎉

Cya all next time. Thanks for being here.
👋

__cekickafa__ : well, thanks for the update @yeastplume

__yeastplume__ : no worries, thanks for the meeting.





## *TO DO List*


* Mwixnet community testing




**Meeting adjourned.**