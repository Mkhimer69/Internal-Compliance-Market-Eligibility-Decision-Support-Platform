# Internal Compliance & Market Eligibility Decision Support Platform

A centralized decision-support platform designed to help operations agents instantly retrieve market-specific compliance, onboarding, and eligibility requirements across the United States and Canada.

---

## Overview

The Internal Compliance & Market Eligibility Decision Support Platform was built to solve a common operational challenge.

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

Finding this information frequently involved consulting multiple documentation sources and operational references, increasing handling time and introducing opportunities for inconsistency.

---

## Solution

The platform consolidates market requirements into a single searchable source of truth.

Agents simply enter a region code and immediately receive:

- Market information
- State / Province information
- Region classification
- Vehicle eligibility requirements
- Driver eligibility requirements
- Insurance requirements
- Inspection requirements
- Driving history requirements
- Regional onboarding requirements
- Local market time

The result is faster decision-making, improved operational consistency, and reduced dependence on fragmented documentation.

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

Access region-specific criteria and onboarding requirements.

### Market Comparison Mode

Compare multiple regions side-by-side.

### Real-Time Local Clock

Display current local time for US and Canadian regions.

### Intelligent Search Suggestions

Autocomplete support helps users locate regions quickly.

### Feedback Collection

Built-in feedback mechanism enables continuous improvement.

### Performance Optimization

Server-side and client-side caching significantly reduce lookup times and improve responsiveness.

---

## Business Value

The platform transformed a multi-source research process into a single-search workflow.

Instead of navigating multiple operational resources, agents can retrieve eligibility and compliance requirements instantly using a region code.

Benefits include:

- Reduced lookup effort
- Faster decision making
- Improved consistency across agents
- Centralized operational knowledge
- Reduced reliance on institutional knowledge
- Enhanced onboarding support

---

## Screenshots

### Search Interface

Centralized search interface enabling agents to retrieve regional requirements using a single region code.

![region-result](https://raw.githubusercontent.com/Mkhimer69/Internal-Compliance-Market-Eligibility-Decision-Support-Platform/refs/heads/main/screenshots/search-interface.png)

---

### Region Results

Unified presentation of market-specific eligibility and compliance information.

![region-result](https://raw.githubusercontent.com/Mkhimer69/Internal-Compliance-Market-Eligibility-Decision-Support-Platform/refs/heads/main/screenshots/region-result.png)
---

### Comparison Mode

Side-by-side comparison capability for evaluating multiple regions simultaneously.

![comparison-mode](https://raw.githubusercontent.com/Mkhimer69/Internal-Compliance-Market-Eligibility-Decision-Support-Platform/refs/heads/main/screenshots/comparison-mode.png)

## Impact

### Adoption Metrics

| Metric | Value |
|----------|----------|
| Active Users | 187 |
| Weekly Executions | 3,726 |
| Error Rate | 0.03% |
| Status | Production |

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

- Dynamic Search Suggestions
- Region Comparison Engine
- Timezone Conversion
- Feedback Collection Workflow
- Performance Optimization Layer

---

## Version History

| Version | Highlights |
|----------|------------|
| 2.0 | Autocomplete, feedback system, server/client caching, enhanced UI |
| 1.5 | Region comparison, live timezone display |
| 1.0 | Initial market eligibility and compliance lookup platform |

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
(Local Storage)
        │
        ▼
 Google Apps Script
        │
 ┌──────┴──────┐
 ▼             ▼
Server Cache  Data Source
(Properties) (Google Sheets)
