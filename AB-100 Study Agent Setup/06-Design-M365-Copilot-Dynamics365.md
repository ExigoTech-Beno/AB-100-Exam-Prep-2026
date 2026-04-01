# Notebook 6: Design — Microsoft 365 Copilot & Dynamics 365 AI

## Copilot Studio Agent Setup

**Agent:** AB-100 | Design: M365 Copilot & Dynamics 365 AI

**System Instructions:**
> "Focus on the key Copilot and AI features across Dynamics 365 Sales, Customer Service, Finance, Supply Chain, and Contact Center, how to extend Microsoft 365 Copilot using declarative agents and plugins, how to configure Microsoft 365 Copilot for Sales and Copilot for Service, and how to propose prebuilt agents for business scenarios."

**Suggested Topics to create:**
- *D365 Copilot Feature Quiz* — trigger: "quiz me on Dynamics 365 copilot features" — agent presents app scenarios and asks which feature applies
- *M365 Extensibility Advisor* — trigger: "how do I extend M365 Copilot" — agent maps the requirement to declarative agent, plugin, MCP plugin, or graph connector
- *Copilot for Sales vs Service* — trigger: "sales versus service copilot" — agent compares configuration and capabilities
- *F&O Knowledge Sources* — trigger: "finance and operations knowledge sources" — agent explains in-app help and MCP integration

---

## Exam Skills Covered

From the AB-100 Study Guide — *Design AI-powered business solutions (25–30%)*:

**Design AI and agents for business solutions**
- Design business terms for Copilot in Dynamics 365 apps for customer experience and service
- Design customizations of Copilot in Dynamics 365 apps for customer experience and service
- Design connectors for Copilot in Dynamics 365 Sales
- Design agents for integration with Dynamics 365 Contact Center channels

**Design extensibility of AI solutions**
- Design agents in Microsoft 365 Copilot
- Optimize solution design by using agents in Microsoft 365, including Teams and SharePoint

**Orchestrate configuration for prebuilt agents and apps**
- Orchestrate AI features in Dynamics 365 apps for finance and supply chain
- Orchestrate AI features in Dynamics 365 apps for customer experience and service
- Propose Microsoft 365 agents for business scenarios
- Orchestrate the configuration of Microsoft 365 Copilot for Sales and Microsoft 365 Copilot for Service
- Design interoperability of the finance and operations agent chats to use additional knowledge sources
- Recommend the process of adding knowledge sources to in-app help and guidance for Dynamics 365 Finance or Dynamics 365 Supply Chain Management apps

---

## Sources to Add

### Dynamics 365 AI Features

| Title | URL |
|---|---|
| AI Overview: All Dynamics 365 Apps | https://learn.microsoft.com/en-us/dynamics365/copilot/ai-get-started |
| Copilot for Dynamics 365 (Dev Hub) | https://learn.microsoft.com/en-us/microsoft-cloud/dev/copilot/copilot-for-dynamics365 |
| Copilot in Dynamics 365 Sales | https://learn.microsoft.com/en-us/dynamics365/sales/copilot-overview |
| Manage Copilot in Customer Service | https://learn.microsoft.com/en-us/dynamics365/customer-service/administer/configure-copilot-features |
| Copilot in Finance and Operations Apps | https://learn.microsoft.com/en-us/dynamics365/fin-ops-core/fin-ops/copilot/copilot-for-finance-operations |
| Create AI Plugins for Finance and Operations | https://learn.microsoft.com/en-us/dynamics365/fin-ops-core/dev-itpro/copilot/copilot-ai-plugins |
| MCP for Finance and Operations Apps | https://learn.microsoft.com/en-us/dynamics365/fin-ops-core/dev-itpro/copilot/copilot-mcp |
| Microsoft 365 Copilot for Sales | https://learn.microsoft.com/en-us/microsoft-sales-copilot/introduction |
| Dynamics 365 2026 Release Wave 1 Plan | https://learn.microsoft.com/en-us/dynamics365/release-plan/2026wave1/ |

### Microsoft 365 Copilot Extensibility

| Title | URL |
|---|---|
| Extend Microsoft 365 Copilot (Hub) | https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/ |
| Declarative Agents Overview | https://learn.microsoft.com/en-us/microsoft-365-copilot/extensibility/overview-declarative-agent |
| Declarative Agent Architecture | https://learn.microsoft.com/en-us/microsoft-365-copilot/extensibility/declarative-agent-architecture |
| Agents, Actions, Connectors Ecosystem | https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/ecosystem |
| Plugins for M365 Copilot | https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/overview-plugins |
| Build MCP Plugins for Microsoft 365 Copilot | https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/build-mcp-plugins |
| Extend M365 Copilot via Copilot Studio | https://learn.microsoft.com/en-us/microsoft-copilot-studio/microsoft-copilot-extend-copilot-extensions |
| M365 Copilot Extensibility Samples | https://learn.microsoft.com/en-us/microsoft-365-copilot/extensibility/samples |
| Copilot Control System Security and Governance | https://learn.microsoft.com/en-us/copilot/microsoft-365/copilot-control-system/security-governance |

### Training

| Title | URL |
|---|---|
| Learning Path: Build Foundation for AI Agents & M365 Copilot | https://learn.microsoft.com/en-us/training/paths/build-foundation-extend-microsoft-365-copilot/ |

### Videos

| Title | URL |
|---|---|
| Manage agents used in Copilot Chat | https://youtu.be/jMCn0-ZCHOM |
| Control agents as a Microsoft 365 admin | https://www.youtube.com/watch?v=cQU1GTm14S8 |

---

## Key Concepts to Understand

### Copilot Features by Dynamics 365 App

| App | Key Copilot Capabilities |
|---|---|
| **Sales** | Opportunity summaries, lead catch-up, meeting prep, email drafts, news, pipeline insights |
| **Customer Service** | Case summarization, suggested replies, knowledge base answers, email drafts, agent assist |
| **Contact Center** | Real-time transcription, sentiment, agent guidance, post-call summarization |
| **Finance** | Collections AI, financial period close assistant, vendor invoice automation |
| **Supply Chain Management** | Demand forecasting, disruption alerts, replenishment suggestions |

### M365 Copilot Extensibility Options

| Type | Description | Built With |
|---|---|---|
| **Declarative Agent** | Custom scoped Copilot experience with defined knowledge and actions | Copilot Studio or Teams Toolkit |
| **API Plugin** | Connect Copilot to a REST API | OpenAPI spec + manifest |
| **MCP Plugin** | Connect Copilot to an MCP server | MCP server + manifest |
| **Graph Connector** | Index external data into Microsoft Graph for Copilot | Graph Connector SDK |

### M365 Copilot for Sales vs. Copilot for Service
- **Copilot for Sales:** CRM integration (Salesforce or Dynamics 365 Sales), deal insights in Teams meetings, email generation with CRM context
- **Copilot for Service:** Case management integration, knowledge base grounding, omnichannel context in Teams

---

## Exam Tips

- Know which Copilot features can be *configured* vs. which require *custom development*
- Business terms (in Customer Service/Sales) allow you to define organization-specific terminology for Copilot
- Knowledge sources for in-app help in Finance/SCM use the same Copilot Studio knowledge source approach but embedded in the F&O experience
- Declarative agents run on M365 Copilot's orchestrator — they do not run in Copilot Studio's runtime
- Contact Center channels have specific integration patterns — agents connect via Omnichannel for Customer Service
