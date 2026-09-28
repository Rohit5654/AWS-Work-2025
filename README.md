22
Card and Bank RRT:
IA0030658- Multiple Applications Experiencing Widespread Issues Since 1:40pm ET- P3- Mitigated ( reconvene at 10 AM ET)
Impact- from 1:40 to 1:51 PM ET on 9/21, some Discover Card and bank customers experienced issues accessing the Account Center and some
online account functions. From 1:42 PM to 1:46 PM ET on a9/21, Bank went into lite mode and it isrestored back.
Cause An Exadata hardware frame in the BDC data center lost netWork connectivity, dropping database connections across hosted instances .
Card- ADWS was placed into lite mode on BDC.
and ocp bundle traffic was moved to SSB 100%
Mitigation: To mitigate, Card AER


26
Al BOOkmar
Card RRT:
SIT104202 Ease Mobile and Web Account Summary Degradation- 3C
Impact: Starting at 09:21 ET to 10:28 AM ET and again from 11:44 AM to 11:49 AM ET Oon 09/25, auto loan customers calls experiencing elevated
504 Gateway Timeout errors for view accounts, balances, or entitlements calls in EASE Mobile/Web , Impacted customers are unable to view
their account summary tile in EASE Web and Mobile. This is also impacting other LOBs for customers who have additional accounts
ICO Impact: We observed socket timeout exceptions in identity-migration-outbound- api for post /enterprise/migration-
outbound/v1/migration/eligibility
Impact count: Card - 15, 571, Bank - 8, 507, DFS External customers - 102
Cause: Due to deployment (CHG7035973) on the COAF Account API, which caused severe latency and service errors.
Mitigation: To mitigate the impact, they rolled back the change CHG7035973
Resolution: Technical teams stabilized the environment by bypassing the Auto Loan Account API at 10:31 ET, deployed a targeted fix and
expanded capacity at 11:41 ET. At 13:19 ET service was fully restored after progressively shifting 100% of traffic back to the EAST
IAO030704 - Some users experienced errors with multiple functions of the Discover Card Account Center - Resolved -Sev5
Impact: From 04:41 AM to e5:15 AM ET on 09/26, We observed errors in few of our applications (Rewardsrest, CMSREST1, CMSREST2) coming from
inetaccountmanagerservice2,
[Customers might not be able to view rewards cashback balance in mobile achome 737 non unique, web only had 1 error]
[Customers might not be able to manage cards in web - 23 non unique. mobile - 156]
Root Cause: The ADWS lite mode, which was kept in BDC for IAB030658, wasn't removed before moving card traffic to A/A as part of change
CHG12736212
Resolution: Card traffic was temporarily moved to 100% SSB to mitigate the issue and the ADWS lite mode was removed from BDC and traffic was
moved to A/A again for validation.


