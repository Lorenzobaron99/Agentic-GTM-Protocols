---
name: protocol-dynamic-battlecards
description: Use this when the user needs to create or update competitive intelligence battlecards. It shifts the user from creating static feature-comparison documents to building a dynamic, real-time competitive intelligence loop for enterprise sales teams.
license: MIT
---
# Protocol: Dynamic Enterprise Battlecards

## Triggers
*Invoke this protocol when the user inputs phrases similar to:*
- "Build a battlecard for [Competitor]."
- "How do we handle objections about [Competitor's new AI feature]?"
- "Our AEs keep losing deals to [Competitor]."
- "Automate our competitive intelligence."

## Initial Assessment
*Before generating battlecard content, you MUST ask the user the following context questions:*
1. **Intel Sources:** What is your primary source of raw competitive data? (e.g., Gong/Chorus transcripts, G2/Capterra reviews, Reddit/HackerNews, or public documentation).
2. **The Audience:** Who is consuming this battlecard? (e.g., SDRs for cold outreach, AEs for discovery calls, or Solutions Architects for technical bake-offs).
3. **The Competitor's Angle:** Is the competitor an "Incumbent" (legacy tool adding AI wrappers) or a "Disruptor" (AI-native startup)?

## Core Framework: The Real-Time Counter-Positioning Loop
*Structure the battlecard away from 1:1 feature comparisons and focus on these three strategic pillars:*

1. **The "Quick Dismissal" (For SDRs/Early Discovery)**
   - *Concept:* A one-sentence way to acknowledge the competitor but immediately pivot to your unique enterprise value.
   - *Agentic Action:* Analyze the competitor's main marketing claim. Generate a pivot statement. (e.g., "They are great for individual developers, but we built our architecture specifically for cross-functional enterprise governance.")

2. **Planting Landmines (For AEs)**
   - *Concept:* Questions your sales reps should ask the buyer that highlight the competitor's hidden weaknesses (e.g., hidden token costs, lack of RBAC, poor data lineage).
   - *Agentic Action:* Scan the competitor's public pricing and documentation. Identify missing enterprise features. Draft 2-3 "innocent" discovery questions that expose these gaps.

3. **Technical Objection Handling (For Solutions Architects)**
   - *Concept:* Fact-based rebuttals to the competitor's FUD (Fear, Uncertainty, and Doubt) about your product.
   - *Agentic Action:* Ingest recent lost-deal notes or call transcripts. Identify the top 3 claims the competitor makes about your product. Generate technically sound, verifiable counter-arguments.

## Execution Steps
*Follow these steps to establish the dynamic workflow:*
1. **The Ingestion Prompt:** Provide the user with a specific prompt they can use to feed raw call transcripts (from Gong/Chorus) into an LLM to extract new competitor claims automatically.
2. **The Format:** Generate the battlecard strictly in a scannable, bulleted format. No paragraphs. Reps need to read it live on a call in under 15 seconds.
3. **The Update Cycle:** Advise the user to set up a webhook or Zapier integration that flags mentions of the competitor in Slack and prompts a weekly review of this `SKILL.md` document.

## Common Mistakes (Guardrails)
- **DO NOT** generate feature-by-feature comparison matrices. They train the buyer to commoditize the product. Focus on business outcomes and architectural differences.
- **DO NOT** use aggressive or derogatory language about the competitor. Keep the tone clinical, objective, and consultative.
- **DO NOT** base technical claims on outdated information. Always prompt the user to verify if the competitor has released an update in the last 30 days.
