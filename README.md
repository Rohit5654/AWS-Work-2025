9th Oct
Bank RRT:
========: ==========
IAOO30856 - Customers Are Unable to Provision Cards in Multiple eWallets - P4
Impact- From 11:44PM ET on e8/10 to 12:24AM ET on 09/10, Customers were intermittently unable to access several Bank
and Personal Loan Acquisitions pages.
RCA- Due to network change CHG12691596 which caused non-graceful interface failovers and intermittent "no route to
host" connectivity drops across WebSphere and 0CP clusters.
Resolutions - Issue got resolved post change completion.
We had a traffic drop for Content -edge-router -bank, AER bank and few other banks apps but we didn't get any traffic
drop alert.
IA9030866- Some Discover Bank Customers Were Unable to View their Rewards Balance- P4
Impact: From 5:52 Am ET to 8:11 AM ET and again from 8:42 AM ET to 8:52 AM ET on 10/09, we observed the errors while
calling specific host of cloak Api. This issue caused some Discover Bank customer's ability to view their Rewards
balance.
RCA :After the completion of a cloak sSB os Patching change (CHG12747017) , a single faulty server node (1 out of 186
total host nodes) encountered errors during Api calls on the rewards balance endpoint.
Resolution : To mitigate the issue, the problematic node was disabled 'and isolated from receiving traffic and taken out
of rotation.
IA9030875 - Primary Multiple DFS Applications Experienced Minimal Impact Due to an AWS Backbone Issue - P4
Impact: From 6:11 PM to 6:50 Pm ET on 10/09, we have seen time out errors in bank migration service from finacle which
result in multiple bank apps was impacted and multiple alerts generated for bank.
RCA: AWS confirmed a backbone network event in us-east-1 causing packet loss between AWS VPCs and on-premises data
centers.
9+
7:11 AM
ENG

AV resoIVe Lie DacKDOrie eveiL,
drid dll uepenueiL SysLems ndve reLurneu LO nOrldi operaLLIg UdseiLIIeS.
Card RRT:
===E====
IAOO30856 - Customers Are Unable to Provision Cards in Multiple eWallets - P4
Impact: From 10:15 PM ET to 11:18 PM ET on 10/08 again from 12: 25 AM ET to 1:10 AM ET on 10/Ø9, Some Discover
Cardmembers were seeing an error after logging in on the AC Home screen for Card mobile. 81 unique customers were
impacted.
Cause: The network change implementation CHG12691596 (ACI top-of-rack leaf switch replacements in SSB), which caused
non-graceful interface failovers and intermittent "no route to host" connectivity drops across WebSphere and 0CP
clusters.
Resolution: To mitigate, AER, Card and 0CP traffic was moved to 100% BDC which reduced the errors, then it was flipped
back to it's initial state A/A. Issue got resolved post the change completion.


IADO30875 - Primary Multiple DFS Applications Experienced Minimal Impact Due to an AWS Backbone Issue - p4
Impact- From 6:11 PM to 6:50 PM ET on 10/09, We observed connection and read timeout exceptions for universal-
customer-login-api, universal-mobile -api and card-ac-home.
card achome web - 7 unique customers, card achome mobile - 357 unique customers are impacted.
Cause- A technical correlation revealed a spike in connection failures between US East and West regions within the AWS
OCP environment during the impact window.
Resolution- Issue subsided without any support intervention. AWS CASE: 179158045000064 is created for further
investigation.


WE
W1tn1n the ANS
OCP environment during the impact window.
Resolution- Issue subsided without any support intervention. AWS CASE: 179158045000064 is created for further
investigation .


