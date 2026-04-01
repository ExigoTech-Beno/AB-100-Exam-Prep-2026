# AB-100 Exam Prep — Copilot Studio Study System

A structured study system for the **Microsoft AB-100 exam** (*Agentic AI Business Solutions Architect*), built entirely on the Microsoft stack using **Microsoft Copilot Studio**.

The system consists of **three AI study agents** — one per exam domain — each grounded in curated Microsoft Learn documentation. Each agent can quiz you with scenario-style questions, explain concepts, compare options, and help you think like an AI solution architect.

> **Prerequisite:** A Power Platform licence with Copilot Studio access is required to build and use the study agents.
> See [Copilot Studio licensing](https://learn.microsoft.com/en-us/microsoft-copilot-studio/requirements-licensing).

---

## The Three Study Agents

| Agent | Config File | Exam Domain | Weight |
|---|---|---|---|
| AB-100 \| Plan Domain Study Agent | [AGENT-01-Plan.md](AB-100%20Study%20Agent%20Setup/AGENT-01-Plan.md) | Plan AI-powered business solutions | 25–30% |
| AB-100 \| Design Domain Study Agent | [AGENT-02-Design.md](AB-100%20Study%20Agent%20Setup/AGENT-02-Design.md) | Design AI-powered business solutions | 25–30% |
| **AB-100 \| Deploy Domain Study Agent** | [**AGENT-03-Deploy.md**](AB-100%20Study%20Agent%20Setup/AGENT-03-Deploy.md) | **Deploy AI-powered business solutions** | **40–45%** |

> Deploy is the highest-weighted domain — prioritise Agent 3 if time is short.

---

## How to Set Up Each Agent

### Step 1 — Open the agent config file
Each `AGENT-0X.md` file contains:
- An **agent name** and **description**
- **System instructions** to paste into the agent editor
- A full list of **knowledge source URLs** to add (Microsoft Learn docs, training modules, blogs)
- A **topics table** with trigger phrases and what each topic does

### Step 2 — Create the agent in Copilot Studio
1. Go to [copilotstudio.microsoft.com](https://copilotstudio.microsoft.com)
2. Create a new agent with the name and description from the config file
3. Paste the system instructions into the agent's **Instructions** field
4. Add all knowledge source URLs under **Settings → Knowledge**

### Step 3 — Create the suggested topics
- Add each topic from the table in the config file
- Set the trigger phrase as listed
- The agent will use generative orchestration to respond using its knowledge sources

### Step 4 — Publish to Teams
- Publish the agent to Microsoft Teams for easy access on any device
- Use the trigger phrases to start structured study sessions

### Step 5 — Study actively
- Type a trigger phrase to start a structured topic (e.g. *"quiz me on CAF"*)
- Ask freeform questions (e.g. *"When would I use MCP vs a native connector?"*)
- Request scenario practice (e.g. *"Give me an exam scenario question"*)

---

## Topic Reference Files

These 13 files contain detailed exam skills, key concepts, and exam tips per topic area. Use them as reference while building and using the agents.

### Plan Domain → Agent 1

| # | File | Topic |
|---|---|---|
| 01 | [01-Plan-AI-Strategy-CAF.md](AB-100%20Study%20Agent%20Setup/01-Plan-AI-Strategy-CAF.md) | AI Strategy, Cloud Adoption Framework, CoE, ROI |
| 02 | [02-Plan-Platform-Selection-Agents.md](AB-100%20Study%20Agent%20Setup/02-Plan-Platform-Selection-Agents.md) | Platform Selection, Multi-Agent Strategy, Model Router |
| 11 | [11-Extra-PromptEngineering-LanguageModels.md](AB-100%20Study%20Agent%20Setup/11-Extra-PromptEngineering-LanguageModels.md) | Prompt Engineering, Model Selection, SLMs |

### Design Domain → Agent 2

| # | File | Topic |
|---|---|---|
| 03 | [03-Design-Copilot-Studio-Core.md](AB-100%20Study%20Agent%20Setup/03-Design-Copilot-Studio-Core.md) | Copilot Studio Agent Design, Orchestration Modes, RAG |
| 04 | [04-Design-MCP-A2A-MultiAgent.md](AB-100%20Study%20Agent%20Setup/04-Design-MCP-A2A-MultiAgent.md) | MCP, A2A Protocol, Multi-Agent Orchestration Patterns |
| 05 | [05-Design-Microsoft-Foundry.md](AB-100%20Study%20Agent%20Setup/05-Design-Microsoft-Foundry.md) | Microsoft Foundry, Custom Models, Fine-Tuning, Evaluation |
| 06 | [06-Design-M365-Copilot-Dynamics365.md](AB-100%20Study%20Agent%20Setup/06-Design-M365-Copilot-Dynamics365.md) | M365 Copilot Extensibility, Dynamics 365 AI Features |
| 07 | [07-Design-PowerPlatform-WellArchitected.md](AB-100%20Study%20Agent%20Setup/07-Design-PowerPlatform-WellArchitected.md) | Power Platform AI, Well-Architected Framework |

### Deploy Domain → Agent 3

| # | File | Topic |
|---|---|---|
| 08 | [08-Deploy-ALM-Lifecycle.md](AB-100%20Study%20Agent%20Setup/08-Deploy-ALM-Lifecycle.md) | ALM, Environment Strategy, Deployment Pipelines |
| 09 | [09-Deploy-Monitoring-Telemetry.md](AB-100%20Study%20Agent%20Setup/09-Deploy-Monitoring-Telemetry.md) | Monitoring, Telemetry, Testing Strategy |
| 10 | [10-Deploy-Security-ResponsibleAI-Compliance.md](AB-100%20Study%20Agent%20Setup/10-Deploy-Security-ResponsibleAI-Compliance.md) | Security, Responsible AI, Governance, Compliance |

### Cross-Domain Reference

| # | File | Purpose |
|---|---|---|
| 12 | [12-Extra-HandsOnLabs-Videos.md](AB-100%20Study%20Agent%20Setup/12-Extra-HandsOnLabs-Videos.md) | Labs, Videos, Conference Sessions |
| 13 | [13-Exam-Strategy.md](AB-100%20Study%20Agent%20Setup/13-Exam-Strategy.md) | Exam Strategy, Decision Tables, Scenario Technique |

---

## Recommended Study Order

```
Week 1: Build Agent 1 → study Plan domain (files 01, 02, 11)
Week 2: Build Agent 2 → study Design: Copilot Studio + MCP/A2A (files 03, 04)
Week 3: Continue Agent 2 → study Design: Foundry, M365/D365, Power Platform (files 05, 06, 07)
Week 4: Build Agent 3 → study Deploy domain — most exam weight (files 08, 09, 10)
Week 5: Cross-domain review (files 12, 13) + scenario practice with all 3 agents
Final:  Use trigger phrases in each agent to quiz weak areas
```

---

## Resources

| Resource | Link |
|---|---|
| Official AB-100 Study Guide | https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/ab-100 |
| Copilot Studio | https://copilotstudio.microsoft.com |
| Copilot Studio Licensing | https://learn.microsoft.com/en-us/microsoft-copilot-studio/requirements-licensing |
| Exam Readiness Zone | https://learn.microsoft.com/en-us/shows/exam-readiness-zone/ |
| Exam Sandbox | https://aka.ms/examdemo |
| Copilot Studio Labs | https://microsoft.github.io/mcs-labs/ |
| Copilot Studio Agent Academy | https://microsoft.github.io/agent-academy/ |
