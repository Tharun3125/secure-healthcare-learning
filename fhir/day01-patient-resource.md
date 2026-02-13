# Day 01 — Patient Resource Fundamentals

Today I created my first FHIR Patient resource manually.

A Patient is not just a record — it is the identity reference for all healthcare data.

Key concepts learned:

- FHIR is a communication contract, not a database schema
- Patient contains structured fields, not plain strings
- Name is repeatable (1..*) because identity varies across systems
- Other resources reference Patient instead of copying data

Important realization:
Healthcare systems rely on a single source of truth.  
All records connect back to Patient identity.

This prevents duplication and mismatching across hospitals.
