# Notebook 4: Design — MCP, A2A & Multi-Agent Orchestration

## NotebookLM Setup

**Notebook title:** AB-100 | Design: MCP, A2A & Multi-Agent Orchestration

**Audio Overview Focus Prompt:**
> "Focus on how Model Context Protocol (MCP) works and how it is used to extend Copilot Studio agents, how Agent2Agent (A2A) protocol enables cross-platform agent communication, the key multi-agent orchestration patterns (orchestrator-subagent, workflow-oriented), and when to use each pattern."

**Suggested audio formats to generate:**
- Standard: MCP vs. A2A — what each does and when to use each
- Extended: Deep dive on all multi-agent orchestration patterns with design trade-offs
- Debate: MCP connectors vs. native connectors — when is MCP worth it?

---

## Exam Skills Covered

From the AB-100 Study Guide — *Design AI-powered business solutions (25–30%)*:

**Design extensibility of AI solutions**
- Design agent extensibility with Model Context Protocol in Copilot Studio
- Design multi-agent solutions
- Design agents for integration across platforms
- Propose Foundry Tools for a given requirement
- Design agent extensibility in Copilot Studio
- Design extensibility of AI solutions
- Design agents in Microsoft 365 Copilot
- Optimize solution design by using agents in Microsoft 365, including Teams and SharePoint
- Design interoperability of the finance and operations agent chats to use additional knowledge sources

---

## Sources to Add

### Model Context Protocol (MCP)

| Title | URL |
|---|---|
| Extend Agent with MCP (Copilot Studio) | https://learn.microsoft.com/en-us/microsoft-copilot-studio/agent-extend-action-mcp |
| MCP Now GA in Copilot Studio (Announcement) | https://www.microsoft.com/en-us/microsoft-copilot/blog/copilot-studio/model-context-protocol-mcp-is-now-generally-available-in-microsoft-copilot-studio/ |
| Introducing MCP in Copilot Studio (Technical Blog) | https://www.microsoft.com/en-us/microsoft-copilot/blog/copilot-studio/introducing-model-context-protocol-mcp-in-copilot-studio-simplified-integration-with-ai-apps-and-agents/ |
| Build MCP Plugins for Microsoft 365 Copilot | https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/build-mcp-plugins |
| MCP for Finance and Operations Apps | https://learn.microsoft.com/en-us/dynamics365/fin-ops-core/dev-itpro/copilot/copilot-mcp |
| Official MCP Specification | https://modelcontextprotocol.io/specification/2025-11-25 |
| Microsoft MCP Server Catalog (GitHub) | https://github.com/microsoft/mcp |
| Agent Academy: MCP Walkthrough | https://microsoft.github.io/agent-academy/special-ops/mcs-mcp/ |

### Agent2Agent (A2A) Protocol

| Title | URL |
|---|---|
| A2A Agent Endpoint in Foundry Agent Service | https://learn.microsoft.com/en-us/azure/ai-foundry/agents/how-to/tools/agent-to-agent?view=foundry |
| Microsoft Cloud Blog: A2A Protocol | https://www.microsoft.com/en-us/microsoft-cloud/blog/2025/05/07/empowering-multi-agent-apps-with-the-open-agent2agent-a2a-protocol/ |
| A2A Protocol GitHub (Official Spec) | https://github.com/a2aproject/A2A |

### Multi-Agent Orchestration

| Title | URL |
|---|---|
| Explore Multi-Agent Orchestration Patterns | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/multi-agent-patterns |
| Orchestrator and Subagent Patterns | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/architecture/multi-agent-orchestrator-sub-agent |
| Workflow-Oriented Multi-Agent Patterns | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/architecture/multi-agent-workflow-oriented |
| Add Other Agents to Your Agent | https://learn.microsoft.com/en-us/microsoft-copilot-studio/authoring-add-other-agents |
| MVP Blog: Multi-Agent Orchestration Patterns | https://holgerimbery.blog/multi-agent-orchestration |

### Hands-On Labs

| Title | URL |
|---|---|
| Copilot Studio Labs: Multi-Agent Lab | https://microsoft.github.io/mcs-labs/labs/mcs-multi-agent/ |
| MCS Labs: MCP Walkthrough | https://microsoft.github.io/agent-academy/special-ops/mcs-mcp/ |
| GitHub: Azure/Copilot-Studio-and-Azure | https://github.com/Azure/Copilot-Studio-and-Azure |

### Videos

| Title | URL |
|---|---|
| Build Autonomous Agents: MCP, Models & Multi-Agent (Mechanics) | https://www.youtube.com/watch?v=OmJAtDFcSZY |

---

## Key Concepts to Understand

### MCP vs. Native Connectors vs. A2A

| Protocol | Purpose | When to Use |
|---|---|---|
| **MCP** | Expose tools, resources, and prompts from any external system to an AI agent | When integrating with systems that expose an MCP server, or when you want tool auto-discovery without custom connector development |
| **Native Connector** | Pre-built connector to a specific SaaS system | When a certified connector exists and MCP is not needed |
| **A2A** | Agent-to-agent communication across different platforms/organizations | When orchestrating agents that live in different systems (e.g., Foundry agent talking to a Copilot Studio agent) |

### MCP Components
- **Resources:** Data that the MCP server exposes (e.g., documents, database records)
- **Tools:** Actions the agent can take via the MCP server (e.g., create record, run query)
- **Prompts:** Reusable prompt templates provided by the MCP server

### Multi-Agent Patterns
| Pattern | Description |
|---|---|
| **Orchestrator-Subagent** | Primary agent receives request, delegates to specialist subagents, aggregates responses |
| **Workflow-Oriented (Sequential)** | Agents pass outputs to the next agent in a defined chain |
| **Workflow-Oriented (Parallel)** | Multiple agents work simultaneously on different parts of a task |

---

## Exam Tips

- MCP requires a running, accessible MCP server — the agent auto-discovers tools from it
- A2A is for cross-platform/cross-organization agent communication — not the same as Copilot Studio agent-to-agent connections
- Copilot Studio uses its own agent-calling mechanism (add other agents) which works within the platform; A2A is for external agent systems
- Know the trade-offs: orchestrator-subagent adds latency but improves specialization; workflow-oriented is more predictable but less flexible
