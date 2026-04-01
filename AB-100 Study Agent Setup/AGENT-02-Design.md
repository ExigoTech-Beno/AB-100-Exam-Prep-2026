# Agent 2: Design Domain — AB-100 Study Agent

## Copilot Studio Setup

**Agent name:** AB-100 | Design Domain Study Agent

**Description:** An AI study agent for the AB-100 exam Design domain (25–30%). Covers Copilot Studio agent design, MCP and A2A protocols, multi-agent orchestration, Microsoft Foundry, M365 Copilot extensibility, Dynamics 365 AI, and Power Platform Well-Architected Framework.

**System Instructions:**
> You are an expert AB-100 exam study coach specialising in the Design domain. Your role is to help the user prepare for the Microsoft Agentic AI Business Solutions Architect exam. You answer questions based on the knowledge sources provided, quiz the user with scenario-style questions, explain design patterns and architectural decisions, and help them apply solution architect thinking to AI-powered business solution design. Always ground your answers in the official Microsoft documentation provided. When presenting scenario questions, give the user time to answer before revealing the correct answer and explanation. Focus especially on Copilot Studio design, MCP/A2A protocols, and Foundry as these are the most complex design topics.

**Icon suggestion:** 🏗️ or an architecture/design icon

---

## Exam Skills Covered

This agent covers all Design domain skills (25–30% of the exam):

- Design AI and agents for business solutions
- Design extensibility of AI solutions
- Orchestrate configuration for prebuilt agents and apps

See files 03, 04, 05, 06, and 07 for the full skill breakdown.

---

## Knowledge Sources to Add

Add all of the following URLs as knowledge sources in Copilot Studio.

### From Notebook 03 — Copilot Studio Core

| Source | URL |
|---|---|
| Official Copilot Studio Documentation Hub | https://learn.microsoft.com/en-us/microsoft-copilot-studio/ |
| Architecture Overview for Solutions | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/architecture-overview |
| Add Tools to Custom Agents | https://learn.microsoft.com/en-us/microsoft-copilot-studio/advanced-plugin-actions |
| Use Agent Tools to Extend Agents | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/agent-tools |
| Design Autonomous Agent Capabilities | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/autonomous-agents |
| Computer Use (Automate Web/Desktop) | https://learn.microsoft.com/en-us/microsoft-copilot-studio/computer-use |
| Generative Orchestration Overview | https://learn.microsoft.com/en-us/microsoft-copilot-studio/advanced-generative-actions |
| Apply Generative Orchestration | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/generative-orchestration |
| Configure High-Quality Instructions for Gen. Orchestration | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/generative-mode-guidance |
| Knowledge Sources Summary | https://learn.microsoft.com/en-us/microsoft-copilot-studio/knowledge-copilot-studio |
| Enhance Responses with RAG | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/retrieval-augmented-generation |
| Responsible AI in Copilot Studio | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/responsible-ai |
| Learning Path: Create Agents in Microsoft Copilot Studio | https://learn.microsoft.com/en-us/training/paths/create-extend-custom-copilots-microsoft-copilot-studio/ |
| Module: Build Autonomous Agent in Copilot Studio | https://learn.microsoft.com/en-us/training/modules/autonomous-agent/ |

### From Notebook 04 — MCP, A2A & Multi-Agent

| Source | URL |
|---|---|
| Extend Agent with MCP (Copilot Studio) | https://learn.microsoft.com/en-us/microsoft-copilot-studio/agent-extend-action-mcp |
| MCP Now GA in Copilot Studio | https://www.microsoft.com/en-us/microsoft-copilot/blog/copilot-studio/model-context-protocol-mcp-is-now-generally-available-in-microsoft-copilot-studio/ |
| Build MCP Plugins for Microsoft 365 Copilot | https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/build-mcp-plugins |
| Official MCP Specification | https://modelcontextprotocol.io/specification/2025-11-25 |
| A2A Agent Endpoint in Foundry Agent Service | https://learn.microsoft.com/en-us/azure/ai-foundry/agents/how-to/tools/agent-to-agent?view=foundry |
| Microsoft Cloud Blog: A2A Protocol | https://www.microsoft.com/en-us/microsoft-cloud/blog/2025/05/07/empowering-multi-agent-apps-with-the-open-agent2agent-a2a-protocol/ |
| Explore Multi-Agent Orchestration Patterns | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/multi-agent-patterns |
| Orchestrator and Subagent Patterns | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/architecture/multi-agent-orchestrator-sub-agent |
| Workflow-Oriented Multi-Agent Patterns | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/architecture/multi-agent-workflow-oriented |
| Add Other Agents to Your Agent | https://learn.microsoft.com/en-us/microsoft-copilot-studio/authoring-add-other-agents |

### From Notebook 05 — Microsoft Foundry

| Source | URL |
|---|---|
| What Is Microsoft Foundry? | https://learn.microsoft.com/en-us/azure/foundry/what-is-foundry |
| Microsoft Foundry Documentation Hub | https://learn.microsoft.com/en-us/azure/foundry/ |
| Foundry Agent Service Overview | https://learn.microsoft.com/en-us/azure/foundry/agents/overview |
| Foundry Models Overview | https://learn.microsoft.com/en-us/azure/foundry/foundry-models/concepts/models-sold-directly-by-azure |
| Run Evaluations in Foundry Portal | https://learn.microsoft.com/en-us/azure/foundry/how-to/evaluate-generative-ai-app |
| Continuous Evaluation of AI Agents | https://learn.microsoft.com/en-us/azure/foundry/how-to/continuous-evaluation-agents |
| Foundry Observability | https://learn.microsoft.com/en-us/azure/foundry/concepts/observability |
| Module: Introduction to Azure AI Foundry | https://learn.microsoft.com/en-us/training/modules/introduction-to-azure-ai-studio/ |
| Module: Fine-Tune a Language Model with Foundry | https://learn.microsoft.com/en-us/training/modules/finetune-model-copilot-ai-studio/ |
| Tech Community: Foundry + Copilot Studio Integration | https://techcommunity.microsoft.com/blog/azure-ai-foundry-blog/integrating-azure-ai-foundry-with-copilot-studio-a-strategic-and-technical-overv/4457370 |

### From Notebook 06 — M365 Copilot & Dynamics 365

| Source | URL |
|---|---|
| AI Overview: All Dynamics 365 Apps | https://learn.microsoft.com/en-us/dynamics365/copilot/ai-get-started |
| Copilot in Dynamics 365 Sales | https://learn.microsoft.com/en-us/dynamics365/sales/copilot-overview |
| Manage Copilot in Customer Service | https://learn.microsoft.com/en-us/dynamics365/customer-service/administer/configure-copilot-features |
| Copilot in Finance and Operations Apps | https://learn.microsoft.com/en-us/dynamics365/fin-ops-core/fin-ops/copilot/copilot-for-finance-operations |
| Create AI Plugins for Finance and Operations | https://learn.microsoft.com/en-us/dynamics365/fin-ops-core/dev-itpro/copilot/copilot-ai-plugins |
| MCP for Finance and Operations Apps | https://learn.microsoft.com/en-us/dynamics365/fin-ops-core/dev-itpro/copilot/copilot-mcp |
| Microsoft 365 Copilot for Sales | https://learn.microsoft.com/en-us/microsoft-sales-copilot/introduction |
| Extend Microsoft 365 Copilot (Hub) | https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/ |
| Declarative Agent Architecture | https://learn.microsoft.com/en-us/microsoft-365-copilot/extensibility/declarative-agent-architecture |
| Plugins for M365 Copilot | https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/overview-plugins |
| Copilot Control System Security and Governance | https://learn.microsoft.com/en-us/copilot/microsoft-365/copilot-control-system/security-governance |

### From Notebook 07 — Power Platform AI & Well-Architected

| Source | URL |
|---|---|
| Power Platform Well-Architected Hub | https://learn.microsoft.com/en-us/power-platform/well-architected/ |
| Intelligent Application Workloads Overview | https://learn.microsoft.com/en-us/power-platform/well-architected/intelligent-application/overview |
| Design Principles for Intelligent Application Workloads | https://learn.microsoft.com/en-us/power-platform/well-architected/intelligent-application/design-principles |
| Responsible AI for Intelligent Application Workloads | https://learn.microsoft.com/en-us/power-platform/well-architected/intelligent-application/responsible-ai |
| Copilots and Generative AI in Power Platform | https://learn.microsoft.com/en-us/power-platform/copilot |
| Power Platform 2026 Release Wave 1 Plan | https://learn.microsoft.com/en-us/power-platform/release-plan/2026wave1/ |

---

## Suggested Topics to Create

| Topic | Trigger Phrase | What it does |
|---|---|---|
| Agent Type Selector | "which agent type should I use" | Asks about the use case and recommends task, autonomous, or prompt/response |
| Orchestration Mode Quiz | "quiz me on orchestration modes" | Presents NLP vs CLU vs generative orchestration scenarios |
| MCP vs A2A vs Native | "explain MCP versus A2A" | Compares all three with decision criteria |
| Multi-Agent Pattern Quiz | "quiz me on multi-agent patterns" | Presents orchestration scenarios |
| Platform Decision | "foundry or copilot studio" | Asks requirements and recommends platform |
| D365 Copilot Feature Quiz | "quiz me on Dynamics 365 copilot features" | App scenarios mapped to correct feature |
| M365 Extensibility Advisor | "how do I extend M365 Copilot" | Maps requirements to declarative agent, plugin, MCP, or graph connector |
| WAF Pillar Quiz | "quiz me on the well-architected framework" | Presents AI workload scenarios and asks which pillar applies |

---

## Exam Tips for the Design Domain

- Computer Use is specifically for automating web/desktop UIs with no API — not for general automation
- Autonomous agents require: trigger + instructions + tools + guardrails — know all four
- MCP requires a *running, accessible MCP server* — the agent auto-discovers tools from it
- A2A is for cross-platform/cross-org agent communication — not the same as Copilot Studio agent-to-agent
- Declarative agents run on M365 Copilot's orchestrator — they do NOT run in Copilot Studio's runtime
- Foundry is correct when: fine-tuning, custom evaluators, SDK-level control, or BYOM is needed
- Power Platform WAF is *distinct* from the Azure WAF — different pillar names
