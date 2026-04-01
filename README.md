# AB-100 Exam Prep — NotebookLM Study System

A structured study system for the **Microsoft AB-100 exam** (*Agentic AI Business Solutions Architect*), built to be used with [Google NotebookLM](https://notebooklm.google.com).

Each file in this repo maps to a NotebookLM notebook — with curated sources, audio overview prompts, key concepts, and exam tips aligned to the [official AB-100 study guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/ab-100).

---

## Exam Domain Coverage

| Domain | Weight | Notebooks |
|---|---|---|
| Plan AI-powered business solutions | 25–30% | 01, 02 |
| Design AI-powered business solutions | 25–30% | 03, 04, 05, 06, 07 |
| **Deploy AI-powered business solutions** | **40–45%** | **08, 09, 10** |

> Deploy is the highest-weighted domain — prioritise notebooks 08–10 if time is short.

---

## Notebooks

| # | File | Topic |
|---|---|---|
| 00 | [00-INDEX.md](AB-100%20exam%20topics%20for%20NotebookLM/00-INDEX.md) | Master index — start here |
| 01 | [01-Plan-AI-Strategy-CAF.md](AB-100%20exam%20topics%20for%20NotebookLM/01-Plan-AI-Strategy-CAF.md) | AI Strategy, Cloud Adoption Framework, CoE, ROI |
| 02 | [02-Plan-Platform-Selection-Agents.md](AB-100%20exam%20topics%20for%20NotebookLM/02-Plan-Platform-Selection-Agents.md) | Platform Selection, Multi-Agent Strategy, Model Router |
| 03 | [03-Design-Copilot-Studio-Core.md](AB-100%20exam%20topics%20for%20NotebookLM/03-Design-Copilot-Studio-Core.md) | Copilot Studio Agent Design, Orchestration Modes, RAG |
| 04 | [04-Design-MCP-A2A-MultiAgent.md](AB-100%20exam%20topics%20for%20NotebookLM/04-Design-MCP-A2A-MultiAgent.md) | MCP, A2A Protocol, Multi-Agent Orchestration Patterns |
| 05 | [05-Design-Microsoft-Foundry.md](AB-100%20exam%20topics%20for%20NotebookLM/05-Design-Microsoft-Foundry.md) | Microsoft Foundry, Custom Models, Fine-Tuning, Evaluation |
| 06 | [06-Design-M365-Copilot-Dynamics365.md](AB-100%20exam%20topics%20for%20NotebookLM/06-Design-M365-Copilot-Dynamics365.md) | M365 Copilot Extensibility, Dynamics 365 AI Features |
| 07 | [07-Design-PowerPlatform-WellArchitected.md](AB-100%20exam%20topics%20for%20NotebookLM/07-Design-PowerPlatform-WellArchitected.md) | Power Platform AI, Well-Architected Framework |
| 08 | [08-Deploy-ALM-Lifecycle.md](AB-100%20exam%20topics%20for%20NotebookLM/08-Deploy-ALM-Lifecycle.md) | ALM, Environment Strategy, Deployment Pipelines |
| 09 | [09-Deploy-Monitoring-Telemetry.md](AB-100%20exam%20topics%20for%20NotebookLM/09-Deploy-Monitoring-Telemetry.md) | Monitoring, Telemetry, Testing Strategy |
| 10 | [10-Deploy-Security-ResponsibleAI-Compliance.md](AB-100%20exam%20topics%20for%20NotebookLM/10-Deploy-Security-ResponsibleAI-Compliance.md) | Security, Responsible AI, Governance, Compliance |
| 11 | [11-Extra-PromptEngineering-LanguageModels.md](AB-100%20exam%20topics%20for%20NotebookLM/11-Extra-PromptEngineering-LanguageModels.md) | Prompt Engineering, Model Selection, SLMs |
| 12 | [12-Extra-HandsOnLabs-Videos.md](AB-100%20exam%20topics%20for%20NotebookLM/12-Extra-HandsOnLabs-Videos.md) | Labs, Videos, Conference Sessions |
| 13 | [13-Exam-Strategy.md](AB-100%20exam%20topics%20for%20NotebookLM/13-Exam-Strategy.md) | Exam Strategy, Decision Tables, Scenario Technique |

---

## How to Use

### Step 1 — Open a notebook file
Each `.md` file contains everything you need to set up one NotebookLM notebook:
- A suggested **notebook title**
- An **Audio Overview focus prompt** (paste into the Customize dialog)
- A table of **sources to add** (Microsoft Learn docs, training modules, blogs, YouTube videos)
- **Key concepts** and comparison tables for active study
- **Exam tips** focused on scenario-style questions

### Step 2 — Create a notebook in NotebookLM
1. Go to [notebooklm.google.com](https://notebooklm.google.com)
2. Create a new notebook with the title from the file
3. Add all sources listed — paste URLs directly (Microsoft Learn, YouTube, GitHub, blogs all work)

### Step 3 — Generate an Audio Overview
1. Click **Customize** in the Audio Overview panel
2. Paste the focus prompt from the file
3. Generate in Standard, Extended, or Quiz format depending on your study goal

### Step 4 — Study actively
- Use the **chat** to quiz yourself with scenario questions
- Ask NotebookLM to compare two options (e.g. "When would I use MCP vs a native connector?")
- Generate **Flashcards** or a **Study Guide** from the Studio panel

### Recommended Study Order

```
Week 1: Notebooks 01 → 02       (Plan domain)
Week 2: Notebooks 03 → 04 → 05  (Design: Copilot Studio, MCP/A2A, Foundry)
Week 3: Notebooks 06 → 07       (Design: M365/D365, Power Platform)
Week 4: Notebooks 08 → 09 → 10  (Deploy domain — highest exam weight)
Week 5: Notebooks 11 → 12 → 13  (Prompt engineering, labs/videos, exam strategy)
Final:  Re-listen to audio overviews for weak areas
```

---

## Resources

| Resource | Link |
|---|---|
| Official AB-100 Study Guide | https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/ab-100 |
| Exam Readiness Zone | https://learn.microsoft.com/en-us/shows/exam-readiness-zone/ |
| Exam Sandbox | https://aka.ms/examdemo |
| Google NotebookLM | https://notebooklm.google.com |
| Copilot Studio Labs | https://microsoft.github.io/mcs-labs/ |
| Copilot Studio Agent Academy | https://microsoft.github.io/agent-academy/ |
