# Enterprise AP Invoice ALM - Sprint 1

## Overview
This repository contains the source-controlled, unpacked Dataverse solution schema for **InvoiceCore_v1**, implementing enterprise Application Lifecycle Management (ALM) practices for Microsoft Power Platform solutions.

## Solution Architecture
- **Publisher Prefix**: `vendor_`[cite: 1]
- **Core Entities**:
  - `vendor_Vendor`: Vendor master records and metadata[cite: 1].
  - `vendor_Invoice`: Accounts Payable invoice transaction tracking[cite: 1].
- **Relationships**: Configured unit, system user, team, and owner bindings[cite: 1].

## ALM Pipeline
1. **Unmanaged Export**: Extracted `InvoiceCore_v1_1_0_0_1.zip` from Power Apps Dev Environment[cite: 1].
2. **Schema Unpacking**: Unpacked binary package using `pac solution unpack` via Power Platform CLI in WSL Ubuntu[cite: 1].
3. **Version Control**: Source metadata tracked directly in Git (`src/` folder) with binary exclusions enforced via `.gitignore`[cite: 1].
