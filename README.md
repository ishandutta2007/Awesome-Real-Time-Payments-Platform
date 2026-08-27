# Awesome-Real-Time-Payments-Platform

Edit
Top Real-Time Payments Platforms Ecosystem

Curated List of SaaS Products & Open-Source GitHub Projects
Focused on Instant Payments, RTP/FedNow, Payment Orchestration, ISO 20022, Banking APIs & Real-Time Money Movement
Last updated: August 2026

This repository tracks notable SaaS/hosted platforms and open-source projects for Real-Time Payments Platforms. These platforms enable banks, fintechs, enterprises, and payment providers to initiate, receive, route, process, reconcile, and monitor instant payments across domestic and cross-border payment rails.

Examples include Modern Treasury, Moov, Form3, Finzly, Volante Technologies, ACI Worldwide, Fiserv NOW, Finastra Payments To Go, ICON Solutions, and ClearBank.

Open-source emphasis: This section is heavily expanded with open-source payment infrastructure, ISO 20022 implementations, RTP/FedNow message libraries, payment gateways, ledger systems, banking APIs, payment orchestration components, and real-time transaction-processing projects. A particularly useful open-source ecosystem comes from Moov, which maintains projects for RTP, FedNow, Fedwire, ACH, ISO 20022, and other financial infrastructure components. Moov's rtp20022 repository specifically implements ISO 20022 messages for Real Time Payments and has been used for RTP certification releases.

Unlike commercial platforms, most open-source projects are building blocks rather than complete certified instant-payment switches. Connecting directly to production payment rails generally requires bank/participant relationships, certification, security controls, compliance, and access credentials.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites or repositories.

Table of Contents

SaaS/Hosted Platforms

Open-Source GitHub Projects

Additional Strong Open-Source Options

Building a Self-Hosted Real-Time Payments Stack

How to Contribute

Disclaimer

SaaS/Hosted Platforms

Modern Treasury
Payments operations platform providing payment infrastructure, payment workflows, ledgers, reconciliation, and connectivity to multiple payment rails.

Moov
Developer-focused payments infrastructure platform supporting ACH, RTP, FedNow, card payments, payouts, and other money-movement capabilities through APIs. Moov also maintains a substantial open-source financial-infrastructure ecosystem.

Form3
Cloud-native payment processing platform providing API-based access to payment schemes and infrastructure for banks and financial institutions.

Finzly
Payments-as-a-service and payment-hub platform supporting real-time payments, FedNow, RTP, ACH, wires, APIs, and payment orchestration.

Volante Technologies
Cloud-native payments processing and orchestration platform supporting ISO 20022, instant payments, FedNow, RTP, wires, and other domestic and international payment schemes.

ACI Worldwide
Enterprise payments software provider offering real-time payments processing, payment switching, fraud management, digital payments, and banking infrastructure.

Fiserv NOW
Fiserv's real-time payments and modern payment infrastructure capabilities supporting banks and financial institutions with instant-payment processing and connectivity.

Finastra Payments To Go
Cloud-based payment processing capabilities designed to help financial institutions modernize payment operations and support emerging payment schemes.

ICON Solutions
Financial-services technology provider specializing in payment infrastructure, payment modernization, integration, and real-time payment solutions.

ClearBank
Cloud-native clearing bank providing banking-as-a-service infrastructure and access to UK payment schemes, including Faster Payments and other real-time banking capabilities.

Additional Notable SaaS / Hosted Platforms

The Clearing House RTP — U.S. real-time payment rail and infrastructure.

FedNow — Federal Reserve instant payment service.

Mastercard Send — Real-time push-payment infrastructure.

Visa Direct — Push-to-card payment infrastructure.

Banking Circle — Payments and banking infrastructure for financial institutions.

Temenos — Core banking and payment processing infrastructure.

FIS — Enterprise banking and payments infrastructure.

Bottomline — Payment automation and financial technology infrastructure.

ACI Speedpay — Real-time and digital payment capabilities.

Paymentology — Issuing and payment-processing infrastructure.

Nium — Global real-time payment and money-movement infrastructure.

Thunes — Cross-border payment and payout infrastructure.

Airwallex — Global payments and financial infrastructure APIs.

Adyen — Global payment processing and financial infrastructure.

Stripe — Payments infrastructure and programmable financial services.

Checkout.com — Global payment processing infrastructure.

Open-Source GitHub Projects

Moov RTP 20022
Open-source Go implementation of ISO 20022 messages for U.S. Real Time Payments. The project contains message structures for RTP and has been used to support RTP certification releases.

Moov FedNow 20022
Open-source Go implementation containing ISO 20022 message definitions for FedNow payments, providing a useful building block for FedNow integrations.

Moov ISO 20022
Open-source Go library and HTTP tooling for creating, parsing, validating, and converting ISO 20022 messages. The project is being superseded by more targeted repositories such as rtp20022.

Moov Fedwire 20022
Open-source ISO 20022 message implementation for Fedwire Funds Service integrations.

OpenFedNow
Open-source middleware architecture for connecting legacy core banking systems with FedNow and RTP. It includes ISO 20022 models, transaction orchestration, idempotency, fraud pre-screening, a shadow ledger, sandbox adapters, and legacy-core adapters.

Moov ACH
Open-source financial infrastructure for generating, parsing, validating, and processing ACH files and transactions.

Moov Wire
Open-source Fedwire file-processing library for legacy FAIM formats. Fedwire moved to ISO 20022 in July 2025, so this project is now primarily useful for historical files, migration, and archival processing.

Moov Paygate
Open-source REST API infrastructure for processing electronic payments without requiring applications to directly understand underlying payment-file specifications.

Moov Watchman
Open-source financial compliance infrastructure for searching sanctions and related watchlists.

Moov Fed
Open-source utilities for interacting with Federal Reserve-related financial institution and routing information.

Moov Accounts
Open-source banking-account and financial-infrastructure building blocks within the Moov ecosystem.

Moov Money
Moov's broader open-source ecosystem provides individual components for payment processing, banking integrations, financial messaging, compliance, and money movement.

Additional Strong Open-Source Options

Apache Fineract — Open-source core banking platform that can serve as a foundation around which payment infrastructure can be integrated.

Mifos X / Fineract — Open-source financial-services and core-banking ecosystem.

ERPNext — Open-source ERP with accounting and payment-related capabilities.

Kill Bill — Open-source payments, billing, and subscription platform.

Medusa — Open-source commerce infrastructure with extensible payment integrations.

Apache Camel — Integration framework useful for connecting banking/payment systems and message-processing pipelines.

Apache Kafka — Distributed event-streaming infrastructure suitable for real-time payment-event processing.

Temporal — Open-source durable workflow engine useful for payment orchestration and long-running transaction workflows.

Debezium — Open-source CDC platform useful for streaming core-banking and payment data into real-time processing systems.

PostgreSQL — Open-source transactional database suitable for payment ledgers and transaction state.

Redis — In-memory data infrastructure useful for idempotency, caching, rate limits, and real-time payment processing.

Keycloak — Open-source identity and access management for payment APIs and banking applications.

OpenTelemetry — Open-source observability framework for tracing payment transactions across distributed systems.

Building a Self-Hosted Real-Time Payments Stack

A practical open-source real-time payments architecture can combine:

API Gateway → Payment Orchestrator → ISO 20022 Engine → Rail Adapter → RTP/FedNow

with:

Core Banking → Ledger → Event Bus → Reconciliation → Fraud/Risk → Notifications

The architecture can be implemented using open-source components such as:

Moov RTP 20022 + Moov FedNow 20022 + Temporal + Kafka + PostgreSQL + Redis + OpenTelemetry

This does not constitute a complete certified replacement for a commercial payment switch, but it provides many of the software building blocks needed to construct one.

Core Real-Time Payments Functions

Payment Initiation — APIs for creating instant payment instructions.

Payment Routing — Determine the appropriate payment rail and participant.

Payment Orchestration — Coordinate multi-step payment workflows.

ISO 20022 Processing — Generate, parse, validate, and transform financial messages.

RTP Processing — Support The Clearing House RTP message flows.

FedNow Processing — Support Federal Reserve instant-payment message flows.

Payment Status Tracking — Track transactions from initiation through settlement.

Idempotency — Prevent duplicate payment execution.

Ledgering — Maintain real-time balances and transaction state.

Fraud Screening — Apply transaction-level risk rules before execution.

Sanctions Screening — Screen participants against relevant watchlists.

Account Validation — Validate beneficiary and account information.

Payment Limits — Enforce customer, account, and transaction limits.

Liquidity Management — Monitor available liquidity for instant settlement.

Exception Handling — Handle rejects, returns, timeouts, cancellations, and reversals.

Reconciliation — Reconcile payment-rail transactions with the core ledger.

Notifications — Generate real-time transaction notifications.

Auditability — Maintain immutable payment and state-transition records.

Observability — Trace payment transactions across distributed services.

High Availability — Operate continuously because instant-payment rails are available around the clock.

Disaster Recovery — Maintain resilient processing across infrastructure failures.

Payment Analytics — Analyze transaction volumes, latency, failure rates, and fraud patterns.

Real-Time Payment Processing Flow

A typical instant-payment flow can be modeled as:

Customer → API → Authentication → Risk/Fraud → Account Validation → Payment Orchestrator → ISO 20022 → RTP/FedNow Adapter → Payment Rail → Receiving Institution → Confirmation

The transaction state can then flow through:

Initiated → Validated → Risk Approved → Submitted → Accepted → Settled → Reconciled

with alternative paths such as:

Rejected → Returned → Reversed → Exception Queue

Real-Time Payments Ledger

A robust system should maintain a transactional ledger independently from payment-rail messaging:

Payment Request → Ledger Reservation → Rail Submission → Settlement Confirmation → Ledger Commit

This separation makes it possible to maintain consistent financial state even when external payment networks or legacy core systems respond asynchronously.

Payment Orchestration Layer

A payment orchestration layer can abstract multiple rails behind a single internal API:

Unified Payment API

→ RTP
→ FedNow
→ ACH
→ Fedwire
→ Visa Direct
→ Mastercard Send
→ SEPA Instant
→ Faster Payments
→ PIX
→ UPI
→ Other domestic instant-payment schemes

This allows applications to initiate payments without embedding every rail's proprietary integration into the business logic.

ISO 20022 as the Messaging Foundation

ISO 20022 is particularly important for modern real-time payment infrastructure because it provides standardized financial messaging across payment networks.

Open-source libraries such as Moov RTP 20022 and Moov FedNow 20022 provide reusable implementations for payment-message processing.

Typical payment messages include:

pacs.008 — Financial Institution to Financial Institution Customer Credit Transfer

pacs.002 — Payment Status Report

pacs.004 — Payment Return

camt.056 — Payment Cancellation Request

camt.029 — Resolution of Investigation

Other pacs, camt, and related ISO 20022 message families

Building a Modern Open-Source Payment Platform

A possible architecture is:

┌───────────────────────────────┐
│ Customer / Merchant / Bank UI │
└───────────────┬───────────────┘
** ↓**
┌───────────────────────────────┐
│ API Gateway / Authentication │
└───────────────┬───────────────┘
** ↓**
┌───────────────────────────────┐
│ Payment Orchestration Engine │
└───────────────┬───────────────┘
** ↓**
┌───────────────────────────────┐
│ Risk / Fraud / Compliance │
└───────────────┬───────────────┘
** ↓**
┌───────────────────────────────┐
│ ISO 20022 Message Engine │
└───────┬───────────┬───────────┘
** ↓ ↓**
** RTP Adapter FedNow Adapter**
** ↓ ↓**
** RTP Network FedNow Network**
** │ │**
** └─────┬─────┘**
** ↓**
** Ledger / Reconciliation**
** ↓**
** Analytics / Observability**

Recommended Open-Source Stack

For a U.S. instant-payments research stack:

Moov RTP 20022 + Moov FedNow 20022 + OpenFedNow + PostgreSQL + Kafka + Temporal + Redis + OpenTelemetry

For payment messaging:

Moov ISO 20022 + RTP 20022 + FedNow 20022

For workflow orchestration:

Temporal + Kafka

For ledgering:

PostgreSQL + application-level double-entry ledger

For API infrastructure:

Kong / Envoy + Keycloak + REST/gRPC

For observability:

OpenTelemetry + Prometheus + Grafana

For compliance:

Moov Watchman + custom transaction-risk engine

Commercial vs Open-Source Landscape

The commercial platforms in this category generally provide the difficult operational layer around:

Payment-network connectivity

Certification

Bank integrations

Scheme compliance

Transaction processing

Fraud controls

Operational dashboards

Settlement

Reconciliation

High availability

Disaster recovery

Regulatory requirements

Production support

Open-source projects tend to focus on individual technical layers:

ISO 20022 → Payment APIs → Message Processing → Orchestration → Ledger → Event Streaming → Compliance → Observability

Therefore, the strongest open-source strategy is generally compositional rather than looking for a single "open-source Modern Treasury/Volante/ACI" equivalent.

How to Contribute

Fork the repo.

Add/edit entries in README.md (follow existing format).

Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

Prefer actively maintained projects with public repositories.

Clearly distinguish between fully open-source, open-core, source-available, research software, and commercial products.

Specify supported payment rails such as RTP, FedNow, Fedwire, ACH, SEPA Instant, Faster Payments, PIX, UPI, Visa Direct, or Mastercard Send where applicable.

Include ISO 20022 message families supported by payment projects where known.

Submit PR with a short explanation.

Star the repo if you find it useful!

Disclaimer

This is a community-curated list — not exhaustive and not an endorsement.

Real-time payment processing is highly regulated and generally requires participation agreements, certifications, security controls, and appropriate banking/payment licenses.

Open-source libraries and frameworks listed here are generally components or building blocks rather than certified production payment switches.

Connecting directly to RTP, FedNow, Fedwire, or other payment networks requires appropriate participant/vendor arrangements.

Payment systems require strong controls around authentication, authorization, encryption, fraud detection, sanctions screening, transaction limits, auditability, reconciliation, and operational resilience.

Financial ledgers should use appropriate transactional guarantees and should not depend solely on asynchronous messaging state.

Instant payment systems operate continuously, making high availability, monitoring, disaster recovery, and operational response particularly important.

Always verify the current license, maintenance status, payment-network specifications, and production-readiness of open-source projects before deployment.

Made for banks, fintechs, payment processors, financial institutions, treasury teams, developers, and organizations building modern instant-payment infrastructure.
Let's make real-time payments more programmable, interoperable, transparent, and developer-friendly.
