# Echosum
_A high-level overview of an internal tooling project developed during my engineering internship for a large technology company._

⚠️ **Important:** The source code for Echosum is proprietary and cannot be shared.  This repo contains a conceptual overview, architectural notes, and examples of my work as the designer and developer of this tool.

### 📑 Project Summary
Echosum is a python-based CLI designed to streamline troubleshooting for large-scale infrastructure automation systems.

It can:
* securely fetch remote automation logs
* parse them into structured tabular data
* identify failure states
* automatically rerun failed tasks
* generate summaries and next steps using LLMs
* send results to Slack for team visibility

The tool was built to support infrastructure and debugging workflows for a production-scale device fleet.

## 🛠️ Technical Highlights
* modular python architecture with ingestion, parsing, formatting, summarization, and notification layers
* custom log parser producing structured `pandas` DataFrames
* CLI built with `Typer`, supporting multiple verosity levels and output types
* automated rerun pipeline for failed hosts
* LLM backend abstraction for multiple providers
* Slack integration with formatted message output
* unit tests built with `pytest` and mocking frameworks

#### 🔧 Tech Stack
* python
* typer (CLI)
* libraries: `pandas`, `paramiko`, `tabulate`
* LLMs: Claude, Gemini
* Slack API
* `pytest`, `pytest-mock`

## ⚡️ What I Owned
* entire end-to-end architecture
* parser implementation
* CLI design and user experience
* LLM prompt system and backend routing
* Slack integration workflow
* documentation and developer onboarding materials

### Why This Project Matters
Echosum turned a slow, manual debugging workflow into a single command that produces structured insights and automated summaries.  it will continue to be used to improve daily workflow efficiency and consistency across team knowledge.
