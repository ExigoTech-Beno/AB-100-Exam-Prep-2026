# Notebook 2: Plan — Platform Selection & Agent Strategy

## NotebookLM Setup

**Notebook title:** AB-100 | Plan: Platform Selection & Agent Strategy

**Audio Overview Focus Prompt:**
> "Focus on the decision criteria for when to use Copilot Studio versus Microsoft Foundry, when to build custom agents versus extending Microsoft 365 Copilot, when custom AI models are needed, how to design a multi-agent solution, and how to develop use cases for prebuilt and customized small language models."

**Suggested audio formats to generate:**
- Standard: Decision framework overview (Copilot Studio vs. Foundry vs. M365 extensibility)
- Extended: Deep dive on multi-agent solution design and SLM use cases
- Debate: Arguments for build vs. buy vs. extend

---

## Exam Skills Covered

From the AB-100 Study Guide — *Plan AI-powered business solutions (25–30%)*:

**Design overall AI strategy for business solutions**
- Design the strategy for building AI and agents in business solutions
- Design a multi-agent solution by using platforms such as Microsoft 365 Copilot, Copilot Studio, and Microsoft Foundry
- Develop the use cases for prebuilt agents in the solution
- Define the solution rules and constraints when building AI components with Copilot Studio, Microsoft Foundry and Foundry Tools
- Determine the use of generative AI and knowledge sources in agents built with Copilot Studio
- Determine when to build custom agents or extend Microsoft 365 Copilot
- Determine when custom AI models should be created
- Develop the use cases for customized small language models (SLMs) for the solution
- Design AI solutions that use multiple Dynamics 365 apps

**Evaluate the costs and benefits of an AI-powered business solution**
- Implement a model router to intelligently route requests to the most suitable model

> *Note: Prompt engineering guidelines and prompt library skills are also Plan-domain skills — see Notebook 11 for full coverage.*

---

## Sources to Add

### Microsoft Learn — Documentation

| Title | URL |
|---|---|
| Copilot Studio Overview | https://learn.microsoft.com/en-us/microsoft-copilot-studio/fundamentals-what-is-copilot-studio |
| What Is Microsoft Foundry? | https://learn.microsoft.com/en-us/azure/foundry/what-is-foundry |
| Foundry Agent Service Overview | https://learn.microsoft.com/en-us/azure/foundry/agents/overview |
| Extend Microsoft 365 Copilot (Hub) | https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/ |
| Declarative Agents Overview | https://learn.microsoft.com/en-us/microsoft-365-copilot/extensibility/overview-declarative-agent |
| Extend M365 Copilot via Copilot Studio | https://learn.microsoft.com/en-us/microsoft-copilot-studio/microsoft-copilot-extend-copilot-extensions |
| AI Overview: All Dynamics 365 Apps | https://learn.microsoft.com/en-us/dynamics365/copilot/ai-get-started |

### Microsoft Learn — Training Modules

| Title | URL |
|---|---|
| Module: Choose a Custom AI Agent Development Path | https://learn.microsoft.com/en-us/training/modules/choose-ai-agent-development-path/ |
| Learning Path: Build Foundation for AI Agents & M365 Copilot | https://learn.microsoft.com/en-us/training/paths/build-foundation-extend-microsoft-365-copilot/ |
| Module: Fine-Tune a Language Model with Foundry | https://learn.microsoft.com/en-us/training/modules/finetune-model-copilot-ai-studio/ |

### Blogs & Comparisons

| Title | URL |
|---|---|
| Inside Track: Copilot Studio vs. Azure AI Foundry? | https://www.microsoft.com/insidetrack/blog/customer-questions-answered-should-i-use-copilot-studio-or-azure-ai-foundry-to-build-my-agent/ |
| Tech Community: Copilot Studio vs. Foundry | https://techcommunity.microsoft.com/blog/azure-ai-foundry-blog/navigating-ai-solutions-microsoft-copilot-studio-vs-azure-ai-foundry/4411678 |
| Tech Community: Foundry + Copilot Studio Integration | https://techcommunity.microsoft.com/blog/azure-ai-foundry-blog/integrating-azure-ai-foundry-with-copilot-studio-a-strategic-and-technical-overv/4457370 |
| Tech Community: Model Router Cost Optimization | https://techcommunity.microsoft.com/blog/azuredevcommunityblog/optimising-ai-costs-with-microsoft-foundry-model-router/4494776 |
| MVP Blog: Choosing Copilot Studio vs. Foundry | https://holgerimbery.blog/which-tool-to-choose |

---

## Decision Framework: Platform Selection

| Scenario | Best Platform |
|---|---|
| Low-code, fast deployment, business users | Copilot Studio |
| Deep code customization, custom models, fine-tuning | Microsoft Foundry |
| Extend existing M365 Copilot experience | M365 Copilot Extensibility (Declarative Agent or Plugin) |
| Enterprise multi-agent orchestration with code control | Foundry Agent Service |
| Citizen developer, Power Platform integration | Copilot Studio |
| Regulated industry, bring-your-own model | Microsoft Foundry |

## Decision Framework: Build vs. Buy vs. Extend

| Scenario | Recommendation |
|---|---|
| Task already covered by a prebuilt agent | Buy / Use prebuilt |
| Need to tailor M365 Copilot with company-specific knowledge | Extend (declarative agent or MCP plugin) |
| Unique business logic not covered by prebuilt | Build custom (Copilot Studio or Foundry) |
| Need domain-specific small language model | Build custom SLM (Foundry fine-tuning) |

---

## Exam Tips

- Understand the specific capabilities of each platform and where they overlap
- Know the exact criteria that would push a solution from Copilot Studio to Foundry
- SLMs (like Phi-4) are used when: domain specificity is critical, latency is important, cost per token must be minimized, or the model runs on-device
- Model router scenarios: cost-saving mode for simple tasks, quality mode for complex reasoning, balanced for mixed workloads
