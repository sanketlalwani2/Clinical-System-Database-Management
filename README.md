# National Family Clinic Database Management System

## Overview

The National Family Clinic, a network of clinics across major U.S. cities, requires a robust relational database system to replace its current file-based system. This database will manage data related to employees, patients, appointments, visits, treatments, billing, and insurance. This document provides a comprehensive overview of the design and implementation process for the clinic's new database system.

## Executive Summary

The project aims to design and implement a relational database for the National Family Clinic, enhancing data management and operational efficiency. The database will store and manage information regarding patients, staff, physicians, appointments, treatments, billing, and insurance. This report details the development process, from requirements gathering to full implementation, and includes conceptual and logical models, as well as the final implementation code.

## Problem Statement

### Goals
- Create a relational database system for managing patient visits and related data for both adult and pediatric care.

### Context
- Transition from a file-based system to a relational database to eliminate data duplication and improve record accuracy and accessibility.

### Scope
- **In-Scope:** Patient information, physician information, appointments, medical history, billing, payment, insurance, departments, and clinic branches.
- **Out-Scope:** Physician personal information, staff personal information, payroll, staff scheduling, and patient access to the database.

## Requirements

### Current System Analysis
- The current file-based system leads to data duplication, poor data quality, and inefficiency. Separate databases for different departments result in fragmented data management.

### Data Requirements
- The database will capture patient information, medical history, appointments, billing, payments, insurance, clinic branches, and departments.

### Business Rules and Logic
- Each clinic branch can schedule multiple patients and departments daily.
- Each department can serve multiple patients daily and must have at least one physician.
- Staff members, including managers and receptionists, play distinct roles in the clinic operations.

### Assumptions
- All patients must have a medical history record.
- Insurance information is updated as needed.
- Bills are expected to be paid within 90 days.
- Multiple payment methods are accepted.

## Solution Approach

### Tables and Relationships
- Key tables: Staff, Treatment, Billing, Payments, Insurance.
- Staff divided into Managers and Receptionists.
- Billing, Payment, and Insurance details are crucial for managing patient financial data.

### Data Collection
- Fictional data based on research and realistic data values were used for database requirements.

### Tools and Technologies
- Implementation was done using CCI Oracle.

## Implementation

- Detailed documentation and SQL commands for database creation, management, and querying are provided, ensuring easy replication and implementation by the client.

## Conclusion

The National Family Clinic’s new relational database system is designed to meet the clinic's needs, ensuring efficient data management and operational effectiveness. This database will support decision-making at clinical and executive levels, accommodating the clinic's growth and evolving needs.
