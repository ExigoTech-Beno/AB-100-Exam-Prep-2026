# Notebook 8: Deploy — ALM & Application Lifecycle Management

## NotebookLM Setup

**Notebook title:** AB-100 | Deploy: ALM & Lifecycle Management

**Audio Overview Focus Prompt:**
> "Focus on the ALM process for Copilot Studio agents, Microsoft Foundry agents, custom AI models, and AI in Dynamics 365 apps — including solution packaging, environment strategy, pipeline deployment, source control, and how to design end-to-end ALM for agentic AI solutions."

**Suggested audio formats to generate:**
- Standard: ALM overview — solutions, pipelines, environments, source control
- Extended: Deep dive on ALM per component type (Copilot Studio vs. Foundry vs. D365)
- Quiz: Test yourself on ALM decisions for different agent component types

---

## Exam Skills Covered

From the AB-100 Study Guide — *Deploy AI-powered business solutions (40–45%)*:

**Design the ALM process for AI-powered business solutions**
- Design the ALM process for data used in AI models and agents
- Design the ALM process for Copilot Studio agents, connectors, and actions
- Design the ALM process for Microsoft Foundry agents
- Design the ALM process for custom AI models
- Design the ALM process for AI in Dynamics 365 apps for finance and supply chain
- Design the ALM process for AI in Dynamics 365 apps for customer experience and service
- Creating a cohesive application lifecycle management (ALM) strategy for agentic-first solutions
- Creating a cohesive environment strategy for AI-powered solutions, with consideration for third-party AI solutions

> *Note: Testing strategy skills (validate prompt best practices, test case strategy, validation criteria) are Deploy-domain skills covered in Notebook 09.*

---

## Sources to Add

### Core ALM Documentation

| Title | URL |
|---|---|
| Power Platform ALM Hub | https://learn.microsoft.com/en-us/power-platform/alm/ |
| ALM Strategy for Copilot Studio (Official Guidance) | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/alm |
| CAF: Governance and Security for AI Agents | https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/ai-agents/governance-security-across-organization |

### GitHub Repos & Labs

| Title | URL |
|---|---|
| GitHub: microsoft/copilot-alm-starter | https://github.com/microsoft/copilot-alm-starter |
| Copilot Studio Labs: Pipelines and Source Control Lab | https://microsoft.github.io/mcs-labs/labs/pipelines-and-source-control/ |
| GitHub: Azure/Copilot-Studio-and-Azure | https://github.com/Azure/Copilot-Studio-and-Azure |
| MCS Labs Setup for Success PDF | https://microsoft.github.io/mcs-labs/assets/pdfs/setup-for-success.pdf |
| MVP Blog: ALM and Environment Strategy | https://holgerimbery.blog/application-lifecycle-managment |

### Foundry ALM

| Title | URL |
|---|---|
| Microsoft Foundry Documentation Hub | https://learn.microsoft.com/en-us/azure/foundry/ |
| Foundry Agent Service Overview | https://learn.microsoft.com/en-us/azure/foundry/agents/overview |

### Testing

| Title | URL |
|---|---|
| Validate Effective Copilot Prompt Best Practices | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/generative-mode-guidance |
| Run Evaluations in Foundry Portal | https://learn.microsoft.com/en-us/azure/foundry/how-to/evaluate-generative-ai-app |
| Continuous Evaluation of AI Agents | https://learn.microsoft.com/en-us/azure/foundry/how-to/continuous-evaluation-agents |

---

## Key Concepts to Understand

### ALM by Component Type

| Component | ALM Approach |
|---|---|
| **Copilot Studio agents** | Package in Power Platform solutions → deploy via Pipelines → source control via GitHub/Azure DevOps |
| **Copilot Studio connectors & actions** | Included in solution packages; custom connectors need independent versioning |
| **Foundry agents** | Deployed via Foundry portal or SDK; use Azure DevOps/GitHub Actions for CI/CD |
| **Custom AI models** | Version via MLflow or Foundry model registry; promote through dev → test → prod |
| **Dynamics 365 AI (F&O)** | Solution packages; AI plugins follow F&O standard ALM (model packages, LCS) |
| **Dynamics 365 AI (CE)** | Power Platform solutions for Copilot customizations; standard ALM pipeline applies |
| **Grounding data** | Data versioning, schema change management, data quality gates in pipeline |

### Environment Strategy
- **Development:** Unmanaged solutions, individual developer environments
- **Test:** Managed solutions, automated testing, integration validation
- **Production:** Managed solutions, locked, monitored
- **Sandbox:** Optional; for user acceptance testing

### Testing Strategy for AI Solutions
- Unit test: Individual topics, actions, and tool calls
- Integration test: Multi-agent flows, end-to-end conversations
- Evaluation test: Model quality metrics (groundedness, relevance, coherence)
- Performance test: Latency, throughput, concurrent users
- Responsible AI test: Safety, fairness, bias detection

---

## Exam Tips

- Copilot Studio agents must be in a *managed solution* to deploy between environments
- Know what is and isn't included in a Copilot Studio solution export (agents, topics, flows, connectors — but not environment variables or secrets)
- For Foundry: model deployment is separate from agent deployment; each needs its own ALM consideration
- Data ALM is often overlooked — grounding data (SharePoint, Dataverse, AI Search indexes) needs versioning and change management too
- The exam may ask you to design an ALM strategy for a *combination* of components — know how they interrelate
