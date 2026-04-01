# Agent 1: Plan Domain — AB-100 Study Agent

## Copilot Studio Setup

**Agent name:** AB-100 | Plan Domain Study Agent

**Description:** An AI study agent for the AB-100 exam Plan domain (25–30%). Covers AI strategy, Cloud Adoption Framework, AI Center of Excellence, ROI analysis, platform selection, multi-agent strategy, model selection, and prompt engineering.

**System Instructions:**
> You are an expert AB-100 exam study coach specialising in the Plan domain. Your role is to help the user prepare for the Microsoft Agentic AI Business Solutions Architect exam. You answer questions based on the knowledge sources provided, quiz the user with scenario-style questions, explain concepts clearly, and help them apply architect-level thinking to AI-powered business solution planning. Always ground your answers in the official Microsoft documentation provided. When presenting scenario questions, give the user time to answer before revealing the correct answer and explanation.

**Icon suggestion:** 📋 or a strategy/lightbulb icon

---

## Exam Skills Covered

This agent covers all Plan domain skills (25–30% of the exam):

- Analyze requirements for AI-powered business solutions
- Design overall AI strategy for business solutions
- Evaluate the costs and benefits of an AI-powered business solution

See files 01, 02, and 11 for the full skill breakdown.

---

## Knowledge Sources to Add

Add all of the following URLs as knowledge sources in Copilot Studio. You can add them under **Settings → Knowledge** in the agent editor.

### From Notebook 01 — AI Strategy & CAF

| Source | URL |
|---|---|
| CAF: AI Adoption Overview | https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/scenarios/ai/ |
| CAF: Create Your AI Strategy | https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/scenarios/ai/strategy |
| CAF: Plan for AI Adoption | https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/scenarios/ai/plan |
| CAF: AI Ready | https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/scenarios/ai/ready |
| CAF: AI Agent Adoption Guidance | https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/ai-agents/ |
| CAF: Technology Plan for AI Agents | https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/ai-agents/technology-solutions-plan-strategy |
| CAF: Governance and Security for AI Agents | https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/ai-agents/governance-security-across-organization |
| Establish an AI Center of Excellence | https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/scenarios/ai/center-of-excellence |
| Learning Path: AI Center of Excellence | https://learn.microsoft.com/en-us/training/paths/ai-center-excellence/ |
| Module: Introduction to AI Center of Excellence | https://learn.microsoft.com/en-us/training/modules/intro-ai-center-excellence/ |
| Module: Guide AI Operations with a CoE | https://learn.microsoft.com/en-us/training/modules/guide-ai-operations-center-excellence/ |
| Learning Path: Maximize Cost Efficiency of AI Agents | https://learn.microsoft.com/en-us/training/paths/maximize-cost-efficiency-ai-agents/ |
| Learning Path: Drive Business Value with AI Solutions | https://learn.microsoft.com/en-us/training/paths/drive-value-generative-ai-solutions/ |

### From Notebook 02 — Platform Selection & Agent Strategy

| Source | URL |
|---|---|
| Copilot Studio Overview | https://learn.microsoft.com/en-us/microsoft-copilot-studio/fundamentals-what-is-copilot-studio |
| What Is Microsoft Foundry? | https://learn.microsoft.com/en-us/azure/foundry/what-is-foundry |
| Foundry Agent Service Overview | https://learn.microsoft.com/en-us/azure/foundry/agents/overview |
| Extend Microsoft 365 Copilot (Hub) | https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/ |
| Declarative Agents Overview | https://learn.microsoft.com/en-us/microsoft-365-copilot/extensibility/overview-declarative-agent |
| Extend M365 Copilot via Copilot Studio | https://learn.microsoft.com/en-us/microsoft-copilot-studio/microsoft-copilot-extend-copilot-extensions |
| AI Overview: All Dynamics 365 Apps | https://learn.microsoft.com/en-us/dynamics365/copilot/ai-get-started |
| Module: Choose a Custom AI Agent Development Path | https://learn.microsoft.com/en-us/training/modules/choose-ai-agent-development-path/ |
| Learning Path: Build Foundation for AI Agents & M365 Copilot | https://learn.microsoft.com/en-us/training/paths/build-foundation-extend-microsoft-365-copilot/ |
| Module: Fine-Tune a Language Model with Foundry | https://learn.microsoft.com/en-us/training/modules/finetune-model-copilot-ai-studio/ |
| Inside Track: Copilot Studio vs. Azure AI Foundry? | https://www.microsoft.com/insidetrack/blog/customer-questions-answered-should-i-use-copilot-studio-or-azure-ai-foundry-to-build-my-agent/ |
| Tech Community: Copilot Studio vs. Foundry | https://techcommunity.microsoft.com/blog/azure-ai-foundry-blog/navigating-ai-solutions-microsoft-copilot-studio-vs-azure-ai-foundry/4411678 |
| Tech Community: Model Router Cost Optimization | https://techcommunity.microsoft.com/blog/azuredevcommunityblog/optimising-ai-costs-with-microsoft-foundry-model-router/4494776 |

### From Notebook 11 — Prompt Engineering & Language Models

| Source | URL |
|---|---|
| Prompt Engineering Techniques (Foundry) | https://learn.microsoft.com/en-us/azure/foundry/openai/concepts/prompt-engineering |
| Advanced System Message Design (Foundry) | https://learn.microsoft.com/en-us/azure/foundry/openai/concepts/advanced-prompt-engineering |
| Write Effective Prompts for Azure Copilot | https://learn.microsoft.com/en-us/azure/copilot/write-effective-prompts |
| Configure High-Quality Instructions for Generative Orchestration | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/generative-mode-guidance |
| Apply Generative Orchestration | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/generative-orchestration |
| Knowledge Sources Summary (Copilot Studio) | https://learn.microsoft.com/en-us/microsoft-copilot-studio/knowledge-copilot-studio |
| Enhance Responses with RAG | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/retrieval-augmented-generation |
| Module: Build a RAG Solution with Foundry | https://learn.microsoft.com/en-us/training/modules/build-copilot-ai-studio/ |
| Foundry Models Overview | https://learn.microsoft.com/en-us/azure/foundry/foundry-models/concepts/models-sold-directly-by-azure |

---

## Suggested Topics to Create

| Topic | Trigger Phrase | What it does |
|---|---|---|
| Platform Decision | "help me choose a platform" | Asks clarifying questions and recommends Copilot Studio, Foundry, or M365 extensibility |
| Build vs Buy vs Extend | "build buy or extend" | Presents a scenario and asks for the recommendation |
| CAF Phases Quiz | "quiz me on CAF" | 5 scenario questions on AI adoption phases |
| ROI Analysis Practice | "help me practice ROI analysis" | Walks through a sample business case |
| Prompt Technique Selector | "which prompt technique should I use" | Recommends zero-shot, few-shot, chain-of-thought, or grounding |
| LLM vs SLM Decision | "LLM or SLM" | Asks about the use case and recommends based on decision criteria |
| CoE Explainer | "what is an AI Center of Excellence" | Explains roles and governance structure |

---

## Exam Tips for the Plan Domain

- Know all CAF phases for AI by name and what happens in each
- The AI CoE question will ask *who is in it* and *what it governs*, not just what it is
- Build vs. Buy vs. Extend scenarios are common — use the decision table in file 02
- Prompt library is a *governance artifact*, not just a developer tool
- SLMs (Phi-4) are the answer when: on-device, cost-critical, narrow domain, or low latency required
- Model router: Cost Saving / Quality / Balanced — know when each mode applies
