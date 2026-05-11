6
Bank RRT :
IAO029107 Personal Loan Applications Failing Due to Vendor Experian Outage - P4
Impact - From 10:47 AM ET to 12:53. PM ET on 05/05,, we were seeing spike in latency in dpl-dlos-rules-processor-service. 327 applications are moved to v90 error queue.
Customers will be observing 5'Call Us page'
Root cause - It was due to experian vendor
Resolution- Issue was resolved by itself


7th

Card & Bank RRT:
IA0029131 - Customers are Experiencing Intermittent Errors for Several Applications - 3C
Impact: From 22:50 PM ET 05/06 to 12:05 AM ET O5/07, A firewall issue caused errors across multiple applications, resulting in intermittent login failures for Card and
Bank Account Center customers, access to AC Home L3 features and causing degradation of multiple applications. Total Critical Impacts:5,747 Discover Web and Mobile
Logins18, 592 AC Home L3 Features.
Root Cause: A network migration change caused a firewall failure, which disrupted dynamic IP updates and subsequently denied valid sessions.
Resolution: The impact was mitigated 'with a failback to SSB and the recycling of firewall services at 00:04 ET on 577.
Reconvene is scheduled at 12:00 PM ET today.





8th
CHG12654589
VENDOR CHANGE** TransUnion Contact Center, Fraud Prevention, Marketing, and Identity Services Maintenance Notice
Completed
Bank and Card RRTs:
IA0029145 - Multiple Applications Degraded due to AWS Issue - 3C
Impact: From around 8:00 PM ET on 05/07, Datadog monitoring and alerting, which remains available, but delayed by 10-30 minutes. At 2:00 AM ET on e5/08 we in Discover are
no longer seeing impact but Datadog has not closed their outage yet.
At 7:39 PM ET, 8:17 PM ET and 11:04 PM ET to 11:12 PM ET on 05/07, and from 12:23 AM to 12:24 AM ET on e5/08, we observe errors for Biometric logins.
Root Cause: The issue is due to a AWS outage. AWS is having an issue in East 1 Az 4. AWS is still experiencing continuous is sues with their server cooling infrastructure
at their US-East -1 AZ4 facility.
Resolution : Teams are working on a fix.
Next update from AWS is scheduled at 10:3am ET.
