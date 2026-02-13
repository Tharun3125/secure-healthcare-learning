# Day 01 — How Systems Communicate Before Authentication

Today I explored what actually happens when a client calls an API.

Communication flow:
Client → DNS → TCP → TLS → HTTP → Server → Response

Key understanding:
HTTPS only encrypts communication.  
It does not decide whether a user is allowed to access data.

That responsibility belongs to authentication and authorization.

Important realization:
A secure healthcare API needs both:
1) Secure channel (HTTPS)
2) Proper access control (permissions)

Healthcare relevance:
Even if FHIR APIs are encrypted, incorrect authorization can still expose patient data.
