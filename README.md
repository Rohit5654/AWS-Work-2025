4th
App team has created a case with vendor for the RCA.
Card RRT:
Impact : From 10:06pm until 10:56pm ET on 3/3, Discover cardmembers directed to the BDC were sporadically unable to redeem their rewards for cash, or submit orders for other types of redemption,
IAB028159: Rewards Cash Redemption in the BDC Degraded
P4
or a statement credit via Mobile app. There were 456 non-unique errors impacting Card redemption. There were 62.3 k non-unique errors for viewing Rewards details during this time, however,
this number conflicts with the typical number of requests per night, which is approximately 9,000 transactions. Majority of the impact was to cardmembers being unable to view their Reward
details. This impacted Mobile app users only.
Rewards -Cash Redemption will investigate why there was such a great increase in errors for GET
Cause : Due to an increase in errors to rewardsrest API in the BD
Root cause under investigation by Rewards -Cash Redemption.
Icardsvcs/acs/rewards/v1/tracker/earn -details.
Resolution: To resolve the issue, Internet Card Ops restarted the RewardsREST JVM on nalp1327 node.
lerts





5th
ange Installs
Card and Bank RRT:
IAB828180: Discover Card and Bank Account Center Login Sporadically Degraded
P4
Inpact: From 16:48pm until 10:58pm ET on 3/4, there were a total of 741 non-unique customers, including sso customers, that faced an error attempting to log into Discover Card or Discover Bank
Account Center. Login impact was sporadic to customers via Web or Mobile.
Cause: The issue is suspected to be due to out of memory issue in ocp clusters, which caused the application to go into a crash loop, leading to login failures . The root cause is still under
investigation by 0CP Ops.
Resolution: To mitigate impact, DigitalEngineering_Citadel updated the configuration settings to heap size and resource memory.


6th
Card RRT:
IAO028196 for Card - Balance Transfers Minimally Degraded
Resolved
Impact: From 12:03am until 5:02 am ET on 3/6, card customers experienced an issue with seeing promotional balance transfer offers. There were 30 non- unique customer requests that failed on the
Card Account Center website, and 151 on the Card Account Center Mobile app.
RCA: The root cause of the issue is unknown and will be investigated by Mainframe Engineering and vendors Kyndryl, and IBM offline.
Resolution: To resolve the issue, vendor Kyndryl manually created a temporary new Local Shared Resources pool.
Bank RRT:
IA0028193 Catchpoint_ TRANS_ INTR BANK TIER2 Failing
We were seeing failure for TRANS INTR BANK TIER2 CP at Auto Redemption step, App team confirmed there is an update to the application where there is a change in functionality due to business
requirement which caused failures. We have dropped a mail to CP team to disable Auto Redemption Step for now.


7th
Bank RRT:
IADe28215 sporadic errors in dpl-payment - val idator - NA
From 9:44 PM to 10: 24PM ET on 03/06 we observed sporadic error for dpl-payment -validator. we paged app team but they didn't ioin. The issue got subsided by its own, inetdpl L2 confirmed as DPL
health check looks good later we closed the call
IABe28232 TransUnion Degraded - P4
Impact: From 9:00am until 11:52 am ET on 3/7, credit report service & MLA service for TransUnion was degraded. This was impacting Discover Personal Loans causing delays with processing and
instant decisions. 35 customers were impacted on the DPL Side .
Cause: Vendor Inflicted- - Vendor TransUnion experienced an internal issue. RCA will be provided at a later date.
Resolution: Vendor resolved their internal issue.
IABe2823e - FAA-Flex Authentication Degraded - P3
Impact: From 8:25am until 11:54am ET, Flex Authentication was degraded. Bank customers experienced failures during Zelle enrollment .
Cause: Due to 1 of 4 Pods in FAA-Challenge Prod2 going into high memory usage distress .
Resolution: To mitigate, Command Center moved FAA-Challenge -Orchestration traffic from East Prod2 to East Prod1. To resolve, FAA-Identity Authentication team performed a restart of Prod2. After
validation, Command Center move traffic back to Prod2 at 3:07pm ET
Card RRT:
IAB028224 Balance Transfer Minimally Degraded --p4
Impact: From 12 :03am until 2:09am ET on 3/7, card customers experienced an issue with seeing promotional balance transfer offers. There were 11 non-unique customer requests that failed on the
Card Account Center website, and 47 on the Card Account Center Mobile app. The impact count will be aggregated onto the problem record PRBO058689 for the same issue on 3/6.
Cause: The root cause of the issue remains unknown and will be investigated by Mainframe Engineering and vendors Kyndryl, and IBM offline.
Resolutíon: To resolve the issue, vendor Kyndryl manually moved the rate file to another LOcal Shared Resources pool.
IAB0282 30: FAA-Flex Authentication Degraded- Resolved
Tnpact: From B:25am until 11:54am ET, Flex Authentication was degraded. 6,178 unique Card and Bank customers experienced failures during the challenge process across multiple functional ities
including Account Center Recovery, Zelle enrollment and payment, Card Activation and Registration.
Cause: Due to 1 of 4 Pods in FAA-Challenge Prod2 going into high memory usage distress.
Resolution: To nitipate, Comand Center moved FA- Challenge - orchestration traffic from East_Prod2 to East _Prodl. To resolve, FAM- Identity Authentication team perforaed a restart of Prod2. After
valídatíon, Command Center move traffic back to Prod2 at 3:07 pm ET
IA0028226 for Card Statements Sporadically Unavailable - Mitigated
Tepact: From 6:24am until B:46am ET on 3/1, Discover Cardmembers were sporadically unable to view their PDF statements in both Neb and Mob ile within Card Account Center. Hobile: 9263 unique
Custoners (48K) unable to view their PDF Statements out of total 19100 calls, Web: 3982 unique customers (42X) unable to view their POF statements out of total 9430 calls.
Mitigation: The issue remains mitigated since the CC moved vault traffic to the BDC at 8:46am.
Update: There Mas a corrupt ion in the Vault database and a roll back was done however index is still giving errors. Teams are still investigating- The Vault support team confirned that the
restoratíon from the BDC to S5B is complete. The Vault team is verifying the restore through testing and awaiting batch to run.

8th
LnCTedse
From 3:30 AM to 5:15 AM on 88/837292b We oDSe
Card RRT:
Resolved
ABe28230: FAA-Flex Authentication Degraded
Inpact: Observed a new spike in errors for faa-challenge- orchestration from 17 :23 - 17:39 ET. Issue appears different than the main 3c issue.
Conclusion: Issue resolved without any manual intervention. Identity Authentication team is investigating the root cause offline.
| Alerts




