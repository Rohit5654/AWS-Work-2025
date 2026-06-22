Lmpa
Card RRT:
IAØ029636 - Discover Customers Experiencing Failures With Several High Risk Activities P4
Impact: From 4:10 am ET to 8:01 am ET on 6/16, Discover cardmembers experienced sporadic authentication errors and
were unable to complete account recovery. A total of 206 non-unique customers were impacted.
Root cause: One specific pod (XTJ4) out of four on the Prod 1 cluster failed to execute its aut omated background
refresh of an internal JsON Web Token (JWT). Operating with an expired token, the pod could no longer authenticate to
downstream services, causing it to go into distress with high memory usage.
Resolution: Services were restored to an active/active state at 08:01 ET. after traffic was temporarily shifted to Prod
2 and the distressed pod was restarted.
Bank RRT:


nge Installs
Bank RRT:
IAB029654 - Observing errors in posted -activities -api - P4
Impact - From 12:36 AM ET to 12:52AM ET, Bank Account home was not loading for bank customers.
Root Cause - For CHG12677365, bank transaction api traffic was flipped to east-1-prod-2, which caused the issue.
Resolution - After flipping bank transaction traffic back to east-1-prod-1 the errors were dropped.
As part of this RRT we had another issue From 12:26:3OAM ET to 12:27:30AM ET and, again from 01:20:30 - 01:20:50 AM ET,
we were seeing errors in bank-migration - service from API Gateway, we had created an INC to gateway team to check on
the RCA.
3:42 AM
ENG
a )
6/22/2026
US
T9+
pe here to search
