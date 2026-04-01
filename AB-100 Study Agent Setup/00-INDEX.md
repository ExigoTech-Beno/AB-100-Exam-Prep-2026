# AB-100 Copilot Studio Study System — Master Index

This study system uses **Microsoft Copilot Studio** to build three AI study agents — one per exam domain. Each agent is grounded in the official Microsoft documentation for that domain and can quiz you with scenario-style questions, explain concepts, and help you apply architect-level thinking.

> **Prerequisites:** A Power Platform licence with Copilot Studio access is required to build and use the study agents. See [Copilot Studio licensing](https://learn.microsoft.com/en-us/microsoft-copilot-studio/requirements-licensing).

Go to: **https://copilotstudio.microsoft.com**

---

## The Three Study Agents

| Agent | File | Exam Domain | Weight |
|---|---|---|---|
| AB-100 \| Plan Domain Study Agent | [AGENT-01-Plan.md](AGENT-01-Plan.md) | Plan AI-powered business solutions | 25–30% |
| AB-100 \| Design Domain Study Agent | [AGENT-02-Design.md](AGENT-02-Design.md) | Design AI-powered business solutions | 25–30% |
| **AB-100 \| Deploy Domain Study Agent** | [**AGENT-03-Deploy.md**](AGENT-03-Deploy.md) | **Deploy AI-powered business solutions** | **40–45%** |

> Deploy is the highest-weighted domain. Prioritise Agent 3 if time is short.

---

## How to Set Up Each Agent

1. Open the agent config file (AGENT-01, 02, or 03)
2. In Copilot Studio, create a new agent with the given name and system instructions
3. Add all knowledge sources listed in the file (paste URLs under **Settings → Knowledge**)
4. Create the suggested topics from the file
5. Publish to Microsoft Teams for easy access on any device
6. Use the trigger phrases to start structured study sessions

---

## Topic Reference Files

These files contain the detailed exam skills, key concepts, and exam tips for each topic area. Use them alongside the agent config files to understand the full scope of what each agent covers.

### Plan Domain (Agent 1)

| # | File | Topic |
|---|---|---|
| 01 | [01-Plan-AI-Strategy-CAF.md](01-Plan-AI-Strategy-CAF.md) | AI Strategy, Cloud Adoption Framework, CoE, ROI |
| 02 | [02-Plan-Platform-Selection-Agents.md](02-Plan-Platform-Selection-Agents.md) | Platform Selection, Multi-Agent Strategy, Model Router |
| 11 | [11-Extra-PromptEngineering-LanguageModels.md](11-Extra-PromptEngineering-LanguageModels.md) | Prompt Engineering, Model Selection, SLMs |

### Design Domain (Agent 2)

| # | File | Topic |
|---|---|---|
| 03 | [03-Design-Copilot-Studio-Core.md](03-Design-Copilot-Studio-Core.md) | Copilot Studio Agent Design, Orchestration Modes, RAG |
| 04 | [04-Design-MCP-A2A-MultiAgent.md](04-Design-MCP-A2A-MultiAgent.md) | MCP, A2A Protocol, Multi-Agent Orchestration Patterns |
| 05 | [05-Design-Microsoft-Foundry.md](05-Design-Microsoft-Foundry.md) | Microsoft Foundry, Custom Models, Fine-Tuning, Evaluation |
| 06 | [06-Design-M365-Copilot-Dynamics365.md](06-Design-M365-Copilot-Dynamics365.md) | M365 Copilot Extensibility, Dynamics 365 AI Features |
| 07 | [07-Design-PowerPlatform-WellArchitected.md](07-Design-PowerPlatform-WellArchitected.md) | Power Platform AI, Well-Architected Framework |

### Deploy Domain (Agent 3)

| # | File | Topic |
|---|---|---|
| 08 | [08-Deploy-ALM-Lifecycle.md](08-Deploy-ALM-Lifecycle.md) | ALM, Environment Strategy, Deployment Pipelines |
| 09 | [09-Deploy-Monitoring-Telemetry.md](09-Deploy-Monitoring-Telemetry.md) | Monitoring, Telemetry, Testing Strategy |
| 10 | [10-Deploy-Security-ResponsibleAI-Compliance.md](10-Deploy-Security-ResponsibleAI-Compliance.md) | Security, Responsible AI, Governance, Compliance |

### Cross-Domain Reference

| # | File | Purpose |
|---|---|---|
| 12 | [12-Extra-HandsOnLabs-Videos.md](12-Extra-HandsOnLabs-Videos.md) | Labs, Videos, Conference Sessions |
| 13 | [13-Exam-Strategy.md](13-Exam-Strategy.md) | Exam Strategy, Decision Tables, Scenario Technique |

---

## Exam Domain Weights

| Domain | Weight | Agent |
|---|---|---|
| Plan AI-powered business solutions | 25–30% | Agent 1 |
| Design AI-powered business solutions | 25–30% | Agent 2 |
| **Deploy AI-powered business solutions** | **40–45%** | **Agent 3** |

---

## Recommended Study Order

```
Week 1: Set up Agent 1 → study Plan domain (files 01, 02, 11)
Week 2: Set up Agent 2 → study Design: Copilot Studio + MCP/A2A (files 03, 04)
Week 3: Continue Agent 2 → study Design: Foundry, M365/D365, Power Platform (files 05, 06, 07)
Week 4: Set up Agent 3 → study Deploy domain — most exam weight (files 08, 09, 10)
Week 5: Cross-domain review (files 12, 13) + scenario practice with all 3 agents
Final:  Use trigger phrases in each agent to quiz weak areas
```

---

## Cross-Domain Resources

| Resource | URL |
|---|---|
| AB-100 Official Study Guide | https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/ab-100 |
| Exam Readiness Zone (video series) | https://learn.microsoft.com/en-us/shows/exam-readiness-zone/ |
| Exam Sandbox (practice environment) | https://aka.ms/examdemo |
| Copilot Studio Licensing | https://learn.microsoft.com/en-us/microsoft-copilot-studio/requirements-licensing |
| Copilot Studio Labs Hub | https://microsoft.github.io/mcs-labs/ |
| Copilot Studio Agent Academy Hub | https://microsoft.github.io/agent-academy/ |