Card RRT:
IABO30429 - Mult iple Batches Delayed -- P3, Resolved
Issue: During a scheduled change at 22:09 ET on 08/31, the ODSTRIG account password was mistakenly reset instead of
the TELEODS account. This blocked Mainframe file transfers to Enterprise Rewards and EDS. The Active Directory team
fixed the password at 07:20 ET on 9/01, resuming file transfers. All delayed background processes (Rewards,
Statements, CFR, Vault Ingestion, and FDR) caught up by 13:46 ET 9/1, fully restoring account updates for Web and
Cause: During Scheduled change CHG12729744, the ODSTRIG generic account password was rotated by mistake instead of the
Mobile users
intended TELEODS account.
Resolution: The Active Directory team fixed the password at 07:20 ET on 09/01, resuming file transfers.


Card & Bank RRT:
IAO030473 - Some Users Are Experiencing Errors Across Multiple Discover Applications Due to a Network Loop- P4
Impact : from 03:56pm ET to 4:25pm ET on 9/03 observed errors in multiple card and bank applications. 384 non-unique
customers unable to login to AC via web and mobile
Suspected root cause: A new, non-production Windows host was configured with a software Network Bridge across its two
network interfaces instead of standard NIC Teaming.
Resolution: Issue got subsided without any support intervention.
Bank RRT:


Bank RRT:
IADO3O488 Some Discover Personal Loan Applicants Are Experiencing Errors Accepting Terms and Conditions or
Completing One-Time Passcode - P4
Impact: From 06:00 Am ET on 09/03 to 07:15 PM ET on 09/04, Discover Personal Loan (DPL) applicants are experiencing
technical difficulties online, specifically encountering blank screens when attempting to complete One-Time Passcode
(0TP) verification or accept Terms & Conditions.
RCA: Technical leads identified a potential correlation with recent deployment changes-specifically an August ad - hoc
release executed on Wednesday night involving Verification UI and Fraud Services.
Resolution -The team evaluated a rolling back the recent UI and service changes and DLOS team refreshed the DPL akamai
pages.




