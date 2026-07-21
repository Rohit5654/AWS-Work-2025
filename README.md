Card RRT:
IAee29935- Multiple applications are experiencing ongoing latency, high error rates, and request timeouts. - P4, Resolved
Issue: From 1e: 10 AM ET to 10:26 AM ET on 7/15, Multiple Card Applications experiences connectivity issues and increased latency. Card
Inventory Service 3 Suffered a prolonged outage until it was manually restarted at 10:26 AM. It had stopped taking traffic on the SSB side
(both internal/ INT and IHS instances) . Mobile API & Digital Portal: Experienced a 2-minute latency/error spike. CVS Payment s saw a high
error rate that subsided by 10:12 AM.
Impact Counts: Account Center Logins (Web & Mobile) - 2,181 Non-unique errors. Mobile Card ACHome Errors - 556 Non-unique errors.
Cause: A network backbone failure between Chicago and columbus that caused the BGP connections between major routing head ends to drop
disrupting communication with the mainframe services. This network instability caused transient latency spikes and error rates across
multiple applications.
Resolution: Network connectivity was restored, and we manually ripple started cardinventoryservice3 in IHS and INT SSB, which re-established
mainframe connectivity and recovered services. This issue is currently being investigated under Cisco Tac Case #701096523.
