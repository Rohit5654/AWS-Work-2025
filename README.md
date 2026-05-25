19th
Card and Bank RRT:
IAO029267 Multiple errors observed for IVR, card, bank - P4
Impact: From 7:38 PM ET to 7:50 PM ET on 5/18, for Card and Bank total 477 non-unique customers were impacted while logging into both Web and Mobile.
Cause: The AWS EC2 Support team confirmed that the underlying hardware failed and an automated mechanism recovered the instance with same configuration (same ENI, I
etc) on another host infrastructure
Resolution : Issue subsided without any support intervention.
Card RRT:


2tg

Card RRT:
JABe29291 - Some Discover Card Customers and Call Center Agents Unable to Download PDF Statements -- P3
Impact: From 4:e0 AM ET to 08:58 AM ET, we observed 404 errors for "/v1/statements/{statementDate}" endpoint.
Discover Card Online Statements 9,458 unique customers impacted
Cause: A background vault process failure on the BDC site caused statement downloading requests to error out, compounded by an incomp lete statement ingestion job for
specific cycle dates.
Resolution: To mitigate the isSue Vault team flipped the traffic to 100% SSB and started the processes on the impacted BDC nodes. A case (case # PRE-0904096) has been
opened with vendor software provider Precisely to assist with root cause investigation.
