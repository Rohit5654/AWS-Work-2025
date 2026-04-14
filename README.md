7th
Bank RRTS:
IABO28683 Bank Mobile Check Deposit Degraded - P4
customers were intermittently encountering error messages when attempting tO
Impact: From 11:33pm ET on 4/6 to 12:41am ET on 4/7, deposis
deposit a check via the mobile application. 75 unique errors were observed.
Cause: Vendor Candescent implemented an SSL certificate update.
Resolution: Candescent configured their SSL trust store so that the old certificate can run in parallel with the new certificate, resolving
the issue. The Digital Connect team will update the corresponding certificate on the Discover side in days to come.
IAB828689 for DPL is observing Sporadic Techdiffs from dpl-prequal-so - Non Alert



12th
Card and Bank RRT:
IAOB28777 : Card, Bank - Discover External Bank Account Verification Degraded -- P4, Resolved
Impact: From 10:38am until 11:02am then again from 3:06pm to 3:10pm ET and 3:46pm until 4:20pm ET on 4/12, Discover Card customers were
unable to add an external bank account via Web and Mobile with 1702 non-unique failures. Discover Personal Loan customers were unable to
make a payment with 346 non-unique failures . 8 unique Discover Bank Deposits customers experienced failures attempting to manually link an
external bank account.
Cause: Vendor Inflicted-- Due to an issue on vendor Early Warning Services' (EWS) end. The vendor will provide RCA.
Resolution: The vendor resolved their internal issue.

10th


IABB28732 - Discover Bank Bill Pay Functionality Degraded - Resolved - P4
From 2:05am until 4:84am ET on 4/10, Discover Bank Bil1Pay Get Payment List functionality was very sporadically degraded while connecting ta
Vendor FIS. There were 122 unique Discover Bank customers attempting to view their Bank Bill Payment history that spor adically experienced a
Tech Diff' page. This impacted Bank customers via web and mobile .
Customers may have been successful upon retry.
Cause: Root cause is under investigation by FIS and Bank Falcons.
Resolution: Issue resolved without any support intervention
Card:



9t
h
Bank RRT:
Impact: From 4:56pm until 7:47pm ET on 4/8, customers were receiving errors when attempting to deposit a check via the mobile app. There
IAOO28709: Bank Mobile Check Deposit Degraded - P4
were 204 unique customer failures out of 1097 attempts. Customers may have been successful upon retry.
Cause: -- Vendor Inflicted -- Due to internal pod issues with vendor Candescent.
Resolution: endor Candes cent restarted their pods.
