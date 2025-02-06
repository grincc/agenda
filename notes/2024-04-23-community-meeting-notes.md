# Community Meeting Notes April 23, 2024

Community Council (CC) meeting held in keybase grincoin#general channel. Meeting duration not explicitly stated, but inferred to be around 45-60 minutes.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_

* scilio
* cekic
* tromp
* anyn

# Short Summary

- Discussion and update on the MWixnet implementation, including its latest pull request with reorg protection, TOR support using Arti, and async/await support.
-  Acknowledgement of the completion of Milestone 3 tasks for MWixnet and a call for approval of payment.
-  Request for a forum post to inform the community about the current status of MWixnet.

# Agenda Points & Actions

*   Update on the status of the MWixnet project.
*   Request for a forum post to inform the community about MWixnet's current status.
*   Call for approval of payment for Milestone 3 tasks.

## MWixnet Implementation Update

__scilio__: Here's the latest pull request [https://github.com/mimblewimble/mwixnet/pull/22](https://github.com/mimblewimble/mwixnet/pull/22) It'll be marked as ready for merge once grin and grin-wallet are released with the new rust-secp256k1-zkp changes, but it's ready for review now. This PR includes: * Reorg protection * TOR support using Arti, the new rust native client * async/await support

__cekic__: This is the last phase right?

__scilio__: The milestone 3 tasks have actually been complete for a while now. These are just nice to haves, some of which were mentioned here [https://forum.grin.mw/t/request-for-funding-scilio-coinswap-implementation/9149#future-plans-5](https://forum.grin.mw/t/request-for-funding-scilio-coinswap-implementation/9149#future-plans-5) The others were just added later to improve testability

## Community Engagement and Milestone Approval

__cekic__: It would be good if more people joined this meeting. Topic added week ago, but I dont see any core or cc members or any other community member. I personally thank you for your contribution @scilio
+1 scilio, tromp

__scilio__: I had hoped we could vote for approval of payment, since all Milestone 3 tasks were merged long ago. But we lack a quorum here :)
+cekic, any

__tromp__: Thanks for all your hard work, scilio

__scilio__: np. Thanks for the patience on this project. It took much longer than hoped, but the end result was, imho, a clean maintainable codebase

__tromp__: Was your funding request targeted at the CC?

__scilio__: There was no targeted council, but the CC approved the request IIUC

__tromp__: I hope the CC can take the necessary steps toward approval of Milestone 3. How many are in active communication in the past month?

## Community Outreach and Testing

__cekic__: @scilio it would be good if you can make a forum post about mwixnet current status info, let the community know also, will be good.
+1 scilio

__cekic__: Anonymous and mike are active, others dont join meetings but reachable i hope. They will certainly see the forum post.
+1 anyn

__anynomous__: @scilio Thanks again for putting in all the extra effort to get a good set of tests and random reorg checks 🙏 . It looks like MWixnet is a solid implementation and it means a big step up for Grin as project in terms of privacy preservation 🎉 . I will do some last build testing when I have time, but I see no problem with moving towards approval since your implementation goes beyond what was requested 🚀 🦾.
+scilio, cekic

## *TO DO List*

* @scilio: Create a forum post about the current status of MWixnet.
* CC Members: Take necessary steps to approve payment for Milestone 3 of the MWixnet project.
*  @anynomous : Perform some last build tests of the MWixnet implementation.



**Meeting adjourned.**