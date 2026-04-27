20
IAB028865 - Managed Card Servicing Degraded in sSB- P4
Inpact: From 5:22am until 7:06am & 7:26am until 7:53am ET on 4/20, Discover Card customers experienced 2,320 non-unique failures (3% of attempts) navigating to the anuge
Cards screen via Mobile. Customers would be successful upon retries.-
Root Cause: Due to CHG12596909- Card, Bank: SSB WAS9- InetSvcstRWProd
WAS FP& 0S patching, 3 of the nodes having issues in cardcust omerinfo service, determned
based on their manual soap validation.
Resolution: Issue was resolved when CardCustomer InfoService SOAP traffic was moved to 100% BDC and restarted the particular nodes and flipped it back to VA


21

Card RRT:
IA9028878: Customer Login Alerts Processor Degraded - P3
Impact: Since 6:00am ET on March 8th, the application team observed increased failures from one of the two pods of customer-login-alerts-processor As aresultsoRE
customers were unable to receive secondary alerts email notification concerning account locks.
Resolution: The affected pod was terminated to mitigate the issue and restore stability.
Cause: RCA is under investigation.
IAB028875: Discover Card Disputes Degraded in SSB -P4- Resolved
Tmpact: From 5:10am ET on 4/16 until 2:09pm ET on 4/20, Discover cardmembers intermittently experienced a generic Null pointer error on 1, 824 Disputes Sumary (L.3
errors) and 1,054 Transaction Disputes (7.4% errors) non-unique page loads. 200 fewer disputes were initiated based on historical nunbers. There was no impact to BaLling
agents opening disputes for customers using Discover Cardmember Disputes System (DCDS).
Resolution: Internet Card Operations team restarted the unhealthy 3VM (Internet CNS2:rwlp1327. ihs. discoverfinancial. com^inetmc8- rwprod-n6)-
Cause: Root cause is under investigation.


23

Card-
IAB028899: Discover Card Mobile Customers Experienced Failures on Payments Pages - P4
Impact: From 8:25am until 8:27am & 9:39am until 9:55 am ET on 4/22. 338 unique Discover Card customers experienced intermittent failures on Payments related pages such as
Payments Reiew and Make a Payment via Mobile (6.25% failure rate). There was no impact to Web.
Cause: Due to Out of Memory (00M) issues on PaymentsREST WebSphere JVMs
Resolution: The JVMs were auto restarted by automation.
IABe28906: Observed errors in multiple ICO applications
NA
Impact: From 11:04 PM ET to 11:7 PM ET on 4/22, card and bank observed errors and time out while connecting to session-suth-api ,we observed 11S mobile failures and 82
web failures
and again from 12:41 AM ET to 12: 44 AM ET on 4/23, observed 68 mobile failures and 5e web failures.
From 4:54 to 4:57 AM ET and From 5:47 to 5:50 AM ET again we observes errors
Cause: The issue caused due to remote cache was disabled during CHG12630932 (Card, Bank: SSB IHS RW Cache : Oracle Database Server NNE Configuration)
Resolution: This issue subsided without support intervention.
IAO028908 - Observing errors for collections-eligibility-api wh ile calling inetepayservice
Impact: From 12:40 AM ET to 6:12 AM ET on 4/23, we observed sporadic errors for paymentsrest and inetepayservice2
endpoints: GET /V3/pendingpayments
GET /V2/paymenthistory
GET /{version}/paymentsummary
Cause: It is due to CHG12630932 - Card, Bank: SSB IHS RW Cache : Oracle Database Server NNE Configuration
Resolution: backing out change resolved the issue
IAB028913
Sporadic failures for API INT CARD MORTIE TIER1


Mail ohit Shinde.
ABockrvaks
Refactored GTM to use new cname chain due to IA0028920 and restore Active/Active Push new cornfigurat ion of Portal ,discover , tom V1/I
CHG12643523
Completed
Common RRT for Bank and Cardt
IA0028920 Discover Card and Bank Login Button Not Working 3C
Impact : Feom 10:54am ET to 107pm ET on 4/23, 91,364 cust omers (72,577 Card, 3,355 Bank, and 17,232 $50) were unable to vieu login prompts within the Discover Card k Bank
Account Center via web, Mobile services remained unaffected, Brand Promise impact reached 29%. from 11 s01am ET to 1:16pm ET on 4/23, 69 ot of 1,199 DiscHer Personal
Loans (DPL) applicants encountered errors during the verlfication proces5, CAUS ing fraud verification delays.
Cause: Following the implementation of vcr decomnission change CHG12621492 (vCr VIP Decomn iss ion cfi21), Global Trasffic Hanaganent (GH) properties for ecount Centar
Login referred to stale PCF instances and failed to resolve,
Resolution: Following the inplementation of a manual bypass of the failing GIH component to restore service and stabilize Brand Promise, the Secure Intarnet Applicat ion
Services team resolved the issue via CHG12643523 (Refactored GTM to use ney CHAME chain).
IA0028937 Multiple Applications Degraded - PA
Impact: Card-From 1:25am until 2:14am ET on 4/24, we observed errors in personalization-api-services where customers wil11 be shown with default offers instead of
personalized offers.
From 1:25AM ET to 2:14AM ET, we observed errors while calling api.capitalone.com where there wi1l be NO real Customer impact,
From 1:25AM ET to 2:14AM ET, We observed errors in universal-user-verifícation-api
From 1: 25AM ET to 2:14AM ET, We observed errors in internetcms3 where we observed 10,7K non unique failures whi le sending SMS notifications.
Bank- From 1:25am until 2:14am ET on 4/24, There were 4 Deposits customers were unable to order Checks through Deluxe and were unable to vies Check Grder history via the
Discover Bank Account Center Web. 32 unique errors in Bank Mobile Check Deposit preventing Deposits customers from depositing Checks to their bank account via the
Discover Bank mobile app.
Cause: Outbound proxy traffic to multiple vendors was disrupted due to CHG12643899 (Proxy VPs Modification) . A misconfiguration added a deny rule to the 558 prony
architecture.
Resolution: Proxyops backed out CHG12643899 to restore service,
Bank RRT:
IAB028933 API INTR BANKMOBI LE LOGIN PWD failing in Catchpoint - Non Alert
Issue: From 9:21 AM ET on 4/21, we started seeing API INTR_BANKMOBILE_LOGIN_PWD CP is sporadically failing.
Sent mail to CP team to fix this issue.
Mail Sub: Mobile Login PWD CP failures
Card RRT:
IAO028926 Card Mobile Payment Degraded- 3C
Impact: From 10:41pm ET on 4/22 until 2:08pm ET on 4/23, a sporadic number of Cardmembers received an error when attempting to make payment via the mobile app. During
Cardmembers would be able to make the payment via web.
this time, there were 11, B00 customers impacted.
4:53 AM
ENG
4/27/2026
US
T9+




25th
Card and Bank RRTs:
IADE28949 Multiple FICO Applications Degraded - Resolved - P3
Inpact: From 7:3Bam until 8:09 am ET on 4/24, multiple FICO applications were in a degraded state. The following impact is as follows . 802 out of 946 non-unique failures
ere observed for card customers who were unable to add external bank accounts via web and mobile. 9 out of 42 non-unique failures in Discover Personal Loans prevented
Customers from adding a bank account. 229 failed LIR (Line Increase Requests) requests. 338 bank customers were unable to perform fund transfers and 3 customers were
unable to add external bank accounts. 124 customers were unable to perform outbound transfers from Discover card to external bank. 214 customers were able to create
transfers but experienced a delay in fund availability. 37 out of 58 failed requests for customers unable to deposit their checks and experienced a tech diff page. 21
failed errors Mith Google VCN transaction for Discover Credit Card holders. 4 customers and 7 sporadic failures when attempting to add Discover Debt Cards to any digital
wallet. 12 customers were unable to access Zelle functionalities and unable to send payments. 22 customers were unable to check out Google VCN via Discover Network
Paymerts for both mobile and web.
Root Cause: Vendor Inflicted- -Vendor FICO experienced degradation in an IM registration port. The vendor is still investigating what caused the issue.
Resolution: Vendor FICO performed a port restart
Bank RRT:

