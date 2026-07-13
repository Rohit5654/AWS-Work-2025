Bank RRT:
IAB029849 Bank Customers experiencing technical difficulties accessing Home Screen - P3
Impact - From 8:00 PM to 10:06 PM on 07/07, customers faced difficulty in accessing Bank ACHome Account activity
widget via mobile and web.
117 unique customers unable to access Bank Achome in web 119 unique customers unable to access activity in Bank Achome
page via web, 746 unique customers unable to access activity in Bank Achome page via mobile, 77 unique customers
unable to perform funds transfer in mobile
Root Cause - It was identified that a recently renewed certificate was not properly taking effect on a specific
cluster within the Enterprise IHS API Gateway, causing it to present an expired certificate.
Resolution - App team cleared cache by performing a dummy operation so that the new certificate can be uploaded.
Card RRT:
