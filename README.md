7th ,

health CheCK 100KS BOo0 ldter
IABe28232 TransUnion Degraded - P4
Impact: From 9: 00am until 11:52am ET on 3/7, credit report service & MLA servíce for TransUnion was degraded. This was impacting Discover Personal Loans causing delays with processing and
instant decisions. 35 customers were impacted on the DPL side.
Cause: Vendor Inflicted- - Vendor TransUnion experienced an internal issue. RCA will be provided at a later date.
Resolution: Vendor resolved their internal issue.
IAB02823e - FAA-Flex Authentication Degraded - P3
Impact : From 8:25am until 11: 54am ET, Flex Authentication was degnaded. Bank customers experienced failures during Zelle enrollment.
Cause: Due to 1 of 4 Pods in FAA-Challenge Prod2 going into high memory usage distress .
Resolution: To mitigate, Command Center moved FAA-Challenge - Orchestration traffic from East Prod2 to East Prod1. To resolve, FAA-Identity Authentication team performed a restart of Prod2. After
validation, Command Center move traffic back to Prod2 at 3:07pm ET
Card RRT:
IAB028224 Balance Transfer Minimally Degraded --p4
lepact: From 12:83am until 2:09am ET on 3/7, card customers experienced an issue with seeing promotional balance transfer offers. There were 11 non- unique customer requests that failed on the
Card Account Center website, and 47 on the Card Account Center Mobile ap. The impact count will be aggregated onto the problem record PRBO058689 for the same issue on 3/6.
Cause: The root cause of the issue remains unknown and will be investigated by Mainframe Engineering and vendors Kyndryl, and IBM offline.
Resolution: To resolve the issue, vendor Kyndryl manually moved the rate file to another Local Shared Resources pool.
LAB82823e: FAA-Flex Authentication Degraded - Resolved
Iepact: Fron B:25am until 11:54am ET, Flex Authentication was degraded. 6,178 unique Card and Bank customers experienced failures during the challenge process across multiple functional ities
including Account Center Recovery, zelle enrollment and payment, Card Activation and Registration .
Cause: Due to 1 of 4 Pods in FAA-Challenge Prod2 going into high memory usage distress .
Resolution : To nitigate, Command Center moved FAA-Challenge-orchestration traffic from East _Prod2 to East_Prod1 . To resolve, FAA-Identity Authentication team performed a restart of Prod2. After
validation, Command Center move traffic back to Prod2 at 3:07pm ET
IAB928226 for Card Statements Sporadically Unavailable Mitigated
Inpact: From 6:24am until 8:46am ET on 3/7, DÍscover Cardmenbers were sporadically unable to view their PDF statement s in both Web and Mobile within Card Account Center. Mobile: 9269 unique
Customers (48%) unable to view their PDF statements out of total 191e0 calls, Web: 3982 unique customers (42%) unable to view their PDF Sstatements out of total 9430 calls.
Hitigation: The issue remains mitigated since the CC moved vault traffic to the BDC at 8:46am.
Update: There was a corruption in the Vault database and a roll back was done however index is still giving errors. Teams are still investigating. The Vault support team confirmed that the
restoration from the BDC to sSB is complete. The Vault team is verifying the restore through testing and awaiting batch to run.
g Alerts
sSues


6th
Card RRT:
IAB028196 for Card - Balance Transfers Minimally Degraded - Resolved
Impact: From 12:03am unti1 5:02am ET on 3/6, card customers experienced an issue with seeing promotional balance transfer offers. There were 30 non-unique customer requests that failed on the
Card Account Center website, and 151 on the Card Account Center Mobile app.
RCA: The root cause of the issue is unknown and will be investigated by Mainframe Engineering and vendors Kyndryl, and IBM offline.
Resolution: To resolve the issue, vendor Kyndryl manually created a temporary new Local Shared Resources pool.
Bank RRT:



5th
5th
Card and Bank RRT:
Inpact: From 10:40pm until 10:58pm ET on 3/4, there were a total of 741 non- unique customers, including SSO customers, that faced an error attempting to log into Discover Card ar Discover Bank
IABe28180: Discover Card and Bank Account Center Login Sporadically Degraded
P4
Cause: The issue is suspected to be due to out of memory issue in ocp clusters, which caused the application to go into a crash loop, leading to login failures. The root cause is still under
Account Center. Login impact was sporadic to customers via Web or Mobile.
Resolution: To mitigate impact, DigitalEngineering_Citadel updated the configuration settings to heap size and resource memory
investigation by 0CP Ops.
IAB028185- Catchpoint API_ INTR_ BANKMOBILE_ LOGIN PWD failure
There were errors from 5:41 AM to 6:01 AM on 05/03/2026 for BANKMOBI LE_ LOGIN _PWD, we checked our datadog JvM's they were good, later we saw success blips .
NA
We dropped a mail to catch point team, so they confirmed the test was failing from 2 specific node. Recently there was a change in IPs for these 2 nodes which needs to be whitelisted. Far tine
being they have removed the 2 nodes from the testing group,
lerts



