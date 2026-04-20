13th
nstalls
Card and Bank RRT:
IAB028781 : Card and Bank Login Degraded -- P4, Resolved
Impact : From 10:19pm until 10:23pm ET and from 11: 33 PM ET to 11:36 PM ET on 4/12, Card and Bank web and mobile customers experienced tech-
diff pages when attempting to login. Bank customers experienced 280 non unique failures while accessing mobile and 142 non unique failures
while accessing web. 163 unique failures were observed for Card mobile and 33 unique failures observed for Card web.
Cause: The issue was caused by change related activity performed during CHG12599277 (Card, Bank: IHS SSB Cache). citadel team performed
remote cache disablement during that time the pods got restarted which caused latency.
Resolution: This issue subsided without support intervention. After the affected pods restarted, the latency dropped .

15

Bank RRT:
IA0028806 Discover Bank BillPay and Zelle Degraded - P4
Impact: From 7:16pm until 7:23pm ET on 4/14, Discover Bank Bill Pay experienced sporadic impact resulting in: 44 unique customers impacted
while enrolling via Bill Pay in mobile. 15 unique customers impacted while enrolling to Bill Pay in web. 2 unique customers impacted while
adding a payee in mobile . 1 Unique customer impacted while adding a payee in web. 3 unique customers impacted while scheduling a payment in
web. Additionally, there were approximately 33 unique Zelle failures, impacting Bank customers attempting to transfer funds via Zelle.
RCA: Due to a connection issue to vendor FIS. Root cause to be provided by vendor FIS.
Resolution: Issue got mitigated without support intervention.
Card RRT :


17
Bank RRT:
IAD028817 for Bank - Bank Debit Card Management Non-Transaction Degraded - Resolved- P4
Impact: From 5:57 pm until 6:4@pm ET on 4/15, Bank Debit Card Management (Non-Transaction) was degraded. 374 unique Bank customers
experienced errors when attempting to freeze and unfreeze their debit cards via web and mobile.
Cause: --Vendor Inflicted - - Vendor FIS had internal issues. Team Monarch wil1 work with FIS on root cause. An RCA will be provided at a
later time.
Resolution: Vendor FIS corrected their issue.
IABe28822- Bank Deposits - Servicing Statements and Tax Forms Degraded - P4
Impact -From 11: 35pm ET to 11:47pm ET on 4/15, Deposits customers were intermittently unable to view tax forms on Discover Bank Account
Center (web only). 98 unique errors were accrued.
Cause - The root cause is under investigation by app team and vendor Thomson Reuters.
Resolution - Impact subsided without support intervention.
IAB028822 - DATADOG CCBM INTR MOBI LE ACHOME


17th

Card RRT:
IAO028832 Card blip for 1 minute investigation - NA
Impact - From 11:34 AM ET to 11:35 AM ET on 4/16, We observed socket time out and read timeout exception for universal -mobile- api,
universal - customer -login- api, 23 non unique customers unable to login in both web and mobile.
Root cause: Due to one of the AKAN POD stopped taking traffic during the above timeframe, and resumed on its own.
Resolution - Issue subsided by its own. AKAN te am will work offline to find the root cause.
IAB028835: Seeing increase in traffic for promo - apr-offers -ui --Nonalert
Issue: From 9:00 AM ET On 04/16, We are observing increase in traffic for promo-apr-offers -ui.
The traffic is due to new email campaign that started on 04/16.
Card&Bank:
IA9028839: Mobile Biometric Authenticiation Logins Degraded - P3
Capital One Severity: 3
Inpact: From 7:44am until 7:53 am ET on 4/17, 8807 customers were unable to login with mobile biomet ric login. Customers were able to login
with other method available.
Cause: --Vendor Inflicted - - Fido- DAON, A workaround during a planned change at vendor caused the issue.
Resolution: Impact subsided without support intervention .
ng Alerts







18th
Card RRTs:
IAOO28844- DiscoverCard Account Center SplitPay Degraded --P4
Lnpact: From 12:38am on 4/14 until 5:37pm ET on'4/17, 330 Discover Card customers were being redirected from the SplitPay page to Fresh
Start page and were getting a tech diff error when trying to schedule payments via Web Only. The accounts selected for the Mave 2 migration
were the only accounts impacted.
Root Cause: Due to issues with the Collections portion of CHG12502304 (Card, Bank: Card Code Install) .
Resolution: Middleware Operations backed out the Collection portion of the change.
IAB028848- Card Cybertron is failing --Nonalert
Impact: From 6:09 PM ET to 7:50 PM ET on 04/17, Cybertron failed and we received 50 Internal Server error.
Root Cause: Due to database credentials rotating in the background. DFS- Secrets -Manager was converted into an init container. When database
credentials refresh, the new credentials are not being picked up and hence Cybertron is failing.
Resolution: Temporary fix performed by SRE Team: Restarted Rollout in each environment, Permanent fix will be done by SRE Team that is
convert DFS-Secrets -Manager into a Sidecar container.
Bank RRT's
IAB028842 - Bank Mobile Check Deposit Degraded- P4
Impact: From 11:2eam until 12:04pm ET on 4/17, Bank customers were sporadically receiving errors when attempting to deposit a check via the
mobile app.
Customers may have been successful upon retry.
Cause: Vendor Candescent had an internal error.
Resolution: Vendor resolved their internal error.
