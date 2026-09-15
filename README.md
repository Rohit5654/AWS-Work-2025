12
CHG12736109 OCP cgroup upgrade to v2 on aws - useast1-ppp-apps-prod-1
talls
IA9030551 - Customers Are Experiencing Errors When Attempting to Retrieve Usern ame or Password on Discover Web and
Mobile - P4
Impact : From 8:08 PM to 11:40 PM ET on e9/11, we observed JweDecryptionException in universal-user -verification - api.
where some discover customers are experiencing errors when attempting to retrieve their User Name/ Password
information. There were 1963 unique customers impacted.
Endpoint : /enterprise/user-verification/v2/user/verification
Root Cause: A expired JWKS decryption certificate on the external API gateway causing account recovery requests to
fail for web and mobile users
Resolution: Team deleted the certificate from the backend, and API management team cleared the cache, which stopped
returning the expired certificate.
erts
IAOO3e523 - Oracle DB (SSB) m231r Active Sessions Increased - 3C (Reopened)
Update - At 10:03AM ET On 9/10, it crossed 40+ active sessions on SSB - as a precaution card traffic was moved to BDC. They discussed the
root behavior was table lock on oracle DB. The team suspects that two different queries are attempting to access or delete the same entry
simultaneously. This competition for the same lock causes transactions to hang-one query acts as a "root blocker" while others wait, leading
to a cascade of blocked transactions. But no proper update on RCA. Oracle DB team is working on it. Will stay in BDC until further updates
from Oracle team. Reconvene on 10 PM ET tonight.

Impact count - 78194 volume drop in login web and mobile
Root cause: Investigation identified database locking involving uncomitted sessions on ssB cache tables including
payment_bank_account_cache and payment_info_cache) Further RCA is still under investigation
Resolution: The issue is mitigated after Card and 0CP traffic moved to 100% BDC and then returned to it's original state(A/A) at 12:45 AM ET
Card RRT:

Shital Telghane 5:04 AM
CHG12739795 - Card, Bank: IHS SSB Cache - Recreate Database Instance 2
ST
(p66m231r2) in the RAC database (p66m231r)
5:10 AM Meeting ended: 10m 24s






