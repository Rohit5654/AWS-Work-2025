2nd Oct
Bank RRT:
IAOO3e786 - Discover bank Check order is impacted - P4
Inpact- From e3:24pm ET to e4:24 pm ET, Customers were experiencing failures when trying to place check orders via web.
RCA - Errors were due to an ongoing change at Deluxe vendor.
Resolution - Errors got subsided post change completion.

3rd

CHG12747715- Calico upgrade to v3.23.2 on aws-uswest2- apps-prod-1 Completed
CHG12747643- Calico upgrade to V3.23.2 on aws-useast1 -ppp-apps-prod-1 - Completed
Bank RRT:
IADe3e8e1 For Bank Discover Bank customers are unable to perform Bill Pay functions via Web and Mobile - P4
Inpact: From 8 PM ET to 9:56 PM ET on 19/02, Discover Bank customers have seen issues while accessing Billpay enrollment and payment
features via both web and mobile. Total 365 unique failures observed.
RCA: TLS Connection establishment failures and 403 Forbidden responses observed when communicating with downstream vendor FIS endpoints .
Resolution: Bank Falcons team executed rolling pod restarts for all four Bill Pay microservice APIS across all production clusters to flush
cached secrets and force Vault to load the new certificate.


4th
Card RRT:
IA0030818 - Some Card eSolutions Agents And ProtectBuy Customers Experienced Intermittent Latency And Authentication Failures Utilizing 00B
Channel -- P4
Issue: From 02:20 ET on 10/4, eSolations agents were unable to load customer accounts quickly because requests that required a database call
timed out after 30 seconds, causing slow page loads and occasional time-outs.
Cause: Overnight database migration moved the primary p_acctcenter database from EP66 to EP67, and the 00B Channel API's egress rules still
pointed to the old cluster, preventing database connections.
Resolution: 00B-Channel-API was redeployed, which restored normal service functionality.

