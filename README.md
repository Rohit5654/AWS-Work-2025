Pre-Migration
Migration Window
Post-Migration
Before, Sunday, March 22nd 2:00 AM EST
Sunday, March 22nd 2:00 AM EST-Monday, March 23rd 3:00 AM EST
After, Monday, March 23rd 3:00 AM EST
Status of Migrating Accounts identified in Finacle:
Bank Lite Mode enabled between:
Migrated Customer status:
oSCHEDULED
o Sunday, March 22 2:00 AM - March 22 8:00 AM ET
If all acCOunts of customers are with COF:
Status of Non-Migrating Accounts in Finace:
Migratihg Accounts deactivated from Discover:
"MIGRATED"
NOT STARTED"
o Accounts marked as "IN PROGRESS" in Finacle.
If some accounts of customers are with COF:
o Finacle Team will manually run the processes for this.
Most features suppressed by March 20, 5:00 PM ET
o "PARTIALLY MIGRATED"
(Friday).
Migrating Customers will view a static page stating,
Credential Migration phase begins.
their account is being setup in COF.
Migrating Customers view a banner with relevant
timelines from March 17th on:
Non-Migrating Customers will see scheduled
maintenance notification.
o Limited feature availability.
o Transfer of account to COF under process.
Non-Migrating Customers can resume BAU activities
from March 22nd, 8:00 AM ET after Bank Lite Mode is
Non-Migrating Customers viewa banner with
disabled.
relevant timelines on:
o Scheduled maintenance.
COF will provide a Sign-Off after receiving Migrating
Account info on their end.
O Finacle Team manually sets Customer status to either
"MIGRATED" or "PARTIALLY MIGRATED".
Internal







*****
16th

Card and Banik RRT:
epact : From 10:40pa until 11:45pm ET on 3/15, customers experienced issues logging in to both the Discover Hobile App and Web Account Center for bth Card and Bank. A total of 3,194 unique custo
ctud
LABO28375: Web and Mobile Login Degraded- P3
Cause: The technicel root cause of the issue remains unknown, and will be investigated offline by the Digital ngineering Citadel team. when they were changing the remote database configurat ion in preparation for
by the issue hen attempting to access their online accounts.
CHG12586388 and CHG12587327 (Database Migrations in the SSB) resulted pods going in crashloopbackoff and had an inpact .
Resolution: To resolve the issue the Comand Center failed traffic over session-auth- api traffic to A/A at 11:45pa ET, and the Digital Engineer ing Citadel team reverted the remote database configuration
ange de
in preparation for the database migration changes. CHG12586388 and CHG12587327 were cancelled to prevent further impacts .


19th
Card and Bank RRT:
IAB828415: Multiple Applications Experiencing Degradation in AWS-USEAST1-PPP-APPS-PROD-1 Cluster -- Mítigated
AION Sit ID: SITeS7812
Inpacted Area (s): Payments
Capital One Severity: 4
Level of Impact - Payments: Medium
Impact: Multiple Global Payments Network applications were experiencing intermittent degradation or unavailability in the AWS-USEAST1 - PPP -APPS - PROD-1 cluster. From 12:3@pm until 5:30pm ET on 3/18, ITP enrollment
was sporadically degraded causing 72 unique customers from landing on the ITP page.
Update: Impact is mitigated. OCP Operations completed the rolling restarts of the infrastructure nodes in the AWS-USEAST1 - PPP -APPS-PROD- 1 cluster. oCP Operations has opened cases with vendors Calico and Red Hat to
investigate the root cause. Command Center will monitor the situation overnight, and will check with OCP Operations for a status update by 3/19 12 :00pm ET.
fiext Update: 3/19 1:00pm ET
IAB028429- Datadog Degraded - P4
Inpact: From 3:16pm until 10:53pm ET on 3/18, Datadog reported an issue causing some metric monitors to intermittently report a "No Data" status. This primarily affected monitors based on dístribution metrics.
Multíple critical and key core application teams were engaged and saw no degradation to their monitoring in Datadog. There were no reports of impact during this tine.
Cause: Due to an internal issue with vendor Datadog caused by a change.
Resolut ion: Datadog backed out the change to resolve the issue.

20th
IA9028458 - bankaccountsapil- backend service time outs - NA
We were paged for an CCBM alert ibankaccountsapil service time out, it was a momentary spike due to latency from downstream service. Also we didnt observe any errors in bank mobile achome journey datadog dashboard.
TAD02B474 - Bank Debit Card Management (Non Transaction) Degraded - P3
Impact: From 2:14pm until 3:23 pm ET on 3/20, 780 total unique Discover Bank customers experienced sporadic debit card freeze/unfreeze functionality errors via web and mobile. All other debit card functonalities
ere not impacted.
Cause: Root cause is under investigation by Tea Monarch. A case was opened with Vendor FIS.
Resolution: Impact subsided without support intervention.
Increase response spike in bank-migration-service - Non-Alert
TAB028476 for


22th


Bank RRT:
IAB028488 seeing errors in cd-retn-closure - api - P4
From 10; 20 PM on 3/21 to e3:15 am Et on 03/22 we are seeing errors in the cd-retn-closure-api JVM in the west side where there is no live traffic
Cause - The'issue is in the health che ck calls, which are failing in west-prod1 and prod2 pods. This does not have any customer impact.
Resolution - OCP ops and app team is working on a fix.

IIAO028490- Bank Tax Documents Downloads Degraded- Resolved- P4
Impact: From 10:46pm ET on 3/21 until 2:00am ET on 3/22, 690 Discover Bank customers were unable to download bank tax documents.
--Vendor Inflicted- Due to maintenance on vendor Thomson Reuters" end that wasn't communicated to Discover.
Cause:
Resolution: Impact subsided without support intervention.

IAB028509- Freeze and Unfreeze issue- NA
from 11:44pm to 11:56pm ET on 3/22, Discover Bank customers experienced sporadic debit card freeze unfreeze functionality error. This issue is related to IA002 8474 which happened on the 3/20. A case was opened with
FIS (CSe68657 19), to help understand the root cause of the issue. The impacts are very low, so this is a non-alert issue.




