# Internal Compliance & Market Eligibility Decision Support Platform

A centralized decision-support platform designed to help operations agents instantly retrieve market-specific compliance, onboarding, and eligibility requirements across the United States and Canada.

---

## Overview

Internal Compliance & Market Eligibility Decision Support Platform was built to solve a common operational challenge:

Agents were required to search across multiple compliance resources, documentation repositories, spreadsheets, help center articles, and regional guides to determine market-specific requirements.

This process was:

- Time-consuming
- Prone to inconsistencies
- Dependent on agent experience
- Difficult to scale

To address this challenge, I designed and deployed a centralized lookup solution that allows agents to retrieve critical regional requirements through a single search.

By entering a region code, agents can instantly access eligibility, compliance, vehicle, driver, insurance, inspection, and regional requirement information from one unified interface.

---

## Business Problem

Prior to implementation, agents often had to navigate multiple systems to answer questions such as:

- Is this vehicle eligible in this market?
- What inspection is required?
- What is the minimum driver age?
- What documentation is required?
- Are there region-specific onboarding requirements?
- What time is it in the driver's market?

Finding this information could involve consulting multiple documentation sources and operational references.

---

## Solution

The platform consolidates market requirements into a single searchable source of truth.

Agents simply enter a region code and immediately receive:

- Market information
- State/province information
- Region type
- Vehicle eligibility rules
- Driver eligibility requirements
- Insurance requirements
- Inspection requirements
- Driving history requirements
- Regional onboarding requirements
- Local market time

---

## Key Features

### Instant Region Search

Quickly retrieve market requirements using a region code.

### Compliance Lookup

Access market-specific onboarding and compliance requirements.

### Vehicle Eligibility Validation

View market-specific vehicle age requirements and restrictions.

### Driver Eligibility Validation

Review minimum driver age and driving history requirements.

### Regional Requirement Tracking

Access special requirements unique to specific markets.

### Market Comparison Mode

Compare multiple regions side-by-side.

### Real-Time Local Clock

Display the current time in the searched region across US and Canadian markets.

### Intelligent Search Suggestions

Autocomplete support helps users find regions quickly.

### Feedback Collection

Built-in feedback mechanism enables continuous improvement.

### Performance Optimization

Server-side and client-side caching reduce lookup times and improve responsiveness.

---

## Impact

### Adoption

- 187 active users
- 3,726 executions within a 7-day period
- 0.03% error rate

### Operational Benefits

- Reduced dependency on multiple compliance resources
- Centralized fragmented operational knowledge
- Improved consistency in agent decision making
- Faster access to region-specific requirements
- Simplified onboarding support workflows
- Reduced lookup effort and handling time

---

## Technology Stack

### Frontend

- HTML5
- CSS3
- JavaScript

### Backend

- Google Apps Script

### Data Layer

- Google Sheets
- Script Properties Cache
- Browser Local Storage Cache

### Additional Capabilities

- Dynamic search suggestions
- Region comparison engine
- Timezone conversion
- Feedback collection workflow

---

## Architecture

```text
Operations Agent
        │
        ▼
 Region Lookup Interface
        │
        ▼
 Client-Side Cache
        │
        ▼
 Google Apps Script
        │
 ┌──────┴──────┐
 ▼             ▼
Server Cache  Data Source
(Properties)  (Google Sheets)
