---
name: protocol-ai-pricing-models
description: Use this when the user needs to design or restructure a pricing strategy for an enterprise AI product. It transitions them from legacy per-seat pricing to outcome-based models by calculating the specific Cost of Intelligence (CoI) to ensure sustainable gross margins.
license: MIT
---
# Protocol: Enterprise AI Pricing & Margin Models

## Triggers
*Invoke this protocol when the user inputs phrases similar to:*
- "How should we price our AI features?"
- "Our token costs and inference overhead are killing our margins."
- "Help me calculate the Cost of Intelligence."
- "Should we charge per seat or per token?"

## Initial Assessment
*Before recommending a pricing model, you MUST ask the user the following context questions to understand their unit economics:*
1. **The Product Type:** Is your product a "Copilot" (assists a human, needs a seat) or an "Agent" (works autonomously in the background)?
2. **Task Complexity (Tokens):** What is the estimated average number of tokens required per successful task resolution?
3. **Model Tier:** What is the cost per 1k tokens of your primary model? (e.g., Flash vs. Pro).
4. **Human Parity Value:** How much does it currently cost a human to perform this exact same task? (e.g., hourly wage / tasks per hour).

## Core Framework 1: The AI Monetization Matrix
*Apply one of these three pricing models based on the user's product type:*

1. **The Hybrid Model (Platform Fee + Consumption)**
   - *Best For:* Heavy infrastructure costs and unpredictable usage.
   - *Structure:* Charge a flat annual platform fee to cover baseline R&D, plus a variable consumption fee based on "credits."
2. **The Outcome-Based Model (Work-as-a-Service)**
   - *Best For:* Autonomous agents replacing human workflows (e.g., AI SDRs).
   - *Structure:* Charge purely based on successful resolutions (e.g., $5 per qualified meeting booked).
3. **Tiered Seats with Usage Caps**
   - *Best For:* Copilots where users still need individual logins.
   - *Structure:* Familiar SaaS per-seat pricing, but with strict "Fair Use" limits to protect compute margins.

## Core Framework 2: The Cost of Intelligence (CoI) Calculator
*Once the model is selected, use the user's variables to calculate their exact pricing:*

1. **Calculate Base Inference Cost:** 
   - *Formula:* `(Tokens / 1000) * Model Cost`
   - *Example:* (2,000 / 1000) * $0.01 = $0.02 base cost per task.
2. **Apply The Efficiency Peg (Outcome-Based):**
   - The pricing of the agent should be pegged at 20-30% of the **Human Parity Value**, NOT just a markup on the inference cost.
   - *Example:* If human parity is $5.00/task, price the AI resolution at $1.00 to $1.50/task.
3. **Verify the Gross Margin:**
   - Ensure the gap between the Base Inference Cost and the final price yields a B2B SaaS margin of >80%. 

## Execution Steps
*Follow these steps to finalize the pricing strategy:*
1. **The Credit System:** Guide the user to abstract raw tokens away from the buyer. Package the pricing into "Resolution Credits" (e.g., 1 successful workflow = 1 Credit).
2. **Margin Optimization (Routing & Caching):** Recommend an architecture where simple user intents are routed to fast, cheap "Flash" models, and complex reasoning is reserved for "Heavy" models. Instruct them to use prompt caching for repetitive enterprise workflows.
3. **Draft the Pricing Page:** Generate the copy for the pricing tiers, ensuring the "Cost of Intelligence" is fully baked into the recurring fees or credit bundles.

## Common Mistakes (Guardrails)
- **DO NOT** expose raw "token" pricing to non-developer enterprise buyers. It causes cognitive overload. Abstract it into "Tasks" or "Credits."
- **DO NOT** price based on cost-plus alone. AI should be priced on the *value of the problem solved* (the Efficiency Peg).
- **DO NOT** recommend a pure per-seat model without usage caps if the product uses expensive foundational models. Power users will destroy the margins.
