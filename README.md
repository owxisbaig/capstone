# Financial AI Multi-Agent System (Enterprise Edition)

### Designed & Developed by Group 2 - Owais Baig, Supraj Mudda, Sunil Purswani, Pavan Pratap Reddy Pedaballi, Aditya Parey, Meiqi Hu

---

## 🚀 1. System Summary

The **Financial AI Multi-Agent System** is a modular, production-aligned AI architecture built using the **NANDA agent framework** and **NEST telemetry system**. It demonstrates how enterprise organizations can deploy and orchestrate AI agents to perform structured financial analytics, generate executive-level insights, and maintain full observability across agent interactions.

This platform includes:

* **Financial Advisor Agent** – Performs quantitative stock analysis
* **Report Summarizer Agent** – Converts metrics into decision-ready insights
* **Wizard AI (Prototype)** – Demonstrates cross-domain extensibility

---

## 🧠 2. Architecture Overview

```
User Input → Financial Advisor Agent
            → Metrics, Signals, Trend Detection
            → Telemetry Logged in MongoDB
            → Report Summarizer Agent
            → Executive Narrative Output
```

Supporting Layers:

* **NANDA Adapter & Registry** – Agent lifecycle management
* **MongoDB Telemetry** – Audit logs, session history, structured outputs
* **Configuration Layer** – Agent capabilities, environment variables, ports

---

## 🛠 3. Core Components

### **Financial Advisor Agent**

* Market data ingestion (via yfinance)
* Rolling statistics, volatility, momentum indicators
* Trend and signal detection
* Robust error handling and fallback logic
* Structured JSON output for downstream agents

### **Report Summarizer Agent**

* Consumes Advisor's structured output
* Generates narrative insights for non-technical stakeholders
* Identifies risks, opportunities, and key takeaways
* Produces clean, high-level summaries for decision-makers

### **Wizard AI (Prototype)**

* Lightweight domain-agnostic agent
* Tests system extensibility beyond finance
* Validates capability scaffolding and registration patterns

---

## 🧱 4. Technology Stack

| Layer                      | Technologies                                    |
| -------------------------- | ----------------------------------------------- |
| **Agents & Orchestration** | Python, NANDA Framework, A2A Protocol           |
| **Data Layer**             | yfinance, MongoDB Atlas                         |
| **Infrastructure**         | NEST Adapter, Registry, Capability Config       |
| **Testing**                | End-to-end flow validation, modular agent tests |

---

## ⚙️ 5. Installation & Setup

### Clone the repository

```bash
git clone <repo-url>
cd capstone-main
```

### Create a virtual environment

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### Install dependencies

```bash
pip install -r streamlined-adapter/requirements.txt
```

### Configure environment variables

Update `.env`:

```
MONGODB_URI="your_mongo_connection"
MONGODB_DB="your_database_name"
```

---

## ▶️ 6. Running the System

### Run complete demo

```bash
python demo.py
```

### Run agents individually

```bash
python financial_advisor_agent.py
python report_summarizer_agent.py
```

### Run test suite

```bash
python test_complete_system_local.py
```

---

## 📊 7. Telemetry & Observability

Each agent interaction generates telemetry logs including:

* Input parameters
* Computed financial metrics
* Advisor + Summarizer outputs
* Timestamps & execution context
* Error tracing and system exceptions

This supports:

* Audit compliance
* Reproducibility
* Debugging & monitoring
* Enterprise observability

---

## 🏗️ 8. Enterprise Features

### ✓ Modular Agent Architecture

Each agent is independently deployable and maintainable.

### ✓ Strict Data Contracts

Standardized JSON schemas ensure reliable cross-agent communication.

### ✓ Extensibility

New agents (risk scoring, portfolio optimization, sentiment analysis) can be added with minimal overhead.

### ✓ Telemetry-first Design

All decisions are logged for compliance, analytics, and debugging.

### ✓ Fault-Tolerant Execution

Fallback logic ensures resilience during external API failures.

---

## 👨‍💻 9. Developer Contribution – *Owais Baig*

### Key Contributions

* Built full **Financial Analysis Pipeline** (metrics, indicators, trend detection)
* Designed structured **Advisor Output Schema**
* Engineered **MongoDB Telemetry Integration** end-to-end
* Improved multi-agent workflow (Advisor → Summarizer)
* Implemented robust error-handling and output normalization
* Developed **Wizard AI** prototype to validate multi-domain capability
* Created full testing workflows and validation cases

### Skills Demonstrated

* Multi-agent AI system design
* Data engineering & quantitative analysis
* Distributed workflow orchestration
* Production-grade observability design
* Clean, modular Python engineering

---

## 🚀 10. Roadmap & Future Enhancements

* Portfolio comparison engine
* Real-time dashboards for financial insights
* RL-based risk optimization
* RAG-enhanced financial context retrieval
* Deployment to AWS/GCP for scalable inference
* SLA monitoring for agent uptime and performance

---

## 📄 11. License

This project is for academic and research use under Northeastern University's MPS Analytics program.

---

## 🎯 12. Developers & Contact

1. Owais Baig — baig.o@northeastern.edu
2. Aditya Parey — parey.a@northeastern.edu
3. Supraj Mudda — mudda.s@northeastern.edu
4. Meiqi Hu — hu.meiq@northeastern.edu
5. Sunil Purswani — purswani.su@northeastern.edu
6. Pavan Pratap Reddy Pedaballi — pedaballi.p@northeastern.edu
   
---


