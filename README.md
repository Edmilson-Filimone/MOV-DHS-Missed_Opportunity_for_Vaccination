# **Missed Opportunities for Vaccination (MOV) Analysis Using Mozambique DHS 2022–23 (Children 9–59 Months)**

This repository contains R scripts for computing Missed Opportunities for Vaccination (MOV) among children aged 9–59 months (under-5) using the Mozambique DHS 2022–23 dataset (Child Recode KR file).

The analysis follows WHO MOV methodology but adapts the eligibility window to include all children old enough to have received MR1 (≥9 months), up to 59 months, allowing analysis of catch-up vaccination, zero-dose, and delayed vaccination among older children.


**Objective**

To quantify Missed Opportunities for Vaccination (MOV) for Measles–Rubella first dose (MR1) among children 9–59 months, and to assess catch-up vaccination patterns using DHS data.

**Core Definitions
Eligibility**

*A child is eligible for MR1 if*:

They are 9–59 months old, and

They have vaccination card data.

**Zero-Dose for MR1**

A child is classified as zero-dose for MR1 if:

MR1 date is missing in the vaccination card and

Caregiver does not report MR1 and

Child is within 9–59 months.

Contact With Health Services After 9 Months

A child had a contact if they received any vaccine at age ≥9 months, including:

- PCV, 
- IPV
- Polio boosters
- Vitamin A
- Measles 2nd dose (if older)
- Any other vaccine recorded after 9 months

**Missed Opportunity for MR1 (MOV)**

Defined as:

`MOV_MR1 = 1 if (MR1 zero-dose) AND (received any other vaccine at age ≥9 months)`
