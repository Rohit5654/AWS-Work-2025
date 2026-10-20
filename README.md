12th
Card :
IABƏ3e899 - Some Discover Customers Are Unable to Access their Account -- 3C --Ongoing
Impact: From 3:36 to 5:36 AM ET on 10/12. we observed sporadic increase in account lock failures for universal -
Customer-login-api. No impact in this first timeframe. From around 5:35 AM ET to to 8:50 AM ET, we observed customers
got blocked and can not access their accounts. 16378 volume drop compared to Sep 7th holiday, only web impacted.
Root cause: Account lock failures due to bot traffic, DFIR Te am implemented this change CHG12759761 to block fraud
traffic. The block was put on hash value but somehow it impacted actual customer, and actual customer got blocked.
Resolution: DFIR ro1led back the change.
Reconvene at 10:00 AM today at 10/13


14th
IAO030927 Some Discover Bank Customers Were Intermittently Unable to Access Statements - p4
Issue : From 7:38 Pm to 9:14 PM ET on 10/14, Bank Customers could experience technical difficulties while accessing
Statements via Bank web and mobile App.
RCA: Bank extraction batch jobs running for system migration caused high latency and thread contention on the Vault
Document Retrieval Service.
Resolution : Appteam manually stopped the extraction batch at 21:14 ET, which successfully mitigated the performance
degradation and restored normal response times.


15th
Bank RRT:
IABO30927- Some Discover Bank Customers Were Intermittently Unable to Access Statements- p4
Issue: From 7:38 Pm to 9:14 PM ET on 19/14, Bank Customers could experience technical difficulties while accessing
Statements via Bank web and mobile App. Total 82 unique customers impacted .
RCA: Identified: Bank extraction batch jobs running for system migration caused high latency and thread contention on
the Vault Document Retrieval Service.
Resolution: Appteam manually stopped the extraction batch at 21:14 ET, Wwhich successfully mitigated the performance
degradation and restored normal response times.


18th
Bank:
IAOO30945 - Observing sporadic failures for fréeze and unfreeze endpoint- P4
Impact: from 07:37 am ET on 10/18 to 08:19 AM ET on 10/18, Bank customers were unable to access their freeze and
unfreeze debit card functionality . 45 unique customer where impacted.
RCA: App team has raised ticket to FIS vendor for RCA. (Ticket no-CS07420325)
Resolution: Issue got resolved without any support intervention.
