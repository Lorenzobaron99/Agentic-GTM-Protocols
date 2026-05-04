---
name: protocol-signal-based-targeting
description: Use this when the user needs to build a go-to-market outbound strategy for an enterprise AI product. It transitions the user from volume-based outreach (TAM) to Account-Based Marketing driven by buying signals (SBM).
license: MIT
---
# Protocol: Enterprise AI Signal-Based Targeting

## Triggers
*Invoke this protocol when the user inputs phrases similar to:*
- "How do we find enterprise buyers for our AI tool?"
- "Help me build a signal-based outbound motion."
- "We are getting ignored by CIOs/CTOs."
- "Automate our lead generation for enterprise."

## Initial Assessment
*Before generating a strategy, you MUST ask the user the following context questions:*
1. **Target Persona:** Who is the ultimate economic buyer? (e.g., VPE, CIO, RevOps, Legal).
2. **Data Tooling:** What data enrichment tools do you currently have API access to? (e.g., Apollo, ZoomInfo, Clearbit, Clay, LinkedIn Sales Navigator).
3. **Core Value Proposition:** Does your AI product drive revenue generation, cost reduction (efficiency), or risk mitigation?

## Core Framework: The Enterprise AI Intent Matrix
*Use this logic to map the user's product value to observable market signals.*

- **IF Value = Cost Reduction / Automation:**
  - *Primary Signal:* Recent layoffs in operational departments, margin compression noted in recent 10-K filings, or hiring freezes for junior roles.
  - *Agentic Action:* Scrape recent earnings call transcripts for keywords like "efficiency," "consolidation," or "doing more with less." Target the CFO/VP of Ops.

- **IF Value = Revenue Generation / Product Velocity:**
  - *Primary Signal:* Spikes in hiring for "AI Engineers," "Machine Learning," or "Data Scientists." Recent announcements of new digital product lines.
  - *Agentic Action:* Monitor GitHub repository creation, tech stack updates (via BuiltWith), and LinkedIn job postings. Target the CTO/VP of Engineering.

- **IF Value = Risk Mitigation / Compliance:**
  - *Primary Signal:* Recent data breaches in their sector, hiring of new CISO, or regulatory changes in their specific industry.
  - *Agentic Action:* Track news APIs for industry compliance updates. Target the CISO/General Counsel.

## Execution Steps
*Follow these steps to build the automated workflow for the user:*

1. **Signal Ingestion:** Define the specific API endpoints or scraping scripts needed to capture the primary signals identified above.
2. **Account Scoring (The 1/0 Rule):** Instruct the user to abandon traditional lead scoring (e.g., "75 points"). In enterprise AI, an account is either "In Market" (1) because a signal fired, or "Out of Market" (0).
3. **Multi-Threading the Committee:** Map the buying committee. For every 1 enterprise account, generate personalized messaging for at least 3 distinct personas (e.g., end-user, technical evaluator, economic buyer).
4. **Triggering the Workflow:** Design a prompt sequence or webhook that takes the raw signal data, passes it to an LLM to draft a personalized email acknowledging the specific signal, and pushes it to the user's sales engagement platform (e.g., Outreach, Salesloft) for human review.

## Common Mistakes (Guardrails)
- **DO NOT** recommend volume-based cold emailing. Enterprise AI buyers will aggressively block domains that spam them with generic AI pitches.
- **DO NOT** treat all signals equally. A company attending a webinar is low intent; a company hiring a "Director of Generative AI" is high intent. Focus only on high-intent data.
- **DO NOT** let the AI send emails autonomously. Always enforce a "Human-in-the-Loop" (HITL) step for enterprise outbound to protect brand reputation.
