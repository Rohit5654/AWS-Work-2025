Bank RRT:
IAO030204 - Debit card freez and unfreez degraded - P3
Impact - From 10:45 PM on 08/09 to 11:40 AM on 08/10, Customers were unable to freeze or unfreeze their debit cards via mobile and web.
RCA - Downstream vendor failure FIS / OnDOT
Resolution Vendor resolved their internal issue.


PpappPS-prod-1
Ount-center- login-restr-prd -- Completed
CHG12715332 - Mobile i0S/Android App Launch
2615.0 (Day1) -- Wi1l start at 12:30 ET
ns talls
IAO30235 - Some Discover Bank Customers Are Unable to Access Cashback Debit Accounts via the Mobile Application - P4
From 1: 54 - 06:31 AM ET on 08/12, Discover Bank and multi-account Customers were unable to access their Cashback Debit accounts via the
mobile application, encountering a blank screen. Web browser users and single-account customers were unaffected.
Resolution: To resolve the issue all the applications part of CHG12712093 (Bank code install) were backed out.
RCA: It was due to RewardsAPI which was not compatible with mobile. Feature suppression data type changed from an array to an object in
RewardsAPI, since the old code expects an array and sees an object, the app failed to render the screen which likely caused the issue.
Alerts


Card RRT:
IA0030255 - Multiple Datadog Alerts - P4
Issue: From 10:48 PM ET to 11:19 PM ET and 11:30 PM ET to 11:47 PM ET 8/13 observed the errors calling to Inetecommprofileservice2, due to
which customers experienced issues while accessing personal profile on web and mobile .
Impact: Card mobile - 1.18k non unique and Card web - 409 non unique
Cause: Issue cause is believed due to be oracle controller contention due to CHG12717898.
Resolution : Issue subsided without any intervention when change completed CHG12717898.
IA0030261 - SSN New Account Inquiry Alerts page is hard down on mobile app and website -- P4
Issue: From 2:23AM ET 8/13 to 11:53AM ET 8/14, Experian's Identity Alerts service experienced an outage affecting users attempting to log in
or enroll. The incident stemmed from a recent domain transfer project where the domain was migrated to a new provider without transferring
essential connection records, taking the service offline.
Impact: Customers experienced issues while accessing SSN alerts page in web and mobile 9.13k non unique failures (last week 7.28k calls)
Customers experienced issues while enrolling into SSN alerts in web and mobile - 747 non unique failures (1ast week 718 calls)
Root Cause: Important internet routing records (DNS CNAME) were missing after a recent domain move from CSC to GoDaddy .
Resolution: The technical team resolved the issue by locating the missing CNAME record and collaborating with GoDaddy, the new domain host,
to restore it. Domain resolution is functioning properly, and user access to the dashboard has been fully restored.
IAO030262 - Internal Users and Systems are Unable to Send or Receive Emails Due to Microsoft Exchange Online Failures - 3C
Impact: From 8:15 AM ET to around 10:52 AM ET on 8/14, we observed issues with Outlook mail box, Users experienced full failure or
significant delays sending and receiving emails enterprise-wide. Internal automated alerts (such as Service Now email notifications) were not
being delivered, requiring manual queue monitoring.
Root Cause: A global DNS resolution failure on Proofpoint's end (GSLB infrastructure) prevented external/internal mail flow and disrupted
connected web services . It was initially suspected to be a native Microsoft/Exchange outage, but further investigation confirmed
Proofpoint's DNS issue as the true root cause.
Resolution: Proofpoint identified the infrastructure root cause and deployed a DNS fix around 18:52 Eastern, Once the fix was applied, IP
resolution began recovering globally . Mail flOw, portal access, and system login capabilities (including e0scar and AppRelay) returned to
normal as DNS changes propagated.

