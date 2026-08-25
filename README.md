20th
Card RRT:
IAO03306 - Multiple Discover Applications Are Degraded due to MQ Issues -- P4
Impact: From e5:05 PM - e5:35 PM ET at 8/19, Multiple consumers impacted from AChome, sending messages via Morse
system, which failed to connect to MQ host due to some connectivity issue with SAN.
Impact Counts: Morse (Card) - 166, 583 non -unique notifications (Push/Email/SMS) delayed or successful upon retry.
Cause : An ARP storm at approximately 16:57 ET caused a temporary network connectivity disruption to the BDC Zone 3
NetApp storage cluster, leading to share volume timeouts and unresponsiveness across hosted Unix MQ servers.
Resolution: Impacted traffic successfully failed over to sSB at 17:32 PM ET; to restore the functionality. All
impacted services are returned to BAU and validated as 00:04 AM ET on 8/20


21st
Card RRT:
IA0030329 - Observing sporadic errors for fido-authentication-api - P4
Impact: From 10:08 AM ET to 10:43 AM ET on 8/21, we observed sporadic errors in fido- authentication- api for
/enterprise/fidoauth/v3/authentication endpoint. Customers experienced intermittent biometric login failures on
discover mobile app, with approx. 200 failed requests. Standard username and password logins were unaffected.
Root Cause : Issue is with vendor Daon. App te am has created a Case #541149. with Vendor for RCA.
Resolution: Issue subsided without any support intervention.
ts

