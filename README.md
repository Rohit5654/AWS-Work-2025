25th

Card and Bank RRT:
==========
======
IABO29723 - Multiple alerts for Card and Bank - Mitigated
Impact From 4:e7PM ET to 4:10 PM ET on 6/25, Card and Bank Customers have Experienced Difficulty Performing Actions.
Card: Card had increased error rates and high latency across multiple applications . UserRegistryServiceV2.0.0 observed
lite mode at 4:09 PM ET and got auto-restored.
Bank: Bank had increased error rates and high latency across multiple applications. Bank went under lite mode from
4:08 PM ET to 4:10 PM ET.
Suspected Cause: A volumetric retry flood caused a 4-to-5-minute technical disruption across card and banking
portfolios. A sudden surge in mobile requests bypassed authentication, overloading the production mainframe and
causing severe latency.
Current Status: A sudden surge in account statement requests overloaded the Customer Info Service, which then flooded
the backend mainframe and DB2 database with too many calls. Management suspects that when the system started slowing
down, apps automatically kept retrying their requests, causing the problem to snowball .
Reconvene at 10:00 AM ET on 6/25.



24th
BANK RRT
IIAO029736 - Bank Money Movement Wire Transfers Completely Failing from Mobile App - P4
Impact - From 11:30 PM ET on 24/06 to 4:09 PM ET on 25/06, Wire transfers initiated via the mobile application were
Completely failing for Bank Account Center customers. 195 unique customers were impacted during the timeframe.
Root Cause - The incident was caused by a software deployment introduced on the night of June 24
Resolution - The Bank Falcons engineering team successfully mitigated the incident by performing a system rollback to
the previous default.
Ts
itoring Alerts
