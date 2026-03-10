
# Hospital Dataset – Explanation (README Style)
Project Overview

This dataset represents a Hospital Management System database used to store and manage information about patients, doctors, treatments, billing, beds, drugs, and hospital staff.

It is designed for data analysis, database design, or Power BI dashboard projects.

The database schema includes multiple relational tables connected through primary and foreign keys.

# Dataset Structure
Core Entities

# 1. Patient
Stores patient personal details.

Fields typically include:
> patient_id
> name
> gender
> age
> contact info

# 2. Doctor
Contains doctor information.

Examples:

> doctor_id
> doctor_name
> specialization
> department_id

# 3. Department
Hospital departments.

Examples:

> department_id
> department_name
> department_head

 Example departments:

> Cardiology
> Neurology
>Orthopedics

# 4. Admission 
Tracks hospital admissions.

Includes:

> admission_id
> patient_id
> admission_date
> discharge_date
> ward_id

# 5. Ward
Information about hospital wards.

Fields:

> ward_id
> ward_name
> capacity

# 6. Bed
Tracks beds available in wards.

Fields:

> bed_id
> ward_id
> bed_status

# Medical Information Tables
Diagnostic Test

Tests conducted for patients.

Examples:

> test_id
> test_name
> cost

# Patient Diagnostic

Links patients with diagnostic tests.

Fields:

> patient_id
> test_id
> result

# Disease

Stores diseases treated in the hospital.

Examples:

> disease_id
> disease_name

# Pharmacy Tables
Drug

Drug information.

Examples:

> drug_id
> drug_name
> manufacturer_id
>price

# Drug Inventory

Tracks stock of medicines.

Fields:

drug_id

quantity

expiry_date

# Drug Manufacturer

Details about medicine manufacturers.

Examples:

> manufacturer_id
> company_name

# Prescription

Contains medication prescribed to patients.

Fields:

> prescription_id
> patient_id
> doctor_id
> drug_id
> dosage

# Billing System
Billing

Patient bill summary.

Fields:

> billing_id
> patient_id
> admission_id
> total_amount

# Billing Detail

Breakdown of charges.

Examples:

> consultation fee
> room charge
> lab test cost

medicine cost

# Insurance
Insurance Provider

Insurance companies.

Examples:

> provider_id
> provider_name

# Patient Insurance

Links patients with insurance providers.

Fields:

> patient_id
> insurance_id
> policy_number

# Staff Tables
Employee

Hospital staff information.

Examples:
> employee_id
> employee_name
> role

# Staff Assignment

Tracks staff assigned to wards.

Fields:
> employee_id
> ward_id
> shift

# Database Relationships

The schema connects tables such as:

> Patient → Admission
> Admission → Ward
> Ward → Bed
> Patient → Billing
> Doctor → Prescription
> Patient → Diagnostic Tests
> Drug → Prescription

This creates a relational hospital database system.
