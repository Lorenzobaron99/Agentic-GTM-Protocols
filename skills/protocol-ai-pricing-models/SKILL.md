---
name: protocol-ai-pricing-models
description: Use this when the user needs to design or restructure a pricing strategy for an enterprise AI product. It helps transition away from legacy per-seat SaaS pricing to hybrid, consumption, or outcome-based models.
license: MIT
---
# Protocol: Enterprise AI Pricing Models

## Triggers
*Invoke this protocol when the user inputs phrases similar to:*
- "How should we price our AI features?"
- "Our inference costs are killing our margins."
- "Should we charge per seat or per token?"
- "Customers want an unlimited plan."

## Initial Assessment
*Before recommending a pricing model, you MUST ask the user the following context questions to understand their unit economics:*
1. **The COGS (Cost of Goods Sold):** Are your inference costs predictable, or highly variable based on user behavior?
2. **The Product Type:** Is your product a "Copilot" (assists a human, needs a seat) or an "Agent" (works autonomously in the background)?
3. **The Value Metric:** What is the atomic unit of value for the customer? (e.g., lines of code written, support tickets resolved, hours saved).

## Core Framework: The AI Monetization Matrix
*Apply one of these three pricing models based on the user's answers:*

1. **The Hybrid Model (Platform Fee + Consumption)**
   - *Best For:* Heavy infrastructure costs and unpredictable usage.
   - *Structure:* Charge a flat annual platform/licensing fee to cover baseline access, integration, and R&D. Charge a variable consumption fee based on "credits" (never expose raw token counts to the buyer).
   - *Agentic Action:* Instruct the user to map token costs to a user-friendly "Credit" system (e.g., 1 Report Generation = 10 Credits).

2. **The Outcome-Based Model (Work-as-a-Service)**
   - *Best For:* Autonomous agents replacing human workflows (e.g., AI SDRs, AI Customer Support).
   - *Structure:* Charge purely based on successful outcomes. (e.g., $1 per resolved ticket, or $500 per qualified meeting booked).
   - *Agentic Action:* Help the user define what constitutes a "successful outcome" and draft the SLA (Service Level Agreement) language to prevent disputes.

3. **Tiered Seats with Usage Caps**
   - *Best For:* Copilots and productivity wrappers where users still need individual logins.
   - *Structure:* Familiar SaaS per-seat pricing (e.g., $30/user/month), but with strict "Fair Use" limits on heavy AI actions to protect compute margins.
   - *Agentic Action:* Define the "overage" paths. What happens when a user hits their limit? (e.g., Drop them to a slower model, or prompt an upsell to a custom Enterprise tier).

## Execution Steps
*Follow these steps to finalize the pricing strategy:*
1. **Margin Calculator:** Ask the user for their average LLM API cost per action. Multiply that by expected monthly usage, and ensure the proposed pricing builds in at least a 70% gross margin.
2. **Draft the Pricing Page:** Generate the copy for the 3-tier pricing page (e.g., Starter, Pro, Enterprise), focusing heavily on the custom nature of the Enterprise tier (custom models, dedicated VPC, volume discounts).
3. **The "Unlimited" Rebuttal:** Draft an internal talking track for sales reps on why the company does not offer "Unlimited AI" (focusing on ensuring quality, speed, and dedicated compute).

## Common Mistakes (Guardrails)
- **DO NOT** recommend exposing raw "token" pricing to non-developer enterprise buyers. It causes cognitive overload. Abstract it into "Tasks," "Queries," or "Credits."
- **DO NOT** recommend a pure per-seat model without usage caps if the product uses expensive foundational models (like GPT-4 or Claude 3.5 Sonnet). Power users will destroy the company's margins.
- **DO NOT** price based on cost-plus alone. AI should be priced on the *value of the problem solved* (e.g., the cost of a human employee doing that same task).
