# High-Level Cost Estimate: Markets+ Entry for RTO

**Document Version:** 1.0
**Date:** December 17, 2025
**Prepared For:** RTO Markets+ Entry Project

---

## Executive Summary

This document provides a high-level cost estimate for an **established electric utility with existing operational systems** to integrate with the SPP Markets+ environment. This estimate assumes the utility already has core infrastructure in place (generation assets, EMS/SCADA, control rooms, transmission management) and is focused on **integration and enhancement** rather than building systems from scratch.

**Total Estimated Investment Range:**
- **Year 0 (Implementation):** $4.6M - $8.8M
- **Year 1 (Operations):** $2.7M - $5.0M
- **Year 2 (Operations):** $2.7M - $5.0M
- **Year 3 (Operations):** $2.7M - $5.0M

**3-Year Total Cost Range:** $12.7M - $23.8M
**Conservative Mid-Point:** ~$18.3M

The range reflects differences in utility size, existing system maturity, integration complexity, vendor selection (build vs. buy), and the scope of market participation. **These costs represent incremental investment to add market participation capabilities to an already-functioning utility operation.**

---

## Cost Assumptions

This estimate assumes an **established utility** with the following characteristics:

**Existing Infrastructure (Already in Place):**
- Medium-sized utility with 500-1500 MW of generation capacity
- Operational Energy Management System (EMS) and SCADA infrastructure
- Existing control room operations and trained operators
- Generation assets with basic telemetry and controls
- Transmission and distribution management systems
- Corporate IT infrastructure and networks
- Basic cybersecurity framework (requires NERC CIP enhancement)

**Integration Scope:**
- Participation in Day-Ahead and Real-Time energy markets (not ancillary services initially)
- Vendor solutions for new market-specific systems rather than full in-house development
- **Integration and enhancement** of existing EMS/SCADA (not replacement)
- New market gateway, ETRM, and forecasting systems that integrate with existing infrastructure
- Phased implementation over 12-18 months
- Conservative approach to Markets+ as preparation for potential full RTO participation

**Key Principle:** Costs represent adding market participation capabilities to existing utility operations, not building a utility from the ground up.

---

## Why These Costs Are Realistic for Integration

This estimate reflects an **integration project** rather than a transformation or greenfield build:

**What You're NOT Doing:**
- Building a new EMS or SCADA system ($5-15M saved)
- Constructing control room facilities ($2-5M saved)
- Implementing core generation controls ($3-10M saved)
- Building enterprise IT infrastructure from scratch ($2-8M saved)
- Hiring and training an entire utility workforce ($10M+ annual saved)

**What You ARE Doing:**
- Adding a market gateway layer that connects to existing systems via APIs
- Enhancing existing ETRM or implementing lightweight market-specific trading software
- Creating middleware/integration code to bridge market systems with legacy infrastructure
- Training existing staff on new market processes
- Adding targeted market-specific roles (traders, analysts) to existing teams
- Implementing market-specific reporting and analytics

**Why Integration is the Majority of Cost:**
The largest cost category is system integration ($800K-$1.5M) because connecting new market platforms to 10-15 year old utility systems requires custom API development, data mapping, and workflow automation. This is labor-intensive but avoids the much higher cost of replacing functional legacy systems.

---

## 1. Upfront Implementation Costs (Year 0)

### 1.1 Technology & Software Systems

**Note:** These costs represent **new systems** (market gateway, ETRM, forecasting) that integrate with existing utility infrastructure, plus **enhancements** to existing systems (EMS/SCADA, cybersecurity). This is not a greenfield build.

| Cost Category | Low Estimate | High Estimate | Notes |
|--------------|--------------|---------------|-------|
| **Market Gateway/Interface System** | $400,000 | $800,000 | **NEW SYSTEM**: Vendor platform for API connectivity to Markets+ REST API, bid/offer management, real-time dispatch interface. Integrates with existing EMS. |
| **ETRM System Enhancement** | $300,000 | $600,000 | **ENHANCEMENT**: Add Markets+ settlement modules to existing trading system or license basic ETRM if none exists. Full utilities typically have some trading capability. |
| **Forecasting & Analytics Tools** | $200,000 | $400,000 | **NEW SYSTEM**: Market-specific load and price forecasting, optimization tools. May leverage existing forecasting infrastructure. |
| **Time-Series Database** | $100,000 | $200,000 | **NEW INFRASTRUCTURE**: Market data storage (LMPs, schedules). May use existing database infrastructure with expansion. |
| **EMS/SCADA Integration** | $300,000 | $800,000 | **INTEGRATION**: API development, middleware to connect existing EMS/SCADA with market gateway, communications upgrades |
| **Cybersecurity Enhancements** | $200,000 | $400,000 | **ENHANCEMENT**: Incremental NERC CIP hardening for market systems, network segmentation for market zone |
| **Reporting & Dashboard Tools** | $100,000 | $250,000 | **NEW SYSTEM**: Market-specific dashboards. May extend existing reporting platforms. |
| **E-Tagging Integration** | $50,000 | $150,000 | **INTEGRATION**: Interface with WECC E-Tag system for scheduling |
| **Outage Management Integration** | $30,000 | $100,000 | **INTEGRATION**: Connection with SPP CROW system |
| **Testing Environment** | $100,000 | $200,000 | Non-production environment for testing and training |
| **Software Licenses (Year 1)** | $150,000 | $300,000 | First-year licenses for new market platforms |
| **SUBTOTAL - Technology** | **$1,930,000** | **$4,200,000** | |

### 1.2 Implementation Services

**Note:** System integration is a **major cost driver** because new market-specific systems must interface with multiple existing utility systems (EMS, SCADA, corporate financial systems, GIS, asset management, etc.). Integration complexity depends heavily on the age and architecture of existing systems.

| Cost Category | Low Estimate | High Estimate | Notes |
|--------------|--------------|---------------|-------|
| **System Integration** | $800,000 | $1,500,000 | **CRITICAL**: Integration labor (vendor + internal IT), API/middleware development between market systems and existing EMS/SCADA, data mapping, workflow automation. Lower if existing systems are modern with good APIs. |
| **Consulting Services** | $300,000 | $600,000 | Market strategy, vendor selection support, integration architecture design, business process optimization |
| **Testing & Certification** | $150,000 | $300,000 | UAT, parallel testing with existing systems, SPP Markets+ certification testing |
| **Training Development & Delivery** | $100,000 | $200,000 | Training existing staff on new market systems and SPP Markets+ rules |
| **Data Migration & Validation** | $75,000 | $150,000 | Asset registration data from existing systems, validation scripts, data quality remediation |
| **Process Redesign & Documentation** | $75,000 | $125,000 | Business process mapping, operational playbooks for market participation |
| **SUBTOTAL - Services** | **$1,500,000** | **$2,875,000** | |

### 1.3 Internal Personnel Costs (Implementation Phase)

| Resource | FTE | Months | Low Estimate | High Estimate | Notes |
|----------|-----|--------|--------------|---------------|-------|
| **Project Manager** | 1.0 | 15 | $225,000 | $300,000 | Dedicated PM for 12-15 month implementation |
| **IT Architects/Engineers** | 2.5 | 12 | $450,000 | $600,000 | Integration specialists, database, network engineers |
| **Trading Analyst/Subject Matter Expert** | 0.5 | 15 | $113,000 | $150,000 | Part-time dedication during implementation |
| **Operations SME** | 0.5 | 12 | $90,000 | $120,000 | Control room integration specialist |
| **Compliance/Legal Support** | 0.25 | 15 | $56,000 | $75,000 | Contract review, regulatory filings |
| **Business Analyst** | 0.75 | 12 | $135,000 | $180,000 | Requirements gathering, testing coordination |
| **SUBTOTAL - Internal Labor** | | | **$1,069,000** | **$1,425,000** | |

### 1.4 Market Entry & Membership

| Cost Category | Low Estimate | High Estimate | Notes |
|--------------|--------------|---------------|-------|
| **Initial Membership Fee** | $50,000 | $150,000 | One-time or reduced first-year fee (varies by market operator) |
| **Credit Requirements/Collateral** | $0 | $0 | Not a cost but may require posting collateral/letter of credit |
| **Legal & Regulatory Filings** | $50,000 | $100,000 | FERC filings, contract negotiations with SPP |
| **SUBTOTAL - Market Entry** | **$100,000** | **$250,000** | |

---

### **TOTAL YEAR 0 (IMPLEMENTATION): $4,599,000 - $8,750,000**
*(Conservative Mid-Point: ~$6.7M)*

**Cost Breakdown:**
- Technology & Software: $1,930,000 - $4,200,000 (42-48%)
- Implementation Services: $1,500,000 - $2,875,000 (33-33%)
- Internal Personnel: $1,069,000 - $1,425,000 (23-16%)
- Market Entry: $100,000 - $250,000 (2-3%)

---

## 2. Ongoing Annual Operational Costs

### 2.1 Personnel (Steady-State Operations)

| Role | FTE | Annual Cost Range | Notes |
|------|-----|-------------------|-------|
| **Energy Traders/Schedulers** | 2.0 - 3.0 | $400,000 - $750,000 | 24/7 coverage for bidding and real-time markets |
| **Market Analysts** | 1.0 - 2.0 | $150,000 - $300,000 | Price forecasting, optimization, strategy |
| **Control Room Integration** | 0.5 | $75,000 - $100,000 | Incremental operator training and oversight |
| **IT Support & Administration** | 1.5 | $225,000 - $300,000 | System administration, database management, support |
| **Settlements Analyst** | 1.0 | $120,000 - $180,000 | Shadow settlements, dispute management |
| **Compliance Officer (Incremental)** | 0.5 | $75,000 - $100,000 | Market rule monitoring, reporting |
| **SUBTOTAL - Personnel** | **6.5 - 8.5 FTE** | **$1,045,000 - $1,730,000** | |

### 2.2 Technology & Software (Annual Recurring)

| Cost Category | Annual Cost Range | Notes |
|--------------|-------------------|-------|
| **Software Licenses & Maintenance** | $600,000 - $1,200,000 | Annual fees for ETRM, market gateway, forecasting tools (typically 18-22% of purchase price) |
| **Cloud/Hosting Infrastructure** | $150,000 - $300,000 | If using cloud-based solutions for databases, analytics |
| **SCADA/EMS Maintenance** | $100,000 - $200,000 | Incremental support for upgraded systems |
| **Cybersecurity (Ongoing)** | $150,000 - $250,000 | Security monitoring, audits, updates, penetration testing |
| **Data Services** | $50,000 - $100,000 | Third-party market data feeds, weather data subscriptions |
| **SUBTOTAL - Technology** | **$1,050,000 - $2,050,000** | |

### 2.3 Market Participation & Membership Fees

| Cost Category | Annual Cost Range | Notes |
|--------------|-------------------|-------|
| **SPP Markets+ Annual Membership** | $200,000 - $500,000 | Varies based on utility size and load served; estimate for medium utility |
| **Scheduling & Ancillary Fees** | $100,000 - $200,000 | Transaction fees, administrative charges |
| **SUBTOTAL - Market Fees** | **$300,000 - $700,000** | |

### 2.4 Other Recurring Costs

| Cost Category | Annual Cost Range | Notes |
|--------------|-------------------|-------|
| **Training & Professional Development** | $50,000 - $100,000 | Ongoing market training, vendor training, conferences |
| **Consulting Support (As Needed)** | $100,000 - $200,000 | Market strategy reviews, system optimizations |
| **Legal & Compliance** | $50,000 - $100,000 | Contract amendments, regulatory support |
| **Contingency & Miscellaneous** | $100,000 - $150,000 | Unplanned expenses, small enhancements |
| **SUBTOTAL - Other** | **$300,000 - $550,000** | |

---

### **TOTAL ANNUAL OPERATING COSTS (Years 1-3):**

| Year | Low Estimate | High Estimate | Notes |
|------|--------------|---------------|-------|
| **Year 1** | $2,695,000 | $5,030,000 | Full first year of operations; may include ramp-up costs |
| **Year 2** | $2,695,000 | $5,030,000 | Steady-state operations |
| **Year 3** | $2,695,000 | $5,030,000 | Steady-state operations |

*(Note: Costs may decrease slightly in Years 2-3 as teams mature and consulting needs diminish. Conservative estimate holds costs flat.)*

---

## 2.5 What's NOT Included (Existing Utility Infrastructure)

**Important:** This estimate assumes the utility already owns and operates the following systems and capabilities. These costs are **NOT** included in the estimates above:

**Operational Systems (Already Owned):**
- Energy Management System (EMS) base platform
- SCADA infrastructure (RTUs, PLCs, field communications)
- Generation assets and control systems
- Transmission and distribution infrastructure
- Corporate IT infrastructure (servers, networks, workstations)
- Enterprise Resource Planning (ERP) and financial systems
- Existing control room facilities and operator workstations

**Personnel (Already Employed):**
- Plant operators and control room staff (base staffing)
- IT infrastructure and support teams (base staffing)
- Engineering and maintenance personnel
- Executive and administrative staff
- Legal and compliance teams (base functions)

**Note:** The personnel costs in Section 1.3 and 2.1 represent **incremental** or **new** roles specifically for market participation (traders, market analysts, integration specialists), not the utility's entire workforce.

---

## 3. Summary of 3-Year Total Cost of Ownership

| Period | Low Estimate | High Estimate |
|--------|--------------|---------------|
| **Year 0 (Implementation)** | $4,599,000 | $8,750,000 |
| **Year 1 (Operations)** | $2,695,000 | $5,030,000 |
| **Year 2 (Operations)** | $2,695,000 | $5,030,000 |
| **Year 3 (Operations)** | $2,695,000 | $5,030,000 |
| **3-Year Total** | **$12,684,000** | **$23,840,000** |
| **Conservative Mid-Point** | **~$18.3M** | |

---

## 4. Key Cost Drivers & Sensitivities

### Higher Cost Scenarios (pushing toward $8-9M Year 0)
- **Large utility (>1500 MW):** Scale factor increases technology and personnel costs by 25-35%
- **Legacy system replacement:** If existing EMS/SCADA is too old/incompatible and requires replacement instead of integration, add $2-4M
- **Build vs. Buy:** In-house development of market gateway/ETRM could add $2-4M but reduce annual license fees by 40-60%
- **Complex bidding strategies:** Advanced optimization and ancillary service participation adds $500K-$1M
- **Full RTO preparation:** If simultaneously building capability for full RTO (CAISO, SPP RTO) instead of just Markets+, costs increase 30-50%
- **Poor existing data quality:** Asset data cleanup, metering infrastructure upgrades, or GIS remediation adds $500K-$1.5M
- **Multiple legacy systems:** Utilities with 3+ separate legacy platforms requiring individual integrations add $400K-$800K

### Lower Cost Scenarios (pushing toward $4-5M Year 0)
- **Small utility (<500 MW):** Technology and personnel costs scale down 25-35%
- **Modern existing systems:** Well-integrated EMS with open APIs, existing ETRM platform reduces integration by 30-40%
- **Markets+ Day-Ahead Only:** Starting with day-ahead market only (adding real-time later) reduces initial scope by 20-25%
- **Phased approach:** Limited initial participation (fewer assets, single BA) reduces complexity
- **Vendor bundling:** Selecting vendors with pre-built SPP Markets+ integrations reduces custom development by 25-40%

---

## 5. Risk Factors & Contingencies

### Technical Risks
- **Integration complexity with existing systems:** Older legacy EMS/SCADA may lack modern APIs, requiring custom middleware development and potentially increasing integration costs by 30-50%
- **Existing system compatibility:** Some existing systems may be incompatible with new market requirements, forcing partial replacements
- **API maturity:** While Markets+ uses modern REST APIs, there may be early-stage issues as the market is relatively new
- **Data quality from existing systems:** Poor asset data, incomplete metering infrastructure, or inaccurate GIS data in existing systems requires remediation before integration
- **Organizational change management:** Existing staff may resist new workflows and systems, requiring additional training and change management effort

### Financial Risks
- **Market volatility:** Unexpected market conditions in first year could impact P&L
- **Regulatory changes:** New requirements from FERC or SPP could trigger additional investments
- **Vendor performance:** Delays or issues with vendor platforms can increase costs and timeline

### Mitigation Recommendations
- Allocate 15-20% contingency budget for implementation phase (~$700K-$1.5M reserve)
- **Conduct thorough existing system assessment FIRST** - this is critical to accurate scoping
- Negotiate fixed-price contracts for software and integration services where possible
- Plan for 12-18 month implementation timeline to allow adequate integration and testing
- Select vendors with proven SPP Markets+ integration experience
- Establish executive steering committee for governance and risk management
- Consider phased approach: Day-ahead market first, then add real-time market

---

## 6. Expected Benefits (Not Quantified in This Estimate)

While this document focuses on costs, the business case should also consider:

- **Wholesale energy cost savings:** Access to broader, more liquid market
- **Renewable integration benefits:** Better management of variable resources
- **Grid reliability improvements:** Access to regional balancing and reserves
- **Revenue opportunities:** Ability to sell excess generation and ancillary services
- **Market intelligence:** Price transparency and improved forecasting
- **Strategic positioning:** Preparation for potential full RTO membership

A full cost-benefit analysis should quantify these benefits against the costs outlined above to calculate Net Present Value (NPV) and Return on Investment (ROI).

---

## 7. Recommended Next Steps

1. **Existing System Assessment (CRITICAL FIRST STEP):** Conduct detailed audit of current IT infrastructure, including:
   - EMS/SCADA age, version, API capabilities, and vendor support status
   - Data quality assessment (asset records, metering, GIS accuracy)
   - Network architecture and cybersecurity posture
   - Integration points and middleware capabilities
   - Identification of systems that may require replacement vs. enhancement

2. **Stakeholder Engagement:** Conduct workshops with operations, trading, IT, and executive teams using questions from `markets-questions.md`

3. **Integration Architecture Design:** Define how new market systems will connect with existing infrastructure before selecting vendors

4. **Vendor RFI/RFP:** Issue Request for Information to market platform vendors, emphasizing integration requirements with existing systems

5. **Pilot Study:** Consider limited participation or market simulation before full entry

6. **Business Case Development:** Quantify expected benefits and complete formal CBA

7. **Governance Framework:** Establish project governance, risk management, and decision-making structure

---

## Appendix A: Cost Estimate Methodology

This estimate is based on:
- Industry benchmarks from similar utility market entry projects (2020-2025)
- Vendor quotes and public pricing for market systems (2024-2025)
- SPP Markets+ documentation and fee schedules
- Consultation with utilities that have joined western markets
- Standard IT implementation cost models
- Regulatory filings and public documents from recent market entries

**Confidence Level:** Medium-High for Year 0 implementation costs; Medium for ongoing operational costs due to variability in utility operations and market conditions.

**Cost Basis:** 2025 USD. Costs should be escalated 3-4% annually for inflation in future planning.

---

## Document Control

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | 2025-12-17 | Initial | First draft cost estimate |

---

*This is a planning document for internal use. Actual costs will vary based on specific utility circumstances, market conditions, and implementation decisions. A detailed bottom-up estimate should be developed during the project planning phase.*
