Installs
1st
Bank RRT:
IABB28622 Multiple Bank Applícations Degraded - P4
Teact: From 9:4208 until 9:45pm ET on 3/31, Bank customers experienced latency and login failures via Bank nobile and big browser. Users would have been unable to make changes en their accat
details during the mentioned tímeframe. There were 1,025 non-unique failures observed during the time of impact.
Cause: During CHG125985e9 (E Patching), RWAPTSGVe7 had 100% cPU and stopped taking traffic.
Resolution: The issue resolved without support intervention .

3rd 
.Card RRTS:
IAB028652 : Discover Card Account Center Registration Degraded - P3
Inpact: From 10: 00pm on 3/31 until 5:02pm ET on 4/2, cardmembers attempting to register their card via web or mobile, and using a user name already in use, would yet a tech diff and not receive
an option to select a different user name. Approximately 3,300 cardmembers were impacted.
Cause: Due to CHG12619083, CHG12619086 (account-center- login -restr-prod) . Root cause under investigation by Login Integration Infrastructure Team.
Resolution: Login Integration Infrastructure team rolled back the changes.



4th
Card RRT:
IAB828658 -Card and Bank login degraded - P4
Impact : From 10: 54pm untíl 10:56pm ET on 4/3, Card and Bank web and mobile customers experienced tech-diff pages when attempting to login. There were 380 non-unique fallures observed uhen
customers attempted to login to the mobile app, and 606 non-unique failures observed when customers attempted to login to the website.
Cause: The issue was caused by change related activity performed during CHG12602990 (IHS SSB Cache Database Migration), in which session-auth- api updated remote session flag for DB calls. Thịs
caused the 2 minutes of impact
Resolution: The issue resolved without further support intervention
IABB28659- Observed errors in paymentsrest - P4
Impact: From 11:54 pm ET on 4/3 until 12:01 am ET on 4/4, we observed errors in payments applications, but there was no inpact to making a payment
Cause: The payments team is going to investigate offline for root cause. Digital SRE to look into Dashboard for Impact analysis.
Conclusion: IssUe resolved without any support intervention.
(Errors existed but the only thing that was prevented was the popup screen saying the payment is confirmed]


