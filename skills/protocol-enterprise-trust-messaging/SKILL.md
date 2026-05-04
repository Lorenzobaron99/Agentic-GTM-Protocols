---
name: protocol-enterprise-trust-messaging
description: Use this when the user needs to write product marketing copy, sales collateral, or overcome objections regarding AI data privacy, security, and hallucinations for an enterprise buyer.
license: MIT
---
# Protocol: Enterprise AI Trust Messaging

## Triggers
*Invoke this protocol when the user inputs phrases similar to:*
- "How do we overcome security objections?"
- "The CISO is blocking our deal."
- "Write a one-pager about our AI architecture."
- "They are worried the AI will leak their data or hallucinate."

## Initial Assessment
*Before generating any messaging, you MUST ask the user the following context questions to understand their actual security posture:*
1. **Deployment Model:** Is the AI hosted via SaaS, Single-Tenant VPC, or On-Premises?
2. **Data Retention Policy:** Do you have a strict "Zero Data Retention" agreement with your LLM providers (e.g., OpenAI/Anthropic Enterprise APIs), or do you train your own models on user data?
3. **Compliance Baseline:** Do you have SOC2 Type II, HIPAA, or GDPR certifications?

## Core Framework: The Enterprise Trust Triangle
*Audit all user-provided marketing copy and ensure it addresses the three pillars of Enterprise AI Trust. If it doesn't, rewrite the copy to include them.*

1. **Pillar 1: Data Privacy & Boundaries**
   - *Message:* "Your data is your data. It is never used to train our foundational models."
   - *Agentic Action:* Inject specific mentions of "Zero Data Retention" (ZDR), SOC2 compliance, and end-to-end encryption into the value proposition. 

2. **Pillar 2: Accuracy & Verifiability (Anti-Hallucination)**
   - *Message:* "Deterministic outputs grounded in your enterprise truth."
   - *Agentic Action:* If the product uses RAG (Retrieval-Augmented Generation), explicitly state that the AI cites its sources. Emphasize "Human-in-the-Loop" (HITL) workflows where the AI drafts, but a human approves.

3. **Pillar 3: Governance & Access Control**
   - *Message:* "The AI only sees what the user is allowed to see."
   - *Agentic Action:* Highlight Role-Based Access Control (RBAC), SSO integrations (e.g., Okta, SAML), and comprehensive audit logs showing exactly what the AI touched.

## Execution Steps
*When asked to draft collateral, follow these steps:*
1. **The Trust Audit:** Read the user's draft. Flag any vague AI terms (e.g., "super smart AI," "magic," "autonomous"). 
2. **The Translation:** Replace vague terms with enterprise-grade technical truths (e.g., change "it knows everything about your company" to "it indexes your secure knowledge base via semantic search").
3. **The Pre-emptive FAQ:** Automatically generate a 3-question "Security & Privacy FAQ" at the bottom of any product one-pager or sales email.

## Common Mistakes (Guardrails)
- **DO NOT** ever use absolute terms like "100% hallucination-free" or "perfectly secure." This destroys credibility with technical buyers. Use terms like "high-fidelity," "grounded," and "enterprise-grade."
- **DO NOT** bury the privacy policy. Trust messaging should be front-and-center, acting as a feature, not a footnote.
- **DO NOT** assume the AI is fully autonomous. Always default to messaging that positions the AI as a "copilot" or "co-worker" under strict human supervision unless the user explicitly states otherwise.
