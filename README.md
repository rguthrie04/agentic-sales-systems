# Agentic Sales Systems

> Full-stack agentic AI infrastructure for sales and revenue operations — built and deployed in production environments.

This repository documents the agentic AI systems I have designed and deployed across real business environments. All systems are production-built and operational. Code is maintained in private repositories; this document describes architecture, tooling, and outcomes.

---

## Overview

Over the past two years, I have moved from using AI tools to building agentic AI systems — multi-step, autonomous pipelines that handle entire workflows without manual intervention. The work began in a sales and operations context and has expanded into full revenue operations automation.

These are not demos or prototypes. Each system described here is running in a live business environment and has measurably changed how that business operates.

---

## System 1: Full-Stack Customer Acquisition Pipeline

**Context:** Whim Hospitality — corporate and event-based hospitality sales

**What it does:**

A multi-agent pipeline covering the entire customer acquisition journey, from prospect identification through qualified handoff:

1. **Research agent** — ingests a target company or contact and autonomously pulls firmographic data, recent news, relevant signals, and contact information across multiple sources
2. **Personalization agent** — generates context-aware outreach messaging tailored to the specific prospect, industry, and signal data gathered
3. **Sequencing agent** — manages multi-step outreach cadences, adapting follow-up timing and messaging based on engagement signals
4. **CRM enrichment agent** — writes structured data back to the CRM after each interaction, keeping records current without manual entry

**Outcome:** Replaced a fully manual prospecting and outreach process. Sales team now operates at a volume and personalization level that was not achievable by hand.

**Stack:** Python · Anthropic Claude API · Zoho CRM API · REST integrations · custom orchestration layer

---

## System 2: Pipeline Intelligence & Forecasting Agent

**Context:** Active sales pipeline analysis

**What it does:**

A backend agent that runs against live CRM pipeline data and surfaces actionable intelligence for the sales team:

- Analyzes deal velocity, stage duration, and engagement patterns across all open opportunities
- Identifies at-risk deals based on configurable signal thresholds (days since last contact, stalled stages, missing next steps)
- Surfaces prioritized daily action lists by rep, ranked by deal value and close probability
- Generates weekly forecast summaries with confidence intervals based on historical close rates by stage

**Outcome:** Replaced manual pipeline review meetings with an automated intelligence layer that gives reps and leadership a clear picture of what needs attention and why.

**Stack:** Python · Anthropic Claude API · CRM API integration · data aggregation and analysis layer

---

## System 3: Construction Sector Sales Operations (UK)

**Context:** Residential insulation company, England

**What it does:**

Rebuilt the sales operations infrastructure for a field sales team using AI-assisted tooling:

- Automated customer communication workflows for quote follow-up, job scheduling confirmation, and post-job review requests
- AI-assisted lead qualification pipeline that scored and routed inbound leads before human review
- Operational reporting agent that aggregated field team activity and generated weekly performance summaries without manual data entry

**Outcome:** Reduced administrative overhead significantly, improved lead response time, and created consistent customer communication where none had existed previously. The operational transformation led directly to launching an independent consulting practice.

**Stack:** Python · Claude API · CRM workflow automation · REST APIs

---

## Approach

Each system is built with the same underlying design philosophy:

- **Agents over automation** — these systems make decisions, not just execute instructions
- **Production-first** — built to run reliably in live environments, not optimized for demos
- **Business outcomes** — every system is measured against a real operational metric, not a technical benchmark
- **Composable** — agents are designed as modular components that can be recombined for new use cases

---

## Tools & Stack

`Python` `Anthropic Claude API` `Claude Agent SDK` `Salesforce` `HubSpot` `Zoho CRM` `n8n` `REST APIs` `Git`

---

*For questions or collaboration inquiries: ryanguthrie@zoho.com*  
*[LinkedIn](https://www.linkedin.com/in/ryan-guthrie-03357910/)*
