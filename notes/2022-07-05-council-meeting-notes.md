# Council Meeting Notes July 05, 2022

Community Council (CC) meeting held @ 10 UTC in grincoin#general channel on Keybase. Meeting lasted 85  min.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_

* anynomous
* yeastplume
* cekickafa
* defistaker
* phyro
* dtavarez
 

# Short Summary

-  Request funding for @cekickafa as groundskeeper is approved.
-  Request funding for @satoshocrat assistant groundskeeper is approved
-  GRIN Transaction Contract flow is discussed.


 

# Agenda Points & Actions
 

* Last meeting notes here: https://github.com/grincc/agenda/tree/main/notes

* Current meeting [agenda](https://github.com/grincc/agenda/issues/59)
  
  
  1) Request for funding @cekickafa; https://forum.grin.mw/t/request-for-funding-cekickafa-june-september/9823/5

  2) Request for funding @satoshocrat, https://forum.grin.mw/t/request-for-funding-assistant-groundskeeper-satoshocrat-july-sept-2022/9884?u=satoshocrat

  3)  TX Contract flow is discussed.
 
## 1)  Request for funding @cekickafa and @satoshocrat 



__anynomous__ : Our first agenda topic for today is:
1) Open discussion about TX Contract flow.


__dtavarez__ : I think we should start with the other topic which is a closed topic.

__anynomous__ : We can also do that.

__dtavarez__ : funding requests of  @satoshocrat and @cekickafa.

__anynomous__ : Ok, we modify the agenda, topic: 1) funding requests of  @satoshocrat and @cekickafa

__dtavarez__ : those two topics are pending for a while and I do not see any objection from the CC to both funding requests.

__anynomous__ : As you might noticed on the forum, there was some discussion on the funding request by @cekickafa since he did not explicitly mentioned the increase in salary, which was because the CC asked him to take on more tasks. That is all clarified now with good set of tasks matching the pay.
For @satoshocrat we did not hear any objections and have clearly discussed with him the tasks and proper pay.
In summary, from within the CC we agree with funding them both.

👍 dtavarez.

__cekikckafa__ : Thank you for your trust. I will do my best🙏🏽

__anynomous__ :  Does anyone object to these funding requests:
@cekickafa (1500 euro/month) - extended his tasks list
https://forum.grin.mw/t/request-for-funding-cekickafa-june-september/9823/22

@satoshocrat  Assistance groundkeeper ( 500 euro/month)
https://forum.grin.mw/t/request-for-funding-assistant-groundskeeper-satoshocrat-july-sept-2022/9884

Since I hear no objection, these two funding request are now approved.
Time to get to work boys.
Congrats @cekickafa @satoshocrat 🎉

🚀 defistaker, dtavarez 💓 cekickafa

__anynomous__ : We did not mention it yet, but we discussed with @jankie1800 that he will first make up for lost hours from his last funding request before putting in a new funding request. He had some personal circumstances that prevented him from making the hours before.

With that we can move back to the open topic for today:

## 2) Open discussion about TX Contract flow.

Current way of thinking, conceptualizing transactions is technocentric:

receiver-sender-receiver (RSR) flow and
sender-receiver-sender (SRS) flow.

New Contract flow, or SSS flow is focused on unifying the concept of a transaction to something like a contract. The name is not important, the way of thinking is, which unifies RSR and SRS and emphasizes the importance of signatures.
 
##New
Send – Sign -Sign (SSS) flow

```contract new - -send```

```contract sign - - receive```

```contract sign```

##Before

```grin-wallet send -d [address] [amount]```
```grin-wallet receive```
 
The purpose for this open discussion is just to hear some feedback on the Contract flow proposed by @phyro  What do you like about it, what do you not like about it. Is it any better than what we currently have?

To start with some feedback from myself, I do not like that the commands are longer now since the user needs to specify whether a transaction is --send or --receive. I do like that the SSS flows unifies the two transaction flows. I do not think a user needs to care who initiated a transaction, only they need to be aware that any unfinished transactions have to be cancelled before making a new one.


__dtavarez__ : when receiver types: 
```./grin-wallet --testnet contract sign --receive=0.2```

what happens exactly?

__anynomous__ : I have not plaid with it in real life, I assume you sign that you will receive a transaction of 0.2.

__phyro__ : yes, you agree on the received amount of 0.2 and you add your partial signature. The result is a slate containing this updated information.

__dtavarez__ : what is the input then?

__phyro__ :  with
 ```contract new --send=0.2``` 

you agree to send 0.2 Grin. To direct it at someone specific, you encrypt it for them (because there are no addresses) with 

```--encrypt-for=grin1abc...```

__dtavarez__ : the unsigned slate?

__phyro__ : yeah, it asks for a slate. It could have no signature or some partial sigs

__anynomous__ : The question would be what to do when multiple people send the same amount, or you just specify by the slate you copy in.

__dtavarez__ :  how will this looks like via tor?

__anynomous__ : Would it be automatically signed?

__phyro__ : I would separate transport from slate construction. This only takes care of the message/slate that we communicate to the other party, it doesn't know anything about the way of how this gets communicated. you can have a separate
```transport tor -d grin1abc```

and then you input the slate or smth.

__anynomous__ : Ok, that makes sense.
What do you all think of the contract flow 'conceptually'? For me it works easier since transactions are the same in requirements, they just need two (partial-)signatures.

__dtavarez__ : my opinion is that I like 
```safe-cancel```

__anynomous__ : In the end the target is to make life easier for all, including average Joe.

__cekickafa__ : I am trying to imagine like  a regular joe. 🤔

__anynomous__ : It should be just ```cancel``` IMO, every cancel for a transaction that has been partially signed should be safe. Users do not need to care, although you might get some people asking why a transaction fee was there.

__phyro__ : I think it's natural to merge SRS and RSR, especially when we go beyond 2 parties.

👍 anynomous

__anynomous__ : I mean, no one should have the option to make a unsafe cancel from my point of view, best to just simply avoid anything unsafe from being done. Only compromise would be to include a non-safe-cancel option which no user in their right mind should use.

💯 cekickafa

Exactly, I missed that point, but in the future interactive transactions and more than 2 parties will become more normal. In that case it is so much better to just think of transactions a a contract that requires multiple (partial-)signatures.

__dtavarez__ : I don't understand the insistence with RSR though.

__anynomous__ : By the way, above I mention partial signatures, again that is something not relevant for the user. We just use signature to keep things clean and simple in our descriptions.

__dtavarez__ : how will this work with more than 2 signers?

__anynomous__ : With multiple signers, it is not so clear who starts, who is second, third, etc. etc.
The point is, it should not matter. A transaction is nothing more than a bunch of information signed by people in a order. The person who has access to all signatures can submit. Transactions for a multisig could involve a lot of interactions if you want to make things safe, avoid modifications or giving power to last signer.

__phyro__ : 

>__dtavarez__ : how will this work with more than 2 signers?

at the moment, you can't guarantee the slate content won't change, but you can guarantee that you get the outcome you agreed to e.g. ```--receive=0.2```, even if there are 5 parties.

__dtavarez__ : to have this implemented we will just need to increase the slate version, right?
or do we need something else?

__anynomous__ : Guys, I have to go pick up my kids at school. I will read up later, looking forward to read all your opinions. Still, I have not heard yet any judgment calls, is this system better... I think so, but we need more feedback to know it this works for all.

👋 anynomous, cekickafa, defistaker, dtavarez, phyro


__dtavarez__ : I do not mind both parties having to pay fees, but I think by default the one paying for the fees should be the sender
unifying both flows is a win, and also the safe cancel advantage.

__phyro__ : to have the contract code implemented? I can't speak for grin++ because I'm not familiar with the code there, but yes, a slate version bump will likely be required. I'm also using this as an opportunity to cleanup the previous attempts. Grin historically had many different ways of building transactions that we were exploring and I think we can now start with a clean plate because we've learned over the years how we can make this process simpler.

__dtavarez__ : I also think this should work via Tor and/or BBS too.

__phyro__ : this does introduce 3 new api endpoints:
```new, setup, sign```

__dtavarez__ : grin++ relies mostly on the API.

__phyro__ : and has a rewritten logic of how you select inputs (favoring payjoins, always adding change output etc.), late-locking by default etc.

__dtavarez__ : it would be nice to have a RFC for this.

__cekickafa__ : is it better for merchants, net shopping plug in ?
both parties pays the fees.
it would be fine.

__phyro__ : the coin selection is wallet detail, but the slatepack construction changes would need an RFC. Potentially the APIs as well if we decide the endpoints should be unified in rust-grin and grin++
but I'm trying to push the code to some state first to see all the details and only after write RFC. If anyone is interested in details right now I'll gladly answer any questions.

__dtavarez__ : what are the constrains of the  ```receive``` param

__phyro__ :

>__cekickafa__ : is it better for merchants, net shopping plug in ?

not in particular. Today's invoice code works just as well imo. Maybe the part of "everyone pays for their own fees" might be better, idk really.

__dtavarez__ : ???
why ```receive``` is necessary?
it can be obtained from the slate, right?

__phyro__ : yes, for 2 parties, it can be derived from the ```slate.amount``` field. You can't do that for 3 parties because there's only a single amount field. It's up to wallet implementation really to define how this is handled. I'm in favor of having a flow that works for most/all of the cases we know rather than adding edge-cases for 3 parties or similar.

A wallet that used this as a backend could simply read the slate content, have a tickbox for ```auto-receive any amount``` and if that the case, read the ```slate.amount``` and call the ```sign --receive=slate.amount```

__dtavarez__ : again, grin++ relies on the API, so all of this it would be easier for me if I see it defined from the API perspective.

__phyro__ : so the core of signing is simple and you can decide how to call it on layers above that e.g. wallet UI can have the autoreceive logic
it's a prototype right now and so it has no API documentation. But if it ever comes to life, it will likely be similar to these structs that are passed in https://github.com/phyro/grin-wallet/blob/e5895dba42fe3bb758d267ecf764dc1826c8b3bb/api/src/owner.rs#L765-L800


__cekickafa__ : Meeting ends? @yeastplume has words maybe.

__yeastplume__ : sorry, something came up, nothing to add at the moment

👋 cekickafa.


## *Action points*

* RFC for TX Contract flow.
* Cekickafa as Groundskeeper,Satoshocrat Assistant Groundskeeper appointed.



**Meeting adjourned.**






























