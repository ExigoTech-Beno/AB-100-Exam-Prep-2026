# Notebook 10: Deploy — Security, Responsible AI, Governance & Compliance

## NotebookLM Setup

**Notebook title:** AB-100 | Deploy: Security, Responsible AI & Compliance

**Audio Overview Focus Prompt:**
> "Focus on the six Microsoft responsible AI principles, how to design security and governance for AI agents, how to detect and mitigate prompt injection and other AI-specific vulnerabilities, how to design access controls on grounding data and model tuning, how to validate data residency compliance, and how to design audit trails for changes to models and data."

**Suggested audio formats to generate:**
- Standard: Responsible AI principles and how they apply to agent design
- Extended: Deep dive on agent security threats — prompt injection, XPIA, jailbreaking, and mitigations
- Debate: Governance controls vs. developer agility — where to draw the line
- Quiz: Test yourself on responsible AI principles and security mitigations

---

## Exam Skills Covered

From the AB-100 Study Guide — *Deploy AI-powered business solutions (40–45%)*:

**Design responsible AI, security, governance, risk management, and compliance**
- Design security for agents
- Design governance for agents
- Design model security
- Analyze solution and AI vulnerabilities and mitigations, including prompt manipulation
- Review solution for adherence to responsible AI principles
- Validate data residency and movement compliance
- Design access controls on grounding data and model tuning
- Design audit trails for changes to models and data

---

## Sources to Add

### Responsible AI

| Title | URL |
|---|---|
| Microsoft Responsible AI (Main Hub) | https://www.microsoft.com/en-us/ai/responsible-ai |
| Responsible AI Principles and Approach | https://www.microsoft.com/en-us/ai/principles-and-approach |
| What Is Responsible AI (Azure ML Docs) | https://learn.microsoft.com/en-us/azure/machine-learning/concept-responsible-ai?view=azureml-api-2 |
| Module: Embrace Responsible AI Principles and Practices | https://learn.microsoft.com/en-us/training/modules/embrace-responsible-ai-principles-practices/ |
| Module: Introduction to Microsoft's Responsible AI Approach | https://learn.microsoft.com/en-us/training/modules/introduction-to-microsofts-responsible-ai-approach/ |
| Responsible AI for Intelligent Application Workloads (Power Platform WAF) | https://learn.microsoft.com/en-us/power-platform/well-architected/intelligent-application/responsible-ai |
| Responsible AI in Copilot Studio | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/responsible-ai |

### Security for AI Agents

| Title | URL |
|---|---|
| Microsoft Security Blog: Top 10 Agent Security Risks | https://www.microsoft.com/en-us/security/blog/2026/02/12/copilot-studio-agent-security-top-10-risks-detect-prevent/ |
| Managed Security Enhancements for Copilot Studio | https://www.microsoft.com/en-us/microsoft-copilot/blog/copilot-studio/announcing-managed-security-enhancements-for-microsoft-copilot-studio/ |
| MSRC: How Microsoft Defends Against Prompt Injection | https://www.microsoft.com/en-us/msrc/blog/2025/07/how-microsoft-defends-against-indirect-prompt-injection-attacks |
| Security for Microsoft 365 Copilot | https://learn.microsoft.com/en-us/copilot/microsoft-365/microsoft-365-copilot-ai-security |
| Copilot Control System Security and Governance | https://learn.microsoft.com/en-us/copilot/microsoft-365/copilot-control-system/security-governance |
| CAF: Governance and Security for AI Agents | https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/ai-agents/governance-security-across-organization |

### Data Residency & Compliance

| Title | URL |
|---|---|
| Azure Data Residency Overview | https://azure.microsoft.com/en-us/explore/global-infrastructure/data-residency |
| Azure Compliance Documentation | https://learn.microsoft.com/en-us/azure/compliance/ |
| M365 Copilot In-Country Data Processing | https://www.microsoft.com/en-us/microsoft-365/blog/2025/11/04/microsoft-offers-in-country-data-processing-to-15-countries-to-strengthen-sovereign-controls-for-microsoft-365-copilot/ |

### Videos

| Title | URL |
|---|---|
| AI and agent data security in Microsoft Purview | https://youtu.be/4BcVWkSTZ3I |
| Control agents as a Microsoft 365 admin | https://www.youtube.com/watch?v=cQU1GTm14S8 |

---

## Key Concepts to Understand

### The Six Microsoft Responsible AI Principles

| Principle | What It Means for AI Agents |
|---|---|
| **Fairness** | Agent responses must not discriminate based on protected characteristics |
| **Reliability & Safety** | Agents must behave as designed and fail safely; include fallback and error handling |
| **Privacy & Security** | Protect user data; enforce access controls; prevent data leakage via prompts |
| **Inclusiveness** | Agents should be accessible to all users, including those with disabilities |
| **Transparency** | Users should know they are interacting with an AI; explain agent decisions |
| **Accountability** | Clear ownership of agent behavior; audit trails; human oversight mechanisms |

### AI Security Threat Taxonomy

| Threat | Description | Mitigation |
|---|---|---|
| **Direct prompt injection** | User manipulates the agent via crafted input | Input validation, content filters, system message guardrails |
| **Indirect prompt injection (XPIA)** | Malicious instructions embedded in data the agent reads (web page, document, email) | XPIA protection in Copilot Studio, data source allow-listing |
| **Jailbreaking** | User attempts to bypass safety constraints | Safety system messages, Microsoft content safety filters |
| **Data exfiltration** | Agent tricked into returning sensitive data | Least-privilege data access, output filtering, DLP policies |
| **Model inversion** | Extracting training data from model responses | Differential privacy in fine-tuning, output filtering |
| **Prompt leakage** | System prompt exposed to the user | Never store secrets in system prompts; use environment variables |

### Access Controls for Grounding Data

- Apply **least-privilege** principle: agents only access data they need for their task
- Use **user-delegated access** where possible (agent acts as the user, not a service account)
- Apply **Microsoft Purview sensitivity labels** to restrict which data sources agents can access
- Configure **Azure AI Search security trimming** to ensure search results respect document-level permissions

### Audit Trail Design
- Enable **Copilot Studio conversation logging** for all production agents
- Use **Microsoft Purview audit logs** for M365 Copilot interactions
- Log all **model configuration changes** (system message edits, tool additions) via ALM pipeline history
- Use **Foundry evaluation logs** to track model performance over time
- Maintain **data lineage** for grounding data: source → chunk → retrieval → response

### Data Residency Checklist
- Identify where each grounding data source is stored (region)
- Identify where the model inference occurs (Azure region of Foundry deployment)
- Identify where conversation logs are stored
- Confirm compliance with regional data sovereignty requirements (GDPR, etc.)
- Use **Geo-restricted Azure regions** and **in-country data processing** options where required

---

## Exam Tips

- Know all six responsible AI principles by name and be able to apply them to a scenario
- Prompt injection (both direct and indirect/XPIA) is heavily tested — know the difference and the mitigations for each
- The exam distinguishes between *governance* (policies, controls, oversight) and *security* (technical protections)
- Data residency questions often involve identifying which component in the solution violates a data sovereignty requirement
- Audit trails are required for both model changes AND data changes — not just one or the other
