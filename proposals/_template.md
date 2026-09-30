## Development Fund Proposal

**Organization:**  BGC LABS
**Author / Primary Contact:**  Builddude
**Status:** Draft
**Created:** 2026-09-30
**Proposal Type:** RFP-aligned
**RFP / Roadmap Area:** Developer Experience, Tooling & Education
**Champion:** [List Champion](https://github.com/canton-foundation/canton-dev-fund/blob/main/sig-directory.md) **OR** `Needs Champion`
**Total Funding Request:**  900,000 CC
**Project Duration:** 3 MONTHS 
**Label:** wallet-apps

---

## Abstract
**BlockBot is building an AI-powered chatbot development tool that enables over 4.8 billion smartphone users to send, manage, and earn cryptocurrency via WhatsApp.** 

Most crypto products were originally built for crypto-native users, not everyday users. That created an ecosystem where people are expected to understand wallets, seed phrases, gas fees, networks, bridges, and signing transactions before they can even use a product. For mainstream users, that onboarding experience is overwhelming.
Another major challenge is infrastructure maturity. Account abstraction, embedded wallets, gas sponsorshiip, and stablecoin payment infrastructure are only recently becoming mature enough to support web2-like user experiences in web 3.
Most existing solutions also focus heavily on speculation and trading rather than practical day-to-day usability. As a result, the industry spent years optimizing for crypto-native behavior instead of simplifying access for normal users.

We aim to make crypto transactions as intuitive as sending a text message.


---

## Specification

### 1. Objective
**The Problem:**
Developers building Web3 experiences inside messaging platforms like WhatsApp face major barriers, including lack of wallet infrastructure, poor onboarding tools, and little documentation for Layer 2 integration. Meanwhile, competing chains like Solana have tooling such as Solana blinks that enable web2-like integrations. However, builders are increasingly frustrated with closed ecosystems and limited autonomy.

**The Solution:**
Crypto adoption is often hindered by complex wallets and fragmented onboarding experiences. BlockBot wants to eliminate friction by integrating crypto actions within WhatsApp on Canton Network.

We are pioneering:

- A mini-app system embedded into WhatsApp for easy crypto actions.
- A lightweight analytics tool that visualizes real-time crypto activity driven by chat-based UX.
- Open-source developer SDK resources for building WhatsApp-integrated crypto tools on Canton Network.

We aim to use this funding to expand BlockBot’s WhatsApp-integrated, chat-based crypto interface into an open, developer-accessible infrastructure that enables secure, low-friction financial interactions within widely used messaging environments like WhatsApp.
By leveraging BlockBot’s embeddable widget and API framework, we will support interoperable, reproducible integrations that allow other applications and communities to build on top of a shared, open system for messaging-based value transfer.

This approach enhances sustainability by reducing reliance on standalone apps and instead embedding financial tools directly into resilient communication channels already used in restrictive environments. Security and user autonomy are strengthened through blockchain-based transactions, minimizing centralized control over funds and access.

### 2. Implementation Mechanics
BlockBot will use a modular architecture consisting of a WhatsApp interface, AI agent, wallet layer, Canton integration layer, and analytics infrastructure.

**The implementation consists of:**

- WhatsApp Layer: Handles incoming messages, user authentication, commands, and transaction confirmations through the WhatsApp Business API.
- AI Agent Layer: Uses an LLM-based agent to parse natural-language requests into structured actions such as balance checks, transfers, market interactions, and other supported Canton operations.
- Wallet Layer: Manages user wallets, transaction signing, address management, balances, and transaction history while abstracting seed phrases, gas, and network complexity from users.
- Canton Integration Layer: Connects BlockBot to Canton Network through supported APIs/SDKs and handles transaction construction, submission, status tracking, and confirmation.
- Developer SDK/API: Exposes reusable endpoints and components that allow third-party developers to integrate BlockBot's wallet and chat-based transaction capabilities into their own applications.
- Analytics Layer: Indexes onchain activity and application events to track transactions, wallet activity, user interactions, and ecosystem engagement through dashboards.

The core execution flow is:

WhatsApp message → AI intent detection → action validation → wallet/transaction construction → user confirmation → Canton transaction submission → confirmation → analytics/indexing.

The system will use environment-isolated development and testing, automated transaction validation, error handling, logging, monitoring, and security testing before production deployment.

### 3. Architectural Alignment
WhatsApp is a global messaging platform with billions of users, including underserved crypto newcomers. As crypto builders explore Miniapps and chat-based interfaces, Canton’s presence within such mainstream channels is minimal.

BlockBot extends Canton Network's accessibility beyond traditional Web3 interfaces by providing a familiar messaging-based entry point.

The architecture enables:

- Users to access Canton-powered financial applications through WhatsApp.
- Developers to build reusable WhatsApp-native Canton integrations using BlockBot's SDK/API.
- Ecosystem teams to measure user activity and onchain engagement through analytics.
- Applications to embed BlockBot functionality without building wallet and messaging infrastructure from scratch.

By equipping developers with the tools and documentation to build WhatsApp-native Miniapps integrated with Canton Network, and surfacing data that shows which apps are driving onchain engagement

In summary, this creates a strong entry point for Canton Network into everyday messaging platforms and increases real-world utility for its ecosystem.

### 4. Backward Compatibility
**No backward compatibility impact.**

BlockBot will operate as an additional interface and integration layer rather than modifying existing Canton Network infrastructure or applications.

Existing Canton applications and workflows remain unchanged. BlockBot will interact with supported Canton services through standard interfaces/APIs and expose additional functionality through its WhatsApp interface, SDK, and analytics layer.

---

## Milestones and Deliverables

### Milestone 1: Documentation & Mainnet Architecture
* **Estimated Delivery:** Week 1
* **Focus:** Mainnet architecture, technical planning, and developer documentation.
* **Deliverables / Value Metrics:**
  * Mainnet architecture for the Canton Network smart wallet.
  * Technical implementation documentation.
  * Integration and security requirements defined.
  * Architecture ready for Milestone 2 implementation.

### Milestone 2: AI Agent Wallet Functionality
* **Estimated Delivery:** Weeks 2–8
* **Focus:** Canton Network mainnet integration and open-beta launch.
* **Deliverables / Value Metrics:**
  * Canton Network smart wallet integrated with WhatsApp.
  * Users can send and receive transactions on Canton Network mainnet.
  * Users can check wallet balances through chat.
  * Open-beta soft launch with real mainnet transactions.
  * Initial user and transaction activity generated.

### Milestone 3: Feedback, Developer Docs & Analytics

* **Estimated Delivery:** Weeks 9–12
* **Focus:** Production feedback, developer tooling, analytics, and ecosystem activation.
* **Deliverables / Value Metrics:**
  * Incorporate feedback from the AI Agent Wallet open beta.
  * Release and open-source **Developer Documentation V3**.
  * Documentation covering how developers build and interact with Canton Network smart wallet through the Widget SDK/API.
  * Release **Analytics Dashboard**.
  * Track unique chat-based wallet activity on Canton Network.
  * Track engagement with Canton Network miniapps.
  * At least 20 projects/teams integrate BlockBot's widget SDK or API into their application.
  * Launch deposit campaign.
  * **Target: $10,000+ in deposited assets volume.**

---

## Acceptance Criteria
The Tech & Ops Committee will evaluate completion based on:

- BlockBot's chat wallet is operational on the agreed Canton environment and can reliably execute supported wallet actions through WhatsApp.
- Users can create/access their wallet, check balances, and initiate supported transfers through the chat interface without requiring a traditional Web3 wallet UI.
- Transactions are correctly submitted, confirmed, and reflected in the user's wallet state and transaction history.
- The BlockBot developer SDK/API enables developers to integrate supported Canton wallet and chat-based transaction functionality into their own applications.
- Developer documentation is complete, publicly accessible, and sufficient for a developer to set up, integrate, and test the supported BlockBot functionality.
- Analytics can measure chat-wallet activity, transaction activity, and engagement generated through BlockBot.
- Production functionality is tested for reliability, transaction correctness, and appropriate user confirmation/security flows.

### Ecosystem Value

Ecosystem value will be measured through:

- Number of users interacting with Canton through BlockBot.
- Number and volume of onchain transactions executed through the chat wallet.
- Number of developers or applications using the BlockBot SDK/API.
- Feedback and adoption from Canton developers, applications, and ecosystem participants.

---

## Funding

**Total Funding Request:** 900,000 CC

### Payment Breakdown by Milestone
- Milestone 1 _(Documentation & Mainnet Architecture)_: 180,00 CC upon committee acceptance
- Milestone 2 _(AI Agent Wallet Functionality)_: 360,000 CC upon committee acceptance
- Milestone 3 _(Feedback, Developer Docs & Analytics)_: 360,000 CC upon final release and acceptance

### Volatility Stipulation
This project duration is **under 6 months**

---

## Co-Marketing
Upon release, the implementing entity will collaborate with the Foundation on:

- Coordinated announcement of the Canton integration and product releases.
- A technical case study or developer-focused blog explaining the integration.
- Developer documentation and tutorials promoting integration with BlockBot.
- Joint ecosystem promotion through relevant social and developer channels.

---

## Motivation
BlockBot provides Canton Network with an additional distribution and usability layer by allowing users to interact with blockchain-based applications through a familiar messaging environment.

The project targets users who may not be comfortable with conventional Web3 wallets while also giving developers reusable infrastructure for building chat-based Canton applications.

The expected ecosystem impact includes:

- Lowering the barrier to entry for new Canton users.
- Increasing onchain activity through a familiar conversational interface.
- Providing developers with reusable wallet, API, SDK, and integration infrastructure.
- Creating measurable data around user and application activity.
- Expanding the reach of Canton applications into messaging-based user experiences.

By combining the chat wallet, developer tooling, and analytics layer, BlockBot can serve both the user-facing and developer-facing sides of the Canton ecosystem.

---

## Rationale
The Canton integration will use supported Canton interfaces and infrastructure for transaction execution and blockchain interaction, while BlockBot provides the application layer that handles WhatsApp communication, AI-driven intent processing, wallet interaction, and developer access.

This separation allows BlockBot to focus on solving the user-experience and distribution problem without requiring changes to Canton Network's underlying architecture.

The architecture also provides a reusable foundation:

_**WhatsApp → BlockBot AI Agent → Chat Wallet → Canton Network → Analytics**_

This makes the integration applicable beyond a single BlockBot use case. Developers can use the SDK/API to build additional Canton-based applications and workflows on top of the same chat-wallet infrastructure.

The rationale for this approach is therefore to use existing Canton capabilities for the underlying blockchain infrastructure while adding the missing **messaging, wallet abstraction, developer tooling, and analytics layers** needed to make Canton applications accessible through mainstream chat-based experiences.
