# Community Meeting Notes July 30, 2024

Community Council (CC) meeting held in keybase grincoin#general channel chat, duration not explicitly stated, assumed to be around 30 minutes. Meeting not explicitly held but notes provided by groundkeeper.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_

* yeastplume
* cekic

# Short Summary

-   Update from @yeastplume on advancements in MWixnet and the Docker project.
-   Docker project now capable of setting up a full node-wallet-MWixnet network for both Testnet and Mainnet.
-   Work in progress to expand the network setup to include multiple MWixnet nodes on Testnet, allowing for GUI wallet transaction testing.


# Agenda Points & Actions

*   Update on MWixnet and the Docker project status.
*   Discussion on future expansion of the network setup.


## MWixnet and Docker Project Update

__yeastplume__: Probably not around for any meet later, but quick update. I've made a few fixes to mwixnet and the docker project can now throw up a whole node-wallet-mwixnet node network with a basic gui monitor for both testnet and mainnet.

## Expanded Network and Testing Plans

__yeastplume__: I just want to extend it to a node-wallet then 3x mwixnet node network (on testnet), then I can start working on throwing txs into it from the gui wallet. Docker project should be good for testing as well as anyone who wants to quickly host a mixnet node



__yeastplume__: I've been educating self on kubernetes as well and have a cluster running locally. I can see an argument for having a version that launches into a kube cluster as I think that method of deployment is going to be more and more popular, but it's much, much more complicated to work with than docker and I don't think it's going to be much use for regular users right this moment.

__yeastplume__: It might be worth creating a helm deployment (an app deployment-templating tool that's popular). I might get around to doing it for my own grin deployments given I'm running my own cluster, but not a priority or anything

## *TO DO List*

*   @yeastplume: Extend Docker project to support a node-wallet and 3x MWixnet node network setup on Testnet.
*   @yeastplume: Begin transaction testing with the GUI wallet.
  
