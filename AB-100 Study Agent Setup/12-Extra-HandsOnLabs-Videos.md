# Notebook 12 (Extra): Hands-On Labs, Videos & Conference Sessions

## Copilot Studio Agent Setup

**Agent:** AB-100 | Extra: Labs, Videos & Conferences

**System Instructions:**
> "Focus on the key hands-on demonstrations and technical walkthroughs for Copilot Studio, Microsoft Foundry, and multi-agent solutions — covering autonomous agent building, MCP integration, model selection, ALM pipelines, and the latest AI features shown at Microsoft Ignite and Microsoft Build."

**Suggested Topics to create:**
- *Lab Recommender* — trigger: "which lab should I do" — agent asks which exam skill you want to practice and recommends the right lab
- *Video Preview* — trigger: "what does [video name] cover" — agent summarises a video and maps it to exam skills
- *Skill Gap Finder* — trigger: "find my skill gaps" — agent walks through all three exam domains and asks confidence level for each skill

> **Note:** Copilot Studio can ingest YouTube video URLs directly and will use the transcript as a source. Add the YouTube links below directly as sources in your notebook.

---

## Why This Notebook

This notebook is different from the others — it collects all the *demonstrative* content (videos, labs, sample repos) in one place. Use it to:

1. Get audio summaries of video content before watching, to decide what to prioritize
2. Ask Copilot Studio questions about specific demos ("What MCP servers were used in the Mechanics video?")
3. Cross-reference demo content with exam skills to identify gaps

---

## Sources to Add

### Microsoft Mechanics (YouTube — add URL directly)

| Title | URL |
|---|---|
| Build Autonomous Agents: MCP, Models & Multi-Agent | https://www.youtube.com/watch?v=OmJAtDFcSZY |
| Run Local AI on any PC — Microsoft Foundry Local | https://www.youtube.com/watch?v=qL3HADDI6W4 |

### Inside Microsoft Foundry (YouTube — add URLs directly)

| Title | URL |
|---|---|
| Explore the Microsoft Foundry Portal | https://youtu.be/BpOAxKzvrPA |
| Create an AI Agent with File Search | https://youtu.be/dBu3il7db0o |
| Create Agent with Foundry Models | https://youtu.be/fUuTvoDPyzo |
| Deploy and Compare Models | https://youtu.be/zPvEYmj8Mi4 |
| Model Router + GPT-5 Models | https://youtu.be/2NL2XpigH0A |
| Freeform Tool Calling | https://youtu.be/y43sgs-Y8-U |
| Full Inside MF Video Index (GitHub) | https://github.com/Azure-Samples/insideMF |

### Microsoft Learn Shows (add URLs directly)

| Title | URL |
|---|---|
| Mastering Copilot Studio (full series) | https://learn.microsoft.com/en-us/shows/mastering-copilot-studio/ |
| Copilot Studio Agent Academy (video course) | https://learn.microsoft.com/en-us/shows/copilot-studio-agent-academy/ |
| AI Show (Azure AI Foundry) | https://learn.microsoft.com/en-us/shows/ai-show/ |
| Exam Readiness Zone | https://learn.microsoft.com/en-us/shows/exam-readiness-zone/ |

### Power Platform Channel (YouTube)

| Title | URL |
|---|---|
| Copilot Studio Generative Answers | https://www.youtube.com/watch?v=2xZHzbKmyJA |
| Copilot Studio Generative Actions | https://www.youtube.com/watch?v=l-FQXSrboIg |
| Copilot Studio with Azure OpenAI | https://www.youtube.com/watch?v=wFJayIz5Jvc |
| Power Apps Maker Copilot | https://www.youtube.com/watch?v=UwbCIZTx59I |
| Power Automate Copilot | https://www.youtube.com/watch?v=FMz0C6cY1qU |

### Agent Governance & Security Videos (YouTube)

| Title | URL |
|---|---|
| Manage agents used in Copilot Chat | https://youtu.be/jMCn0-ZCHOM |
| Control agents as a Microsoft 365 admin | https://www.youtube.com/watch?v=cQU1GTm14S8 |
| AI and agent data security in Microsoft Purview | https://youtu.be/4BcVWkSTZ3I |

### Conference Sessions (On-Demand)

| Event | URL |
|---|---|
| Microsoft Ignite 2025 — AI Agents Sessions | https://ignite.microsoft.com/en-US/Sessions?filter=topic%2FlogicalValue%3EInnovate+with+Azure+AI+apps+and+agents%09Microsoft+Foundry&onDemand=1 |
| Microsoft Build 2025 — AI, Copilot & Agents | https://build.microsoft.com/en-US/sessions?filter=topic%2FlogicalValue%3EAI%2C+Copilot+%26+Agents |
| AI Tour | https://aitour.microsoft.com |

### Hands-On Lab Sites (add hub URLs as sources)

| Title | URL |
|---|---|
| Microsoft Copilot Studio Labs Hub | https://microsoft.github.io/mcs-labs/ |
| Copilot Studio Agent Academy Hub | https://microsoft.github.io/agent-academy/ |
| Microsoft Copilot Studio Resources Hub | https://microsoft.github.io/agent-resources/copilot-studio/ |
| Microsoft Adoption — Copilot Studio | https://adoption.microsoft.com/en-us/ai-agents/copilot-studio/ |

### GitHub Sample Repos (add README URLs as sources)

| Title | URL |
|---|---|
| microsoft/CopilotStudioSamples | https://github.com/microsoft/CopilotStudioSamples |
| Azure/Copilot-Studio-and-Azure | https://github.com/Azure/Copilot-Studio-and-Azure |
| microsoft/copilot-camp (M365 Copilot extensibility labs) | https://github.com/microsoft/copilot-camp |
| microsoft/agents (M365 Agents SDK) | https://github.com/microsoft/agents |
| microsoft/copilot-alm-starter | https://github.com/microsoft/copilot-alm-starter |

---

## Video-to-Exam-Skill Mapping

| Video | Primary Exam Skill |
|---|---|
| Build Autonomous Agents: MCP, Models & Multi-Agent | Design MCP extensibility; design autonomous agents; multi-agent orchestration |
| Explore the Microsoft Foundry Portal | Propose Foundry Tools; design AI solutions with custom models |
| Create Agent with Foundry Models | Foundry Agent Service; model selection |
| Model Router + GPT-5 Models | Implement model router |
| Manage agents in Copilot Chat | Governance for agents; M365 Copilot agent management |
| Control agents as M365 admin | Design governance for agents |
| AI and agent data security in Purview | Design audit trails; data residency; access controls |
| Copilot Studio Generative Actions | Design tools and actions in Copilot Studio |

---

## Lab-to-Exam-Skill Mapping

| Lab | Primary Exam Skill |
|---|---|
| MCS Labs: Multi-Agent Lab | Design multi-agent orchestration |
| MCS Labs: Pipelines and Source Control | ALM for Copilot Studio agents |
| Agent Academy: MCP Walkthrough | Design MCP extensibility |
| copilot-alm-starter repo | Design ALM process for Copilot Studio |
| Copilot-Studio-and-Azure repo | Integration patterns; monitoring with Application Insights |
