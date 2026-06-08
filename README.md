Shital Telghane Tuesday 8:46 PM Edited
IA0029463 - Some Datadog Monitoring Alerts Are
ST
Experiencing Delayed xMatters Page Notifications --
3D
Impact: From 5/29 to 2:21 PM ET on 06/02, a
subset of monitoring incidents experienced delayed
XMatterS pages and acknowledgement notifications
following migration from Moogsoft to Datadog
ITSM integration. Approximately 214 notifications
(6-10% of monitoring incidents) were affected.
Cause: Investigation identified a configuration issue
in the newly deployed ServiceNow Datadog
integration business rule. The business rule was
configured to execute asynchronously, creating
transaction bottlenecks and queue delays during
high transaction volumes. As a result, automated
payload transmission from ServiceNow to XMatters
was delayed, causing late delivery of alert
notifications and acknowledgements.
Resolution: Under CHG12673671, teams
implemented a configuration fix to move
notification execution from asynchronous queue-
based processing to immediate execution within the
ServiceNow system flow. The fix was validated in a
lower environment and deployed successfully to
production at 2:21 PMET. Post deployment


ServiceNow system flow. The fix was validated in a
lower environment and deployed successfully to
production at 2:21 PM ET. Post deployment
monitoring confirmed that newly generated
incidents were paging and acknowledging
successfully without additional delays.
