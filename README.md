16

IABeBe587 - Some Discover Card Customers Are Unable to View Balance Transfer Offers or Manage Cards - P4 (Reconvene is Schedule at 2pm ET on
9/16)
Impact: From 1: 26 PM to 2:05 PM ET on 9/15, Discover Card members experienced intermittent failures when attempting to view Balance Transfer
offers or perform Card Management functions. The impact is minimal.
Root Cause : The issue was caused by WebSphere application servers reaching 100% disk space capacity across both data centers, driven by
high-volume Log4j debug logging in system. out. log files from supporting backend services (eContact, eCommProfile, and Account Data Service).
Resolution: Temporary fix to mitigate the impact
1) MidOps manually cleared and compressed archived log files, restoring disk availability and allOwing customer error rates to subside back
to normal thresholds.
2) Storage Expansion: Infrastructure teams (UnixOps, Storage, and Winops) executed automated and manual disk space expansions (increasing
file systems from 82 GB up to 150 GB) across all 24 Websphere nodes to provide an immediate operational safety buffer.
Permanent Resolution to fix the issue - On 9/14 this CHG12502376 - Card, Bank: Card Code Install went into production, The Digital Card Bank
Release team executed e Com profile application rollback in coordination with the bank release maintenance window.


17th
IABO38600 - Bank Tier2 Catchpoint failing - P4
Impact: From 11:86 PM ET on 89/16 to 3:56 AM ET on 9/17, Message an Agent option is missing from Bank Help Center page. No errars ere
observed in the Help Center endpoint.
RCA: Message an agent option was suppressed as per business requirements, hence closed RRT
Resolution: We asked the catchpoint team to remove that step, and they removed it hence catchpoint runs Successfully.


18th
Bank RRT:
Issue: From 84:10 - 10:56 AM ET 09/18, Discover customers were unable to make a personal loan payments via web, they were seeing a blank
IAB03e622- DPL Payments issue on web - p4
screen. 84 unique customers were impacted
RCA: Issue is due to a recent UI deployment CHG12743376, CHG12743389.
Resolution: Issue resolved post back out of the UI Changes.
Digital Payment Enablement Customers Experienced LNP and LCM Failures Across Multiple Wallets -P4
Card & Bank:
Inpact: From 7:30 AM ET to 11:10 AM ET 9/18, Observed Intermittent error spikes were observed briefly affecting multiple applications (IVR,
IAOB3624
Action, Orion, Atlas Rewards) . Most application impact subsided by 11:10am ET or retry logic was in place. No customer impact.
Cause: Identified CHG12743028 caused ingress routing latency and HAProxy node degradation on the East Prod 1 cluster.
Resolution: inpact was mitigated by flipping traffic avay from EAST Prod 1 cluster. At 4:55 PM ET the daemonset which was installed via
CHG12743028 was rolled back from the East Prod 1 cluster.
-api - NA

19th
Bank RRT:
IABƏ3OS36 - Some Customers Experiencing Blank Screens on Web DPL Payments - P4
Inpact: from 7:48 AM ET to 18:05 AM ET, the payment processing system for Discover Personal Loans is experiencing an issue, inpacting
customers attempting to make dpl payments . 98 unique cust omer were impacted
Cause - This is related to IA0030622, after backout of their install, Akamai cache was not purged, which caused the issue.
Resolution - After the akamai was purged the errors were stopped.

