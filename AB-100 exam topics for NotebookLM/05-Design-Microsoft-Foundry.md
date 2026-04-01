# Notebook 5: Design — Microsoft Foundry

## NotebookLM Setup

**Notebook title:** AB-100 | Design: Microsoft Foundry

**Audio Overview Focus Prompt:**
> "Focus on Microsoft Foundry Agent Service capabilities, how to build and evaluate agents in Foundry, the model catalog and how to select models, how the model router works, how to fine-tune custom AI models, and how to design AI solutions using custom models in Microsoft Foundry."

**Suggested audio formats to generate:**
- Standard: Foundry overview — what it is, key capabilities, when to use it
- Extended: Deep dive on model evaluation, fine-tuning, and observability
- Quiz: Test yourself on Foundry tools, model selection, and agent design choices

---

## Exam Skills Covered

From the AB-100 Study Guide — *Design AI-powered business solutions (25–30%)*:

**Design extensibility of AI solutions**
- Design AI solutions by using custom models in Microsoft Foundry
- Propose Foundry Tools for a given requirement
- Propose code-first generative pages and the use of an agent feed for apps
- Determine when custom AI models should be created
- Develop the use cases for customized small language models for the solution
- Implement a model router to intelligently route requests to the most suitable model

From *Deploy AI-powered business solutions (40–45%)*:

**Design the ALM process for AI-powered business solutions**
- Design the ALM process for Microsoft Foundry agents *(see also Notebook 08)*
- Design the ALM process for custom AI models *(see also Notebook 08)*

**Analyze, monitor, and tune AI-powered business solutions**
- Interpret telemetry data for performance and model tuning *(see also Notebook 09)*

**Manage the testing of AI-powered business solutions**
- Create validation criteria of custom AI models *(see also Notebook 09)*

---

## Sources to Add

### Microsoft Learn — Documentation

| Title | URL |
|---|---|
| What Is Microsoft Foundry? | https://learn.microsoft.com/en-us/azure/foundry/what-is-foundry |
| Microsoft Foundry Documentation Hub | https://learn.microsoft.com/en-us/azure/foundry/ |
| Foundry Agent Service Overview | https://learn.microsoft.com/en-us/azure/foundry/agents/overview |
| Foundry Models Overview | https://learn.microsoft.com/en-us/azure/foundry/foundry-models/concepts/models-sold-directly-by-azure |
| Foundry Models from Partners and Community | https://learn.microsoft.com/en-us/azure/foundry/foundry-models/concepts/models-from-partners |
| Run Evaluations in Foundry Portal | https://learn.microsoft.com/en-us/azure/foundry/how-to/evaluate-generative-ai-app |
| Continuous Evaluation of AI Agents | https://learn.microsoft.com/en-us/azure/foundry/how-to/continuous-evaluation-agents |
| Foundry Observability | https://learn.microsoft.com/en-us/azure/foundry/concepts/observability |
| A2A Agent Endpoint in Foundry Agent Service | https://learn.microsoft.com/en-us/azure/ai-foundry/agents/how-to/tools/agent-to-agent?view=foundry |

### Microsoft Learn — Training

| Title | URL |
|---|---|
| Microsoft Foundry Training Hub | https://learn.microsoft.com/en-us/training/azure/ai-foundry |
| Module: Introduction to Azure AI Foundry | https://learn.microsoft.com/en-us/training/modules/introduction-to-azure-ai-studio/ |
| Module: Build a RAG Solution with Foundry | https://learn.microsoft.com/en-us/training/modules/build-copilot-ai-studio/ |
| Module: Fine-Tune a Language Model with Foundry | https://learn.microsoft.com/en-us/training/modules/finetune-model-copilot-ai-studio/ |

### Blogs & Tech Community

| Title | URL |
|---|---|
| Tech Community: Foundry + Copilot Studio Integration | https://techcommunity.microsoft.com/blog/azure-ai-foundry-blog/integrating-azure-ai-foundry-with-copilot-studio-a-strategic-and-technical-overv/4457370 |
| Tech Community: From Prototype to Production with Foundry | https://techcommunity.microsoft.com/blog/azuredevcommunityblog/from-prototype-to-production-building-a-hosted-agent-with-ai-toolkit--microsoft-/4501969 |
| Tech Community: Model Router Cost Optimization | https://techcommunity.microsoft.com/blog/azuredevcommunityblog/optimising-ai-costs-with-microsoft-foundry-model-router/4494776 |
| Build with Foundry, MCP, and Aspire (Dev Blog) | https://developer.microsoft.com/blog/build-a-real-world-example-with-microsoft-agent-framework-microsoft-foundry-mcp-and-aspire |
| Microsoft Foundry Dev Blog | https://devblogs.microsoft.com/foundry/ |

### Videos

| Title | URL |
|---|---|
| AI Show (Azure AI Foundry series) | https://learn.microsoft.com/en-us/shows/ai-show/ |
| Explore the Microsoft Foundry Portal | https://youtu.be/BpOAxKzvrPA |
| Create an AI Agent with File Search | https://youtu.be/dBu3il7db0o |
| Create Agent with Foundry Models | https://youtu.be/fUuTvoDPyzo |
| Deploy and Compare Models | https://youtu.be/zPvEYmj8Mi4 |
| Model Router + GPT-5 Models | https://youtu.be/2NL2XpigH0A |
| Freeform Tool Calling | https://youtu.be/y43sgs-Y8-U |
| Model Mondays Playlist | https://www.youtube.com/watch?v=fjSxraAmGMI&list=PLmsFUfdnGr3wzz6a4E-Szksg92JPng-AL |
| Run Local AI — Microsoft Foundry Local (Mechanics) | https://www.youtube.com/watch?v=qL3HADDI6W4 |
| Full Inside Microsoft Foundry Video Index | https://github.com/Azure-Samples/insideMF |

---

## Key Concepts to Understand

### Foundry vs. Copilot Studio

| Dimension | Microsoft Foundry | Copilot Studio |
|---|---|---|
| Audience | Developers, data scientists | Business users, low-code makers |
| Customization depth | Full code control, fine-tuning, custom evaluators | Configuration-based, Power Automate flows |
| Model flexibility | Any model in catalog + BYOM | Configured models via Foundry connection |
| Agent orchestration | SDK-based (Python/.NET) | Canvas-based, generative orchestration |
| Deployment | Azure-hosted, any channel | Power Platform channels + M365 Copilot |

### Foundry Evaluation Metrics
- **Groundedness:** Does the response accurately reflect the source data?
- **Coherence:** Is the response logically structured?
- **Relevance:** Does the response answer the question asked?
- **Tool call accuracy:** Did the agent call the right tools with correct parameters?
- **Safety:** Does the response avoid harmful content?

### Model Router Modes
| Mode | Behavior |
|---|---|
| **Cost Saving** | Routes to cheapest capable model |
| **Quality** | Routes to highest-performing model |
| **Balanced** | Optimizes cost-quality trade-off |

---

## Exam Tips

- Foundry is the right answer when: the scenario requires fine-tuning, custom evaluators, SDK-level control, or BYOM
- Know what "Foundry Tools" means: code interpreter, file search, Bing grounding, function calling, Azure AI Search
- Continuous evaluation is key for production agents — not just one-time evaluation
- The exam distinguishes between "evaluate" (testing) and "monitor" (production telemetry)
