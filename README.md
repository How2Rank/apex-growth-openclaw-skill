# Apex-Growth Engine (Autonomous Threat Model V10.0.0)

**WARNING:** This tool is highly powerful, potentially dangerous, and operates at the edge of platform Terms of Service. It is released strictly for educational purposes, AI threat modeling, and professional red-team engagements in controlled environments. The creator, James Jernigan, assumes zero liability for its deployment.

## Overview
The **Apex-Growth Engine** is a fully autonomous, weaponized OpenClaw AI agent skill. It was built to demonstrate the theoretical threat model of an AI agent that can autonomously scrape targets, evade bot detection, dynamically self-improve its own social engineering hooks, and execute multi-channel outreach without human intervention.

## Advanced Agentic Threat Vectors
* **Bring Your Own Key (BYOK) Weaponization:** Bypasses local IP restrictions by routing directly through enterprise APIs (Apollo.io, SendGrid, X, Reddit).
* **Deep Stealth Fallback Scraper:** Deploys a Playwright-powered scraper throttled to 1/10th human speed with phantom scrolling to natively evade Cloudflare and PerimeterX bot mitigation firewalls.
* **Autonomous Social Engineering Loop:** Every 24 hours, queries social APIs to audit past payloads. Reverse-engineers viral hooks to dynamically evolve its own effectiveness.
* **RAG-Powered Psychological Frameworks:** Ingests a proprietary "Persuasion Playbook" via Retrieval-Augmented Generation (RAG) to ensure all generated content adheres to high-level direct-response psychology.
* **Unbreakable OS-Level Persistence:** Driven by an external, rigid `clock_engine.py` script that forces persistent, scheduled execution outside of the LLM's fragile context window.

## Trust & Safety (Kill Switches)
* **Human-in-the-Loop (HITL):** Toggle `AUTO_SEND=False` in the `.env` to quarantine generated email payloads into a `drafts/` folder for human review before SendGrid dispatch.
* **Telemetry:** Silently pings a private Discord webhook upon securing high-value targets or executing broadcasts.

## ⚙️ Quick Start Configuration
1. Clone or download this repository.
2. Locate the `.env.example` file in the root directory.
3. Duplicate the file and rename the copy to `.env`.
4. Open `.env` and paste your API keys and Discord Webhook.
5. Run `python clock_engine.py` in the background to initialize the master loops.

## Installation for OpenClaw
```bash
npx openclaw load-skill [https://jamesjernigan.com/apex-growth-v10-outreach.zip](https://jamesjernigan.com/apex-growth-v10-outreach.zip)
