Card RRT:
IA0029347-Discover Card Customers are unable to load statements -3C
Issue- We started seeing errors with statement rest from 7:22 AM ET until 8:48 AM ET With end point
get_/v1/statements/_statementdate
Card Impact Discover card customers/Statement Viewing 13,137 non unique Customers, 2,081 unique customers via Web. 11056, unique Mobile customers .
Bank Impact - From 9:46 PM ET on 05/25 to Ongoing, Bank Customers sporadically experiencing issues with Bank SMC, when customer tried to access the latest statement PDF
it was not loading.
Cause- Initially Vault process was down on BDC, To mitigate the impact vault traffic was flipped to 100% ssB but later on it was hard down on both the sides.
Resolution - Vault team has restarted the vault process on SSB after second trial where live traffic was pointing which helped on mitigat ing the impact for SsB.
