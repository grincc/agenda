# Community Meeting Notes December 17, 2024

Community Council (CC) meeting held in keybase grincoin#general channel chat. 
 Meeting duration approximately 1 hour.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_

* anynomous
* wiesche
* cekic

# Short Summary

-  Discussion about a donation to grincoin.org, awaiting further feedback from CC members.
-  Feedback on difficulties in setting up and testing MWixnet, highlighting the need for improved documentation and troubleshooting.
-  Specific technical issues encountered by @wiesche while trying to run MWixnet on a Proxmox VM.

# Agenda Points & Actions

*   Donation to grincoin.org
*   Discussion about improved documentation and test cases for MWixnet.

## Donation to Grincoin.org

__anynomous__: Todays meeting agenda can be found here: [https://github.com/grincc/agenda/issues/151](https://github.com/grincc/agenda/issues/151)
Lets take 2 minutes to read the agenda, if there are any other suggestions for agenda topics, please let me know so I can add them.
Lets start with agenda topic 1 for today:
1) Donation to Grincoin.org
In short, I think a modest donation should be in place but I am waiting for more feedback from other CC members. Also I would welcome any feedback
community members here. What's your opinion on this @wiesche?
See here the
link to the discussion on the forum:
[https://forum.grin.mw/t/donation-to-grincoin-org/11415](https://forum.grin.mw/t/donation-to-grincoin-org/11415)
@wiesche If you do not have a particular view on it, that is also fine, jut le me know

__wiesche__: I use grincoin.org often and I think it is justified. I use the Api with GRIM and with my own projects.

__anynomous__: Ok, good to know. I think we all appreciate the contribution, the least we can do is compensate for material costs for the long run.
But that is just my own opinion,, … we need 4 CC onboard for funding.
Thanks for the input at least, maybe also useful if you express your opinion on the forum to give the thread a boost:
[https://forum.grin.mw/t/donation-to-grincoin-org/11415](https://forum.grin.mw/t/donation-to-grincoin-org/11415)

## MWixnet Testing and Documentation

__anynomous__: As for our second agenda topic:
2) Some community members request more detailed instructions with test cases to make it easier to get started mwixnet in layman terms.

__wiesche__: that is my point

__anynomous__: You mean the above agenda topic?

__wiesche__: the second point

__anynomous__: Ok, feel free to explain, you find the instructions to opaque/vague?

__wiesche__: I have install a grin node and a grin-wallet in a poroxmox ubuntu vm.

__anynomous__: In general I think testing is very ill defined since it can encompass anything. Ok, not familiar with poroxmox.

__wiesche__: proxmox..sry.
i have build mwixnet from sources in the VM
than i have run (instruction like git mwixnet)

__anynomous__: I will be honest, I have not looked at mwixnet for testing yet. But I think in general the idea is to spin up node+mwixnet+wallet, share pubkey with others to connect mwixnet nodes and start doing testnet transactions.
Ok, and all is good or running into issues at some point?

__wiesche__: one moment i share an image

__anynomous__: Ok, and your node is running? Ok, perhaps a configuration issue, did you look at the configurations shared on github?
Just to be sure, you did run "mwixnet init-config"

__wiesche__: yes, the mwixnet --testnet init-config cmd generate the toml

__anynomous__: You can check, if wixnet-config.toml exist, its configured
ok

__wiesche__: this is the config
.png
(Note: the image was not included)

__anynomous__: And if you opened, it does contain some key?

__wiesche__: The config refers to the key files and exists in the path.

__anynomous__: Ok, if you are running grin-wallet, does it also show a connection issue? I wonder if it is just mwixnet does have connection issue with the node, or also the wallet.

__wiesche__: grin-wallet is running as a service

__anynomous__: Ok, so grin-wallet is working like normal, but mwixnet has connection error, is that correct? Ok, so far so good.

__wiesche__: testnet owner_api is okay

__anynomous__: but then when you run mwixnet, you have that error?

__wiesche__: true

__anynomous__: Ok, I do not know what the issue might be. Perhaps something to do with grin node running on 0.0.0.0.13414 and not on 127.0.0. something....
This would be easiest to debug by comparing with someone who has it running
Did you ask on dev channel?

__wiesche__: no, not yet
i think it would be very good in principle if we could get a little more meat in the description. I'm a software developer myself and I'm having a bit of a hard time with it. So I ask myself, how can we get more people to test?
we don't have to solve the problem now.
i have seen that there is also a docker variant. Is mwixnet already installed and functional here?

__anynomous__: Ok, best to ask on grincoin#dev.
I agree with you that good documentation is key. Also troubleshooting between testing peers is key. We all overlook stuff and each OS has their own quirks.
Probably together as testers, we have to find the weaknesses in documentation and fix it.
Ok, I got to go now. Refreshing to hear a new voice at these meetings.

## *TO DO List*

*   CC: Further discuss and vote on the donation to grincoin.org.
*   @wiesche: Post technical details of the MWixnet setup issues on the grincoin#dev channel.
*   Improve MWixnet documentation and provide practical examples for easier setup.
*   Community : Testers compare notes and find issues in documentation and software to fix.


**Meeting adjourned.**