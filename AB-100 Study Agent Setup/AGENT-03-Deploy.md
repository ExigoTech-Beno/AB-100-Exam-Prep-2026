# Agent 3: Deploy Domain — AB-100 Study Agent

## Copilot Studio Setup

**Agent name:** AB-100 | Deploy Domain Study Agent

**Description:** An AI study agent for the AB-100 exam Deploy domain (40–45% — the highest-weighted domain). Covers ALM and lifecycle management, monitoring and telemetry, testing strategy, security, responsible AI, governance, and compliance.

**System Instructions:**
> You are an expert AB-100 exam study coach specialising in the Deploy domain, which is the highest-weighted domain on the exam at 40–45%. Your role is to help the user prepare for the Microsoft Agentic AI Business Solutions Architect exam. You answer questions based on the knowledge sources provided, quiz the user with scenario-style questions, and help them apply architect-level thinking to AI solution deployment, monitoring, security, and governance. Always ground your answers in the official Microsoft documentation provided. When presenting scenario questions, give the user time to answer before revealing the correct answer and explanation. Emphasise the Deploy domain's importance and ensure the user can confidently handle ALM, monitoring, security, and responsible AI scenarios.

**Icon suggestion:** 🚀 or a deployment/shield icon

---

## Exam Skills Covered

This agent covers all Deploy domain skills (40–45% of the exam):

- Design the ALM process for AI-powered business solutions
- Analyze, monitor, and tune AI-powered business solutions
- Manage the testing of AI-powered business solutions
- Design responsible AI, security, governance, risk management, and compliance

See files 08, 09, and 10 for the full skill breakdown.

---

## Knowledge Sources to Add

Add all of the following URLs as knowledge sources in Copilot Studio.

### From Notebook 08 — ALM & Lifecycle

| Source | URL |
|---|---|
| Power Platform ALM Hub | https://learn.microsoft.com/en-us/power-platform/alm/ |
| ALM Strategy for Copilot Studio (Official Guidance) | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/alm |
| CAF: Governance and Security for AI Agents | https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/ai-agents/governance-security-across-organization |
| GitHub: microsoft/copilot-alm-starter | https://github.com/microsoft/copilot-alm-starter |
| Copilot Studio Labs: Pipelines and Source Control Lab | https://microsoft.github.io/mcs-labs/labs/pipelines-and-source-control/ |
| Microsoft Foundry Documentation Hub | https://learn.microsoft.com/en-us/azure/foundry/ |
| Run Evaluations in Foundry Portal | https://learn.microsoft.com/en-us/azure/foundry/how-to/evaluate-generative-ai-app |
| Continuous Evaluation of AI Agents | https://learn.microsoft.com/en-us/azure/foundry/how-to/continuous-evaluation-agents |

### From Notebook 09 — Monitoring, Telemetry & Testing

| Source | URL |
|---|---|
| Monitor AI Agents with Application Insights | https://learn.microsoft.com/en-us/azure/azure-monitor/app/agents-view |
| Application Insights OpenTelemetry Overview | https://learn.microsoft.com/en-us/azure/azure-monitor/app/opentelemetry-overview |
| Foundry Observability (Concepts) | https://learn.microsoft.com/en-us/azure/foundry/concepts/observability |
| Run Evaluations in Foundry Portal | https://learn.microsoft.com/en-us/azure/foundry/how-to/evaluate-generative-ai-app |
| Continuous Evaluation of AI Agents | https://learn.microsoft.com/en-us/azure/foundry/how-to/continuous-evaluation-agents |
| Copilot Studio: 6 Core Capabilities to Scale Agent Adoption | https://www.microsoft.com/en-us/microsoft-copilot/blog/copilot-studio/6-core-capabilities-to-scale-agent-adoption-in-2026/ |
| Configure High-Quality Instructions (Generative Orchestration) | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/generative-mode-guidance |

### From Notebook 10 — Security, Responsible AI & Compliance

| Source | URL |
|---|---|
| Microsoft Responsible AI (Main Hub) | https://www.microsoft.com/en-us/ai/responsible-ai |
| Responsible AI Principles and Approach | https://www.microsoft.com/en-us/ai/principles-and-approach |
| What Is Responsible AI (Azure ML Docs) | https://learn.microsoft.com/en-us/azure/machine-learning/concept-responsible-ai?view=azureml-api-2 |
| Module: Embrace Responsible AI Principles and Practices | https://learn.microsoft.com/en-us/training/modules/embrace-responsible-ai-principles-practices/ |
| Module: Introduction to Microsoft's Responsible AI Approach | https://learn.microsoft.com/en-us/training/modules/introduction-to-microsofts-responsible-ai-approach/ |
| Responsible AI in Copilot Studio | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/responsible-ai |
| Microsoft Security Blog: Top 10 Agent Security Risks | https://www.microsoft.com/en-us/security/blog/2026/02/12/copilot-studio-agent-security-top-10-risks-detect-prevent/ |
| Managed Security Enhancements for Copilot Studio | https://www.microsoft.com/en-us/microsoft-copilot/blog/copilot-studio/announcing-managed-security-enhancements-for-microsoft-copilot-studio/ |
| MSRC: How Microsoft Defends Against Prompt Injection | https://www.microsoft.com/en-us/msrc/blog/2025/07/how-microsoft-defends-against-indirect-prompt-injection-attacks |
| Security for Microsoft 365 Copilot | https://learn.microsoft.com/en-us/copilot/microsoft-365/microsoft-365-copilot-ai-security |
| Copilot Control System Security and Governance | https://learn.microsoft.com/en-us/copilot/microsoft-365/copilot-control-system/security-governance |
| CAF: Governance and Security for AI Agents | https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/ai-agents/governance-security-across-organization |
| Azure Data Residency Overview | https://azure.microsoft.com/en-us/explore/global-infrastructure/data-residency |
| Azure Compliance Documentation | https://learn.microsoft.com/en-us/azure/compliance/ |

---

## Suggested Topics to Create

| Topic | Trigger Phrase | What it does |
|---|---|---|
| ALM Component Quiz | "quiz me on ALM" | Presents a component type and asks for the correct ALM approach |
| Environment Strategy Advisor | "design my environment strategy" | Walks through dev, test, production, sandbox considerations |
| Solution Export Checklist | "what is in a copilot studio solution" | Lists what is and isn't included in a solution export |
| Metrics Interpreter | "interpret my agent metrics" | Explains what low resolution rate or poor groundedness scores mean |
| Continuous Improvement Walkthrough | "improve my agent" | Steps through the 7-step improvement loop |
| Responsible AI Quiz | "quiz me on responsible AI" | Presents agent design scenarios and asks which principle is at risk |
| Threat Mitigation Advisor | "identify my agent's security risks" | Walks through the threat taxonomy for the agent's design |
| Data Residency Checklist | "check my data residency compliance" | Runs through the 4-point checklist |
| Audit Trail Designer | "design my audit trail" | Explains what must be logged for models, data, and conversations |

---

## Exam Tips for the Deploy Domain

- **This domain is 40–45% of the exam** — do not underestimate it
- Copilot Studio agents must be in a *managed solution* to deploy between environments
- Know what IS and ISN'T in a solution export: agents, topics, flows, connectors ✓ — environment variables, secrets ✗
- For Foundry: model deployment is separate from agent deployment — each needs its own ALM approach
- Grounding data (SharePoint, Dataverse, AI Search indexes) also needs ALM — not just the agents
- Application Insights has a unified **Agents view** covering Foundry, Copilot Studio, and third-party agents
- Distinguish *monitoring* (production, ongoing) from *evaluation* (pre-production, model quality)
- Know all 6 responsible AI principles by name — these are guaranteed exam points
- Direct vs. indirect (XPIA) prompt injection — know the difference and the mitigations for each
- Audit trails required for BOTH model changes AND data changes
