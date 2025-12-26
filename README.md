# cleandeedin
Property Title Verification Platform
# CleanDeed 🛡️ 
### *Verify Title Before You Buy.*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Temporal](https://img.shields.io/badge/Orchestration-Temporal-blue)](https://temporal.io)
[![Scraping](https://img.shields.io/badge/Scraping-Browserbase-orange)](https://browserbase.com)

**CleanDeed** is a high-assurance property verification platform designed for the Indian real estate market. We automate the deep due diligence required to ensure a property has a "Clean Title," protecting buyers from fraud, litigation, and regulatory traps.

---

## 🚀 Key Features

- **30-Year EC Audit:** Automated continuity checks across 30 years of Encumbrance Certificates.
- **Deed Authenticity:** Verification of Sale/Gift deeds against official SRO records.
- **Regulatory Check:** Automated validation of HMDA/DTCP approvals and LRS status.
- **Hybrid Workflow:** Seamless human-in-the-loop (HITL) escalation for portal downtimes or CAPTCHA resolution.
- **Risk Scoring:** A comprehensive "Pass/Fail" report with actionable legal recommendations.

## 🛠️ Tech Stack

- **Orchestration:** [Temporal](https://temporal.io) (Durable workflows)
- **Analysis:** [LangGraph](https://langchain-ai.github.io/langgraph/) (Agentic reasoning for legal logic)
- **Database:** MongoDB (Structured NoSQL property documents)
- **OCR:** Azure AI Document Intelligence

## 🏗️ Architecture

CleanDeed follows a modular, agentic architecture to handle the unreliability of government portals:

1. **Document Extraction:** AI-powered OCR extracts data from user-uploaded deeds.
2. **Context-Aware Orchestration:** Temporal manages the lifecycle, retrying flaky APIs and managing wait states.
3. **Validation Logic:** Cross-referencing extracted data with official records to generate a risk report.



## 🚦 Getting Started

### Prerequisites
- Python 3.10+
- [Temporal Server](https://docs.temporal.io/docs/server/quick-install) running locally
- Browserbase API Key

### Installation
1. Clone the repo:
   ```bash
   git clone [https://github.com/CleanDeedIn/cleandeed-backend.git](https://github.com/CleanDeedIn/cleandeed-backend.git)
