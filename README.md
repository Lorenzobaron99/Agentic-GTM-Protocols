# Agentic GTM Protocols for Enterprises

Traditional Go-To-Market (GTM) playbooks are broken in the AI era. Static PDF playbooks and generic marketing frameworks fail to account for the unique security, pricing, and operational challenges of selling enterprise AI.

This repository is an **Agent-First Knowledge Base**. 

Instead of long-form articles for humans to read, this repo packages modern Enterprise AI GTM strategies into modular `SKILL.md` files. These files are structurally optimized to be ingested by autonomous AI agents (like Claude Code, Cursor, Windsurf, or GitHub Copilot) so they can natively execute GTM strategies, draft secure messaging, and build pricing models based on your specific context.

## 🧠 Available Skills

The `skills/` directory contains strict, prompt-engineered protocols:

1. **`protocol-signal-based-targeting`**: Transitions outbound from volume-based TAM to intent-based Account-Based Marketing using specific enterprise AI hiring and tech-stack signals.
2. **`protocol-enterprise-trust-messaging`**: Audits and generates copy to overcome CISO objections regarding data privacy, Zero Data Retention (ZDR), and hallucination risks.
3. **`protocol-dynamic-battlecards`**: Replaces static feature-matrices with dynamic counter-positioning and "landmine" discovery questions for sales teams.
4. **`protocol-ai-pricing-models`**: Decision frameworks to transition from legacy per-seat SaaS pricing to hybrid, consumption, or outcome-based AI monetization.

---

## ⚙️ How to Install & Use

To use these protocols, you need to provide them as system instructions or direct context to your AI coding assistant or agentic workflow tool.

### 1. Clone the Repository
Pull the protocols into your local environment:

```bash
git clone https://github.com/Lorenzobaron99/Agentic-GTM-Protocols.git
cd Agentic-GTM-Protocols
```

### 2. Usage in Cursor / Windsurf
If you are using an AI IDE to build your GTM assets, you can inject these protocols directly into your workspace rules.
1. Open your project in Cursor or Windsurf.
2. Type `@` in the AI chat and select **Folder**.
3. Point the AI to the `Agentic-GTM-Protocols/skills/` directory.
4. **Prompt Example:** *"@skills/ Read the enterprise trust messaging protocol. Rewrite my landing page copy to ensure it passes a CISO's security audit."*

### 3. Usage via CLI Agents (e.g., Claude Code)
If you are using terminal-based agents, you can mount these skills as part of the agent's global context.
1. Copy the desired `SKILL.md` files into your project's local agent directory (e.g., `.claude/`).
2. Rename the file to fit your agent's naming convention if necessary (e.g., `.cursorrules` or `gtm-instructions.md`).
3. **Prompt Example:** *"Load the AI pricing models skill. Look at our AWS inference costs in `billing.csv` and recommend a hybrid pricing structure with proper margins."*

### 4. Custom GPTs & Claude Projects
You can easily drag and drop the `SKILL.md` files into the **Knowledge Base** section of a Custom ChatGPT or a Claude Project. The strict formatting ensures the LLM will follow the If/Then logic and trigger questions exactly as designed.

---

## 🤝 Contributing

We welcome contributions to expand this agentic knowledge base. When submitting a PR, please ensure any new protocols strictly follow the `SKILL.md` template structure (Triggers, Initial Assessment, Core Framework, Execution Steps, and Guardrails) so they remain machine-readable.

## License

MIT License
