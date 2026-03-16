9th
Resolved
Cause: An identified agent was performing excessive transaction ingestion which exceeded
AWS burstable IOPS limits, causing intermittent latency and timeouts.
Resolution: Impact was mitigate by moving multiple impacted OCP applications and APls
100% to USEast Prod 1. The agent identified was disabled on USEast Prod 1 and 2 at 2:00pm
ET, West Prod 1 at 4:45pm ET, and West Prod 2 at 5:30pm ET. There is no risk due to the
disabling of the agent as there is a similar functioning agent that performs the same functions
running on the environment.
2 2)


10th
Card RRT'S:
IAO028226: Card Statements Sporadically Unavailable - P4
Impact: From 6:24am until 8:46am ET on 3/7, Discover Cardmembers were sporadically unable to view their PDF statements in both Web and Mobile within Card Account Center. Mobile: 9269 unique
customers (48%) unable to view their PDF statements out of total 191ee calls. Web: 3982 unigue customers (42%) unable to view their PDE statements out of total 9430 calls. Additionally, Customer
Service and Engagement agents encountered similar errors when attempting to load customer statements in Orion, resulting in 32 non- unique failures (39%).
Cause: Due to index being corrupted . The Vault team is working with vendor Precisely on full RCA.
Resolution: After restorat ion was confirmed complete at 9:00pm ET on 3/8. The Command Center moved Internal traffic to A/A at 11:20am ET and moved external traffic to A/A at 12:45pm ET.
Validations for both internal and external traffic were completed at 1:00pm ET
IAB028274: Multiple Applications Degraded - P3
Impact: From 7:14am until 10:54am ET on 3/9, Discover Card and Bank customers experienced intermittent failures during login and loading ACHome. Card & Bank Mobile Passwordless Login: 4334
failures (non-unique). Card Mobile ACHome: 135 unique customers experienced failures. Card Web ACHome: 187 unique customers experienced failures. Bank Mobile ACHome: 804 failures (non-unique).-
Discover Card and Bank customers experienced intermittent failures performing flex authentication for high-risk transactions. Additional customer impacts are being assessed and confirmed. Zelle
enrollment and payment, and card activation and registration. 580 unique Card and Bank customers were unable to load homepage. 55 unique Discover Bank customers experienced failures performing
funds transfer.
Cause: An identified agent was performing excessive transaction ingestion which exceeded AWS burstable IOPS limits, causing intermittent latency and timeouts.
Resolution: Impact was mitigated by moving multiple impacted OCP applications and APIS 100% to USEast Prod 1. The agent identified was disabled on USEast Prod 1 and 2 at 2:00pm ET, West Prod 1
at 4:45 pm ET, and West Prod 2 at 5:30pm ET. There is no risk due to the disabling of the agent as there is a similar functioning agent that performs the same functions running on the
environment.
IAB028230: FAA-Flex Authentication Degraded - P3
Impact: From 6:36pm until 7:19 pm ET, faa-challenge -orchestration degraded
1636 unique customers impacted from 6:36PM ET to 7:19PM ET 3/9 during the challenge process across multiple functionalities that include Login, Account Recovery, Zelle enroll and payment , Card
Activation and Registration, External Funds Transfer. During this same window, 4110 unique customers successfully completed the challenge process.
Cause: Due to 1 Pod in FAA-Challenge Prod1 going into distress with 0% memory but 99% errors.
Resolution: To mitigate, .FAA-Identity Authentication te am performed a restart of the impacted Prod1 pod post which the errors stopped.
IABR28290:
MPUM


11th
alls
Card and Bank RRT:
IABB28301 - Card and DPL - External Bank Account Verification Degraded - P4
Impact: From 9:59am until 11:56am ET on 3/10, external bank account verification calling vendor Early Warning Services (EWS) was intermittently failing-
Discover Card customers experienced 712 non-unique failures (26.3%) adding an external bank account in payments flow.
Discover Personal Loans customers experienced 158 non-unique failures adding an external bank account in DPL payments flow. 152 non-unique attempt s to make a DPL payment failed.
Deposits customers were not impacted.
Cause: --Vendor Inflicted-Vendor Early Warning Services (EWS) experienced an internal issue with their Account Owner Authentication (AOA) application, causing Discover API perfarm bank account
Owner verification to intermittent ly fail. The vendor will provide RCA within 2 business days.
Resolution: The vendor resolved their internal issue.
Alerts
