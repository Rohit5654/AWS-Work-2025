# AWS-Projects

Bank RRT:
IA0027919 - Bank Mobile Check Deposit Degraded
P3
Impact: From 5:00am until 2:25pm ET on 2/19, Bank Mobile Check Deposit was in a degraded state. Bank customers experienced failures attempting to
deposit checks to their Discover Bank account via the Discover Bank Mobile App. There were an estimated 291 unique customer errors encountered
during this time. Customers may have been successful on subsequent attempts.
Cause: Due to a Postgres database being out of sync and replication failure. Root cause remains under investigation by Digital Connect.
Resolution : To mitigate impact, at 2:25pm ET, Command Center flipped traffic to US EAST Prod 1. To resolve, Postgresql-Support team used the "Solve
Now" button and after running troubleshooter, Digital Connect team was successful with recreating the subscription.
IAØ027925 Discoverbank. com Degraded - P3
Impact: From 9: 40pm until 10:05pm ET on 2/19, Discoverbank. com was in a degraded state. Bank customers experienced slowness logging in and
navigating Discover Bank online, via web. There were also 994/28, 822 (3.4%) non-unique login tech diff failures.
Cause: There was a Bank JVM that went into distress after Discover Bank traffic failed over 100% to the SSB for a scheduled change. Root cause
under investígation by Internet Banking and Deposits - Boot Bots.
Resolutíon: Impact subsided after the distressed JVM auto restarted.
Alerts
