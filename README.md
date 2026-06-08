IASƏ29463 - Some Datadog Monitoring Alerts Are Experiencing Delayed xMatters Page Notifications -- 3D
Impact: From 5/29 to 2:21 PM ET, a subset of monitoring incidents experienced delayed xMatters pages and acknowledgement notifications
following migration from Moogsoft to Dataddg ITSM integration .
Cause: Investigation identified a configuration issue in the newly deployed ServiceNow Datadog integration business rule. The business rule
was configured to execute asynchronously, creating transaction bottlenecks and queue delays during high transaction volumes. As a result,
automated payload transmission from ServiceNow to xMatters was delayed, causing late delivery of alert notification s and acknowledgements.
Resolution : Under CHG12673671, teams implemented a configuration fix to move notification execution from asynchronous queue-based processing
to inmediate execution within the ServiceNow system flow. The fix was validated in a lower environment and deployed successfully to
production at 2:21 PM ET. Post deployment monitoring confirmed that newly generated incidents were paging and acknowledging successfully
without additional delays .



Card RRT:
Impact : From 7:17 PM ET to 9:22 PM ET on 6/4, Catchpoint TRANS INT SSO LOGIN continuously failing at Step 3: Card: Discover Card. No
IABe29505: Catchpoint_TRANS_ INT_SSo_LOGIN failing - P4 NA
Conclusion: The catchpoint monitors are failing due to a test account issue, The Catchpoint (Vendor) team updated the script for the test
Customer impact.
account. Post changes by Vendor we are seeing continuous success runs.
pi --Nonalert
