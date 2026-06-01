Card RRT:
IA0029347-Discover Card Customers are unable to load statements -3C
Issue- We started seeing errors with statement rest from 7:22 AM ET until 8:48 AM ET With end point
get_/v1/statements/_statementdate
Card Impact Discover card customers/Statement Viewing 13,137 non unique Customers, 2,081 unique customers via Web. 11056, unique Mobile customers .
Bank Impact - From 9:46 PM ET on 05/25 to Ongoing, Bank Customers sporadically experiencing issues with Bank SMC, when customer tried to access the latest statement PDF
it was not loading.
Cause- Initially Vault process was down on BDC, To mitigate the impact vault traffic was flipped to 100% ssB but later on it was hard down on both the sides.
Resolution - Vault team has restarted the vault process on SSB after second trial where live traffic was pointing which helped on mitigat ing the impact for SsB.



Swastik Saha Friday 2:14 AM
Today changes:
Ss
CHG12671159 Emergency Change to Fix Vault ongoing Production Situation 61764 - Ongoing
https//capitalone zoom usli/61504033222 pwd=eEE3emt2WktCZUpReEhHekE3dIZOdz09
re
Breakroom 10 (informed them to us know once complete)
NNE



Update from AlONE
Wade Moore lega166)-2026-05-3108:43:06
Overall incident SummaryBeginning at 07:22 ET on 5/25, customers were unable to access biling statements across digital channels. At 08:48 ET, the Vault team restored statemertieing
cOmpleie process restart for austomers with a biling cyce príor to S/23. From 11:00 ET until 05:45 ET on 5/29, customers with accounts cycled 5/23 and later could not view their aurentmothesttnt
Vawebor mcbile Tomitigzte impact, austomers were able to view monthiy statement detalls via tihe web. Printed statements were also mailed to customers on the 5/23 and 5 24blinEodsAnmt
otion was fy degloyed to BDC and taling 100% traffc as of 05:45S ET on S/29. This enabled ful access to pdf statements online. The solution was implemented in SBB and mirraring turned en ut 2ET
an500. Traicwas then grdually moved to active/active, cormpleting at 20:50 ET. Alservices are now back to normal operations.Cause:ldentihed: Processing a 1TB- fle trissered an uinosielimit in
Predisely softare, causing an indeer D heap error, index corruption, and total failure of the Vault ingestion path.Total Critical lImpacts:7,480 - Discover Card Statements prior to S23
DMiatediGrbspr-77.000-Customers that accessed the Staternents sereen in Webor Mobile could not get to statement pdf, but could get key staterment information via Web (MMigted TBD-Cadlet
Ipact Mtigated)
ON-202605-
