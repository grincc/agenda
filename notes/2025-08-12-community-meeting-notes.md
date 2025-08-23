

**Community Meeting Notes August 12, 2025**

Grin Governance Council (GGC) meeting held in Telegram @ 22:30 UTC. Meeting lasted approx. 65 minutes.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

**Community attendance:**

* transatoshi
* cekic
* wayne
* wiesche
* bluegecko
* mammothine


**Short Summary**

*   Clarification was provided on the GGC fund, confirming it is a merger of the 41.52 BTC from the OC fund and the 22 BTC from the former GrinCC fund.
*   Members discussed ongoing node synchronization issues, with users experiencing slow speeds and a low number of peers.
*   The funding proposal for an Umbrel/EmbassyOS Grin node by `@wiesche` was discussed, with a call to finalize the community vote.
*   A new community member, `@bluegecko`, announced plans to build a dedicated Grin exchange (`grin.exchange`) to address recent delistings, receiving positive community feedback.
*   `@transatoshi` shared a completed Ansible playbook for deploying Grin nodes and announced a new "memes for tips" site https://suchgrin.lol/ to encourage engagement.
*   The `grin.mw` website was reported to have  access and certificate issues.

**Agenda Points & Actions**
## Follow Up.
- _Fixing peers_, [grin++ node bans Rust nodes](https://forum.grin.mw/t/funding-proposal-pibd-implementation-in-grin/11583/2).
- [Payment proofs ](https://forum.grin.mw/t/grin-product-wishlist/9704/61) fix.
- Grin [Github organization](https://github.com/grincc/agenda/issues/177#issuecomment-2973518577).

Current meeting agenda https://github.com/grincc/agenda/issues/186

* Topics discussed were:
1.  GGC Fund Composition
2.  Technical Discussion: Node Sync Speed & Peers
3.  Umbrel/EmbassyOS Funding Proposal Update
4.  Grin Website (`grin.mw`/`gri.mw`) Status
5.  New Project: `grin.exchange`


**GGC Fund Clarification**

transatoshi: Question, so I see the 41.52 BTC from the GrinCC fund in the multisig, I wasn't expecting the deposit of 22 more BTC, was that from the OC fund or something.

cekic: 41 btc is OC fund. Grincc is 22 btc

transatoshi: Thank you for clarifying, since we have merged the OC + CC it is just considered the same fund now, right?

cekic: yes true

## Technical Discussion: Node Sync Speed & Peers ##

cekic: There is no topic added for agenda. Since title is technical meeting, that slow synch and peer issue persists for me generally. It was synching more fast before. Anybody has such issue lately ?

wayne: @cekic (Since title is technical meeting, that slow synch and peer issue persists for me generally. It was synching more fast before. Anybody has such issue lately ?) Is that with grin-node?

cekic: yes, before 6 peers, now hardly i can catch 1-3 peers. It takes about 10-12h.

wiesche: Today synchronized from 0 with grim (10 Hour)

transatoshi: I get about the same result, maybe a little quicker since I'm right next to a big IXP

wayne: I synced a grin-node a few days ago. It got stuck for a while after a few hours but a restart got it fully synced after a few minutes on limux

cekic: @wiesche well hope so. Or is it related that isuue of grin++ banning rust nodes? https://forum.grin.mw/t/funding-proposal-pibd-implementation-in-grin/11583/2

## Umbrel/EmbassyOS Funding Proposal Update ##

wiesche: @ckeci https://forum.grin.mw/t/funding-request-grin-node-meets-umbrelos-embassyos/11928 I hope this will help

transatoshi: I also have ansible playbooks for deploying mainnet and mwixnet/testnet nodes. Ansible is maybe easier to set up than docker for those not technically inclined. I do support this work being done though.

wiesche: @trans UmbrelOs makes it user-friendly. In the background with docker

transatoshi: @wiesche > transatoshiツ: Ah gotcha, not too familiar with Umbrel. Is it just a generic OS to run on anything, or meant for like little NAS devices?
👍 wiesche

wiesche: There is own hardware or raspberry

transatoshi: Looks easy to use from a 2 minute browse of their site.

wayne: Wiesche, where are we at with regards to your proposal of work? https://forum.grin.mw/t/funding-request-grin-node-meets-umbrelos-embassyos/11928/18
I suppose we need a formal vote

wiesche: A few thumbs up are still missing. I would start the work in 2 weeks.
👍lepooh, broyoudontknw, cekic, wayne, transatoshi

cekic: well no objections from forum community.Summer time effected particiaption it looks like:
👍 wiesche

wiesche: The survey is in private chat

cekic: forward in public chat here and get voted. Topic is already on forum public.

transatoshi: @wiessche If there is anything I can do to make the work go faster I am willing to help or do testing for you.
👍 wiesche, cekic, broyudontknow

wiesche: I think I'll be ready by the end of September @transatohsi
👍 broydntknow, cekic

## Grin Website Status ##

bluegecko: nvm grin.mw is working now lol

transatoshi: Works for me

bluegecko: thank you to whoever fixed it.

transatoshi: I usually ping Tromp to help when I update the site, he has access.

wayne: It didn't work on my linux machine a few days ago

transatoshi: I believe it is just a Github pages type setup if I am not mistaken, so too many redirects seems like an odd error to have

bluegecko: the download page still isn't working

wayne: It said that the certificate has expired

wiesche: @transatsohi Do you do the hosting for gri.mw?

@wayne Probably need to clear your cache



transatoshi: No, that's ardocrat's domain. I know he is on vacation so it might be a minute before the site is back. I'll ask him if this is mirrored to his gitlab. https://github.com/GetGrin/grim
👍 wiesche , bluegecko

wiesche: ok

transatoshi: I just host grinminer.net grinchat.mw grin.ceo For now

bluegecko: lol. gri.mw is down for me too

## New Project Announcement: grin.exchange ##

bluegecko: I saw TradeOgre delisted and I don't have Gate.io access. I'm building a Grin exchange (grin.exchange) so we can have a dedicated exchange where people can trade won't have to worry about delistings anymore
🔥 lepooh, huell, cekic, broyoudontknow, wayne, transatoshi, wiesche, mammothine

cekic: are you from Nonlogs or ? @bluegecko

wayne: @bluegecko Wow, super cool domain. How will it work? Would you run it alone?

transatoshi: Is it going to be slatepack based like TO?

bluegecko: no I just kinda got into Grin recently. I'm this guy: https://x.com/grincryptolab
Used to be an exchange on zksync called ZigZag Exchange. decided to pivot to Grin because I like it so much

> @wayne for now running it alone yes

>@transatoshi: tbh I have to read more into Grin to figure that out
not sure how people have been doing addresses

checking the docs now, and ya I think it will be
that seems like the best one.
 👍  transatoshi

transatoshi: Adresses are generated by the wallet, but are transported over TOR, so using slatepacks which are just a string of code is much better
👍 bluegecko, wiesche

wayne: A working single centralised exchange would be a massive support for the project now
👍 wiesche

bluegecko: ok. ya my plan is to only support Grin not even worry about anything else

mamothine: what pairs are you thinking?

bluegecko: > Blue Gecko: GRIN/ETH, GRIN/BTC, GRIN/USDT
Maybe just GRIN/USDC to start. whatever people use.

transatoshi: I can also provide hosting if it is needed, I am running several Grin services already.
👍 cekic

bluegecko: sounds good man. thank you.

cekic: looks cool. you are welcome to Grin
👍 wieshce, bluegecko

wayne: Yeah definitely reach out whenever you need support. It's worth creating a post on the forum

bluegecko: ok I'll do that

cekic: Yes,anytime you can ping here also if needed.

bluegecko: Thanks

wiesche: @bluegecko When are you planning to launch the Exchange?

bluegecko: Whenever I can finish the code lol. Maybe October or so
💛 wiesche, cekic

## Community Tools and Contributions (SuchGRIN.lol meme microtipping site) ##


transatoshi: I am going to be making a memes for tips site very similar to suchwow.xyz except without needing to make an account. You'll be able to post memes with a slatepack address or email/TG/etc for manual slatepacks so you can receive tips
💛 wayne, mammothine, bluegecko, cekic

cekic: Summer breeze tonight lol 💛
🙂 wiesche

transatoshi: I figure that'll drive a bit of engagement with Grin and also be another way to obtain free Grin along with my faucet. Got the Grin node as a service playbook done
[Ansible playbook code omitted for brevity]

Got the Grin node as a service playbook done

- hosts: test
  remote_user: root
  tasks:

  - name: Create user grin
    ansible.builtin.user:
      name: grin
      group: grin
      password: <SHA-512 HASH>

  - name: Download grin
    get_url:
      url: https://github.com/mimblewimble/grin/releases/download/v5.3.3_rebuild/grin-v5.3.3_rebuild-linux-x86_64.tar.gz
      dest: /tmp/grin.tar.gz
      mode: '0775'
      force: 'yes'

  - name: Extract grin
    ansible.builtin.shell:
      chdir: /home/grin/
      cmd: tar xf /tmp/grin.tar.gz

  - name: Download grin-wallet
    get_url:
      url: https://github.com/mimblewimble/grin-wallet/releases/download/v5.4.0-alpha.1/grin-wallet-v5.4.0-alpha.1-linux-x86_64.tar.gz
      dest: /tmp/grin-wallet.tar.gz
      mode: '0775'
      force: 'yes'

  - name: Extract grin-wallet
    ansible.builtin.shell:
      chdir: /home/grin/
      cmd: tar xf /tmp/grin-wallet.tar.gz

  - name: Creating an empty file
    file:
      path: "/etc/systemd/system/grin-main.service"
      state: touch

  - name: Set up service for Grin node
    copy:
      dest: "/etc/systemd/system/grin-main.service"
      content: |
        [Unit]
        Description=Grin Mainnet node
        After=network.target

        [Service]
        WorkingDirectory=/home/grin
        User=grin
        Group=users
        #PrivateDevices=yes
        #Type=simple
        ExecReload="/bin/kill -HUP $MAINPID"
        KillMode=mixed
        KillSignal=SIGTERM  
        TimeoutStopSec=60
        ExecStart=/home/grin/grin server run
        Restart=on-failure
        RestartSec=30

        [Install]
        WantedBy=multi-user.target
        Alias=grin-main.service

  - name: Enable service grin and ensure it is not masked
    ansible.builtin.systemd_service:
      name: grin
      enabled: true
      masked: no

  - name: Make sure a service unit is running
    ansible.builtin.systemd_service:
      state: started
      name: grin



👍  ardo, anonymous

cekic: great! you are on steam my friend

wayne: Such a fun looking site

transatoshi: It is awesome, I have made way over 1,000 Wownero from posting memes.


wiesche: @bluegecko  When are you planning to launch the Exchange?

bluegecko: Whenever I can finish the code lol. Maybe October or so

💛 wiesche, cekic

**TO DO List**
* Vote for Umbre/OS bounty proposal.

🔨 

**Meeting adjourned**
