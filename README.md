6Card RRT:
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

BANK RRTS
IAOO29970 - Bank Customers could experience technical difficulties accessing Home Screen on Mobile App. - P4
IMPACT - From 06:40 ET until 07:24 ET bank went into Lite mode due to which few Bank customers were unable to perform certain functions
across Discover Bank Web and Mobile applications. Discover Personal Loans were also experiencing errors. We observed issues connecting to
Finacle.
To mitigate the impact FIServices SOAP Gateway traffic was moved to the SSB data center.
Mitigation
RCA: It was dis covered that TLS 1.3 was accidentally unchecked on the BDC side specifically for the FI service, due to which application was
picking up the incorrect protocol (TLS 1.2). The Gateway team has manually re-checked the TLS 1.3 box for the FI service on BDC to resolve
the issue.
insights-eligibility- api - Non-Alert
IAO029965 for issues in
Issue: From 3:06am until 3:12 am ET 07/18, we have seen time out errors and traffic drop in insights-eligibility- api, it was due to Postgres
DB Connection failure (all connections got terminated) . During this time around 175 application calls were failed with status 50e.
Issue resolved by itself and we have dropped a mail to app team to investigate on the DB connection issue.


