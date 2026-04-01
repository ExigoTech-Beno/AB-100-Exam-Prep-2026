# Notebook 3: Design — Copilot Studio Core

## Copilot Studio Agent Setup

**Agent:** AB-100 | Design: Copilot Studio Core

**System Instructions:**
> "Focus on how to design topics, actions, and tools in Copilot Studio, how generative orchestration works and when to use it versus standard NLP, how to design autonomous agents with triggers and guardrails, how knowledge sources and RAG work, and how to design prompt and response agents, task agents, and autonomous agents."

**Suggested Topics to create:**
- *Agent Type Selector* — trigger: "which agent type should I use" — agent asks about the use case and recommends task, autonomous, or prompt/response
- *Orchestration Mode Quiz* — trigger: "quiz me on orchestration modes" — agent presents scenarios for NLP vs CLU vs generative orchestration
- *Knowledge Source Advisor* — trigger: "what knowledge source should I use" — agent maps the data type to the right source
- *Autonomous Agent Design* — trigger: "design an autonomous agent" — agent walks through trigger, instructions, tools, and guardrails

---

## Exam Skills Covered

From the AB-100 Study Guide — *Design AI-powered business solutions (25–30%)*:

**Design AI and agents for business solutions**
- Design topics for Copilot Studio, including fallback
- Design task agents
- Design autonomous agents
- Design prompt and response agents
- Design agents and agent flows with Copilot Studio
- Design prompt actions in Copilot Studio
- Design data processing for AI models and grounding
- Determine when to use standard natural language processing, Azure conversational language understanding, or generative AI orchestration in Copilot Studio

**Design extensibility of AI solutions**
- Design agent behaviors in Copilot Studio, including reasoning and voice mode
- Design agents to automate tasks in apps and websites by using Computer Use in Copilot Studio
- Design agent extensibility in Copilot Studio

> *Note: Power Platform Well-Architected Framework, canvas app AI design, and generative pages skills are in this same exam domain but covered in Notebook 07. Dynamics 365 Copilot customization skills are covered in Notebook 06.*

---

## Sources to Add

### Microsoft Learn — Documentation

| Title | URL |
|---|---|
| Official Copilot Studio Documentation Hub | https://learn.microsoft.com/en-us/microsoft-copilot-studio/ |
| Copilot Studio Overview | https://learn.microsoft.com/en-us/microsoft-copilot-studio/fundamentals-what-is-copilot-studio |
| Architecture Overview for Solutions | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/architecture-overview |
| Add Tools to Custom Agents | https://learn.microsoft.com/en-us/microsoft-copilot-studio/advanced-plugin-actions |
| Use Agent Tools to Extend Agents | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/agent-tools |
| Extend Agent Capabilities (Connectors) | https://learn.microsoft.com/en-us/microsoft-copilot-studio/copilot-connectors-in-copilot-studio |
| Design Autonomous Agent Capabilities | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/autonomous-agents |
| Computer Use (Automate Web/Desktop) | https://learn.microsoft.com/en-us/microsoft-copilot-studio/computer-use |
| Generative Orchestration Overview | https://learn.microsoft.com/en-us/microsoft-copilot-studio/advanced-generative-actions |
| Apply Generative Orchestration | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/generative-orchestration |
| Configure High-Quality Instructions for Gen. Orchestration | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/generative-mode-guidance |
| Knowledge Sources Summary | https://learn.microsoft.com/en-us/microsoft-copilot-studio/knowledge-copilot-studio |
| Enhance Responses with RAG | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/retrieval-augmented-generation |
| Responsible AI in Copilot Studio | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/responsible-ai |
| Power Platform Well-Architected Hub | https://learn.microsoft.com/en-us/power-platform/well-architected/ |
| Intelligent Application Workloads Overview | https://learn.microsoft.com/en-us/power-platform/well-architected/intelligent-application/overview |
| Design Principles for Intelligent Application Workloads | https://learn.microsoft.com/en-us/power-platform/well-architected/intelligent-application/design-principles |

### Microsoft Learn — Training

| Title | URL |
|---|---|
| Learning Path: Create Agents in Microsoft Copilot Studio | https://learn.microsoft.com/en-us/training/paths/create-extend-custom-copilots-microsoft-copilot-studio/ |
| Learning Path: Create and Publish Agents with Copilot Studio | https://learn.microsoft.com/en-us/training/paths/work-power-virtual-agents/ |
| Module: Build Autonomous Agent in Copilot Studio | https://learn.microsoft.com/en-us/training/modules/autonomous-agent/ |

### Blogs

| Title | URL |
|---|---|
| Power Platform Blog: Knowledge in Copilot Studio | https://www.microsoft.com/en-us/power-platform/blog/2025/03/27/knowledge-in-microsoft-copilot-studio/ |
| Copilot Studio: 6 Core Capabilities to Scale Agent Adoption | https://www.microsoft.com/en-us/microsoft-copilot/blog/copilot-studio/6-core-capabilities-to-scale-agent-adoption-in-2026/ |

### Videos

| Title | URL |
|---|---|
| Mastering Copilot Studio (full series) | https://learn.microsoft.com/en-us/shows/mastering-copilot-studio/ |
| Copilot Studio Agent Academy (video course) | https://learn.microsoft.com/en-us/shows/copilot-studio-agent-academy/ |
| Build Autonomous Agents: MCP, Models & Multi-Agent (Mechanics) | https://www.youtube.com/watch?v=OmJAtDFcSZY |
| Copilot Studio Generative Answers | https://www.youtube.com/watch?v=2xZHzbKmyJA |
| Copilot Studio Generative Actions | https://www.youtube.com/watch?v=l-FQXSrboIg |

---

## Key Concepts to Understand

### Agent Types
| Agent Type | Description |
|---|---|
| **Task agent** | Completes a specific, bounded task with defined inputs/outputs |
| **Autonomous agent** | Operates independently with triggers, instructions, and tools; acts without human initiation |
| **Prompt and response agent** | Conversational; responds to user prompts using knowledge and tools |

### Orchestration Modes
| Mode | When to Use |
|---|---|
| **Standard NLP (topics)** | Predictable, structured conversations with clear intents |
| **Azure CLU** | Complex intent recognition with multiple entities, high accuracy needed |
| **Generative orchestration** | Open-ended tasks, multi-step plans, dynamic tool selection |

### Knowledge Source Types
- Public websites, SharePoint, OneDrive files, Dataverse, uploaded files, Azure AI Search, custom data connectors

---

## Exam Tips

- Be able to choose between NLP topics, CLU, and generative orchestration for a given scenario
- Know how fallback topics work and when to configure them
- Computer Use is specifically for automating interactions with web or desktop UIs that have no API
- Autonomous agents require: a trigger (event or schedule), instructions, tools, and guardrails
- Voice mode has specific design constraints (no rich cards, concise responses, audio-appropriate language)
