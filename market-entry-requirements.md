# Market Entry Requirements: RTO and Markets+

This document outlines the business, functional, and technical requirements for an electric utility to select, implement, and integrate the systems needed to participate in a Regional Transmission Organization (RTO) or the SPP Markets+.

---

## 1. Business Requirements

These requirements define the high-level business goals, justifications, and constraints for the project.

| Requirement Area | Description | Applicability |
| :--- | :--- | :--- |
| **Market Participation Strategy** | Define the strategic goals for market entry (e.g., lower cost of energy, increase reliability, integrate renewables, generate new revenue). | Both |
| **Cost-Benefit Analysis (CBA)** | A formal CBA must be conducted, projecting long-term costs (implementation, membership fees, operational overhead) against expected benefits (cost savings, market revenue). | Both |
| **Risk Management Framework** | Establish a comprehensive risk management policy defining trading limits, credit risk exposure, and hedging strategies. | Both (more complex for RTOs) |
| **Regulatory Compliance Plan** | Develop a plan to ensure adherence to all relevant regulations from FERC, NERC, and the specific market rules of the RTO or Markets+. | Both |
| **Stakeholder Engagement** | Identify and engage all internal stakeholders, including executive leadership, trading, legal, IT, and operations, to define roles and responsibilities. | Both |
| **Return on Investment (ROI)** | The selected solution and implementation plan must meet a defined ROI target and payback period. | Both |
| **Phased-in Participation** | A business plan for a phased approach, potentially starting with basic participation and expanding to more complex market products (e.g., Financial Transmission Rights - FTRs). | More relevant for Markets+ as a stepping stone. |

---

## 2. Functional Requirements

These requirements describe *what* the system must do to enable market participation.

| Requirement Area | Description | Applicability (Notes) |
| :--- | :--- | :--- |
| **Asset Registration & Management** | The system must be able to register and manage the technical attributes of physical assets (generators, loads, transmission facilities) with the market operator. | Both |
| **Bidding & Offering** | The system must allow traders to create, submit, validate, and manage various bid and offer types (e.g., three-part offers for generation, virtual/financial bids, demand response bids). | **RTO:** More complex, often includes a wider variety of auction types (e.g., FTRs, capacity).<br>**Markets+:** Focused on day-ahead and real-time energy. |
| **Market Data Ingestion** | The system must automatically download, process, and store all relevant market data, including Locational Marginal Prices (LMPs), ancillary service prices, and system status messages. | Both |
| **Real-Time Dispatch & Control** | The system must be able to receive, interpret, and act upon real-time dispatch signals (e.g., MW setpoints, startup/shutdown commands) from the market operator. | Both |
| **Settlements & Validation** | Functionality to receive settlement statements from the market, validate charges and credits against internal data ("shadow settlement"), and manage the dispute process. | **RTO:** Extremely complex, with many charge types.<br>**Markets+:** Initially simpler, focused on energy and imbalance. |
| **Outage Management** | The system must provide a means to submit, track, and manage planned and forced outages of generation and transmission assets with the market operator. | Both |
| **Reporting & Analytics** | Generate standard and ad-hoc reports for traders (e.g., P&L), operators (e.g., dispatch performance), and compliance officers (e.g., NERC reporting). | Both |
| **User Interface & Visualization** | Provide intuitive dashboards for traders and operators to visualize market prices, asset performance, system constraints, and other key operational data. | Both |
| **E-Tagging** | The system must be ableto create, submit, and manage electronic tags (E-Tags) for energy schedules that cross balancing authority boundaries. | Both |

---

## 3. Technical Requirements

These requirements describe *how* the system will be built and integrated, defining the necessary technology and standards.

| Requirement Area | Description | Applicability (Notes) |
| :--- | :--- | :--- |
| **System Architecture** | The solution must be highly available (24/7/365 with defined uptime SLAs, e.g., 99.99%) and fault-tolerant, with robust disaster recovery capabilities. | Both |
| **Market Interface/API** | The system must have a certified API to connect and communicate securely with the market operator's systems. | **RTO:** Often uses older XML/SOAP-based APIs.<br>**Markets+:** Utilizes modern RESTful APIs, which may simplify integration. |
| **Internal System Integration** | The solution must integrate seamlessly with existing utility systems, including the Energy Management System (EMS), SCADA, ETRM, and enterprise financial software. | Both |
| **Data Storage** | A high-performance database infrastructure, typically including a time-series database optimized for storing and retrieving large volumes of market data. | Both |
| **Performance & Latency** | The system must meet strict performance requirements for processing real-time dispatch signals and submitting bids within tight market windows (sub-second latency may be required). | Both |
| **Cybersecurity** | The system and its network infrastructure must be compliant with NERC CIP (Critical Infrastructure Protection) standards. This includes secure access control, data encryption, and regular security audits. | Both (NERC CIP is mandatory) |
| **Communication Protocols** | Must support industry-standard protocols, including ICCP (Inter-Control Center Communications Protocol) for real-time data exchange between control centers. | Both |
| **Scalability** | The architecture must be scalable to handle future growth in data volume, market complexity, and the number of participating assets. | Both |
