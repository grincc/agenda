# Community Meeting Notes July 2, 2024

Community Council (CC) meeting held in keybase grincoin#general channel chat, duration not explicitly stated, assumed to be around 30-60 minutes.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_

* yeastplume
* anynomous
* cekic
* ardocrat


# Short Summary

-   Discussion about the containerization of Grin and its subprojects using Docker and Kubernetes, aiming for easier testing of MWixnet networks.
-   Clarification on the Grin-GUI's build target, now exclusively against the contracts branch with a legacy transaction toggle.
-   Overview of new features in the contracts branch, including contract transaction flow, new proofs, safer self-send, and a partially implemented MWixnet.
-  Discussion on the prioritization of MWixnet testing over pay-joins in the near future.

# Agenda Points & Actions

*   Update on yeatplume's containerization efforts.
*   Review of the contract branch and its new functionalities.
*   Discussion of priorities for upcoming development tasks.

## Grin Containerization with Docker and Kubernetes

__yeatplume__: Anyhow... all of this is in service of Grin :D Taking a few weeks out here and there over the summer, but I've been getting grin and all subprojects containerized with the goal of being able to push up and pull down entire mwixnet networks for testing. Creating containers within docker is easy enough, but kubernetesing them is a bit more complicated, and I'm working through it

+1 cekikcafa, ardocrat

__anynomous__: A ok, well it should making testing a way more easy experience on the long run, but I do not envy you for having to figure out how to build and deploy those containers 😛
The work you do with docker is all on the contract branch right?

__yeastplume__: Everything docker related is just in the docker project (which I'll post for everyone else). Right now there are builds for both the main branch and contracts branch of the wallet, so you can configure and push up either)
that is this project here [https://github.com/mimblewimble/grin-docker](https://github.com/mimblewimble/grin-docker)

## Grin-GUI and Contracts Branch

__anynomous__: A ok. But the idea is at some point to switch Grin GUI to the contracts branch, is that correct?
Can you give us an overview of which new functions will be in there? I is contracts, mwixnet, bidirectional-payment proofs, a not very finished safe cancel (by phyro) anything else...?
I know it is all still very much in development and in need of testing, but I want to keep track of which functions are being worked on and in which stage of implementation they are.

__yeastplume__: Grin gui only builds against the contracts branch now, but you can turn legacy transctions on and off
if you choose contracts from settings, you get contract transaction flow + new proofs, safer self-send.
and mwmixnet is somewhat there, it just needs a test network up before it can be developed further

++1 any

__anynomous__: The safer self-send is basically a safe cancel by self spend (with downside of revealing you own the output right).

__yeastlume__: Yes, basically

__anynomous__: Ok good. I think it is by far the most simple solution. Better giving a way some information on an output you owned than allowing someone to possibly steal an output when you try to spend the same output to them. Simple solutions are often the best.
Will you also try to put pay-joins in the contract branch any time soon, or is that for the far far future?

__yeastplume__: that's likely in the future, really I'd just like to get mwixnet up and working first then see how we get on

__anyn__: I can imagine that is enough work. Thanks, just trying to keep track of things.

__yeastplume__: no worries.

__anynous__: Thanks for the update @yeastplume and for diligently pushing grin in the right direction 🙏



## *TO DO List*

*   @yeatplume: Continue development and testing of Grin containerization with Docker and Kubernetes.
*   Community:  Test and provide feedback on the Grin-GUI on the contracts branch, focusing on contract transactions, new proofs, safer self-send and MWixnet.
*   Community: Focus on getting MWixnet up and running, before addressing Payjoin functionality.


**Meeting adjourned.**