# Notebook 13 (Extra): Exam Strategy & Readiness

## Copilot Studio Agent Setup

**Agent:** AB-100 | Extra: Exam Strategy & Readiness

**System Instructions:**
> "Focus on strategies for approaching the AB-100 exam, how to read and interpret scenario-based questions, key comparison frameworks for platform selection and design decisions, the most commonly tested concepts across all three exam domains, and how to eliminate wrong answers by applying architect-level thinking to AI-powered business solution scenarios."

**Suggested audio formats to generate:**
- Standard: Overview of exam structure and scenario-question technique
- Brief: Quick-fire review of the most exam-relevant decision frameworks
- Quiz: Test yourself on scenario questions across all three domains

---

## Exam Overview

| Attribute | Detail |
|---|---|
| **Exam code** | AB-100 |
| **Full name** | Microsoft Certified: Agentic AI Business Solutions Architect |
| **Passing score** | 700 / 1000 |
| **Domains** | Plan (25–30%) · Design (25–30%) · **Deploy (40–45%)** |
| **Official study guide** | https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/ab-100 |
| **Exam sandbox** | https://aka.ms/examdemo |
| **Exam Readiness Zone** | https://learn.microsoft.com/en-us/shows/exam-readiness-zone/ |

---

## Sources to Add

### Official Resources

| Title | URL |
|---|---|
| AB-100 Study Guide (Official) | https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/ab-100 |
| Exam Readiness Zone | https://learn.microsoft.com/en-us/shows/exam-readiness-zone/ |
| Exam Sandbox (practice environment) | https://aka.ms/examdemo |
| Certification: Agentic AI Business Solutions Architect | https://learn.microsoft.com/en-us/credentials/certifications/agentic-ai-business-solutions-architect/ |

### Community & Practice

| Title | URL |
|---|---|
| Microsoft Q&A | https://learn.microsoft.com/en-us/answers/products/ |
| Microsoft Tech Community | https://techcommunity.microsoft.com |
| Microsoft MVP Community Hub | https://techcommunity.microsoft.com/category/mvp |

---

## How to Approach Scenario Questions

Most AB-100 questions follow this pattern:
> *A company needs to [business goal]. They have [constraints]. Which approach/tool/design should the architect recommend?*

**Step-by-step technique:**
1. **Identify the constraint** — is it cost, code level, platform, regulation, or timeline?
2. **Identify the actor** — business user, developer, or admin?
3. **Match the constraint to a decision framework** (see tables below)
4. **Eliminate clearly wrong answers** — usually one answer is the wrong platform tier, one is over-engineered, one is correct
5. **When two answers seem right**, pick the one that uses the *least privilege / lowest complexity* approach that still meets the requirement

---

## Master Decision Framework Tables

### Platform Selection

| Scenario Signal | Best Platform |
|---|---|
| Business user, low-code, fast deployment | Copilot Studio |
| Developer, fine-tuning, custom models, SDK control | Microsoft Foundry |
| Extend existing M365 Copilot with company knowledge | M365 Copilot Extensibility (Declarative Agent) |
| Enterprise multi-agent orchestration with code | Foundry Agent Service |
| Citizen developer + Power Platform integration | Copilot Studio |
| Regulated industry, BYOM, on-premises data | Microsoft Foundry |

### Build vs. Buy vs. Extend

| Scenario Signal | Recommendation |
|---|---|
| Task already handled by a prebuilt agent | Buy / Use prebuilt |
| Tailor M365 Copilot with org-specific knowledge | Extend (Declarative Agent or MCP Plugin) |
| Unique business logic not covered by prebuilt | Build custom (Copilot Studio or Foundry) |
| Domain-specific language model needed | Build SLM (Foundry fine-tuning) |

### Agent Type Selection

| Need | Agent Type |
|---|---|
| Bounded task with defined inputs/outputs | Task agent |
| Operates independently, triggered by event or schedule | Autonomous agent |
| Conversational, responds to user prompts | Prompt and response agent |

### Orchestration Mode (Copilot Studio)

| Scenario | Mode |
|---|---|
| Predictable, structured intents | Standard NLP (topics) |
| Complex multi-entity intent recognition | Azure CLU |
| Open-ended tasks, dynamic tool selection | Generative orchestration |

### MCP vs. Native Connector vs. A2A

| Need | Protocol |
|---|---|
| Tool auto-discovery from an external system | MCP |
| Pre-certified connector to a SaaS app | Native Connector |
| Agent-to-agent communication across organizations or platforms | A2A |

### Model Size Selection

| Use LLM (e.g., GPT-4o) | Use SLM (e.g., Phi-4) |
|---|---|
| Complex reasoning, broad knowledge | Simple, focused, narrow domain task |
| Cloud deployment acceptable | On-device or edge deployment |
| Long context window needed | Cost per token is critical |

### Responsible AI Principles (know all six)

| Principle | Key Test Angle |
|---|---|
| Fairness | Responses must not discriminate |
| Reliability & Safety | Fail safely, fallback topics, error handling |
| Privacy & Security | Prevent data leakage, enforce access controls |
| Inclusiveness | Accessibility, all users can interact |
| Transparency | Users know they're interacting with AI |
| Accountability | Audit trails, human oversight, clear ownership |

### Security Threat Quick Reference

| Threat | Key Mitigation |
|---|---|
| Direct prompt injection | Input validation, content filters |
| Indirect prompt injection (XPIA) | XPIA protection in Copilot Studio, data source allow-listing |
| Jailbreaking | Safety system messages, Microsoft content safety |
| Data exfiltration | Least-privilege, output filtering, DLP |
| Prompt leakage | Never store secrets in system prompts |

---

## Highest-Weight Topics Checklist (Deploy = 40–45%)

Before your exam, confirm you can answer scenario questions on each:

**ALM (Notebook 08)**
- [ ] ALM approach differs for: Copilot Studio agents vs. Foundry agents vs. D365 AI
- [ ] Managed vs. unmanaged solutions — when each is used
- [ ] What IS and ISN'T included in a Copilot Studio solution export
- [ ] Grounding data also needs ALM (not just agents)

**Monitoring & Testing (Notebook 09)**
- [ ] Application Insights Agents view — unified across Foundry, Copilot Studio, third-party
- [ ] Key metrics: resolution rate, escalation rate, groundedness score, P95 latency
- [ ] Difference between monitoring (production) and evaluation (pre-production)
- [ ] Continuous improvement loop: telemetry → identify → root cause → update → deploy → monitor

**Security & Responsible AI (Notebook 10)**
- [ ] All six responsible AI principles by name
- [ ] Direct vs. indirect (XPIA) prompt injection — difference and mitigations
- [ ] Data residency checklist: where data is stored, where inference runs, where logs are stored
- [ ] Audit trails required for BOTH model changes AND data changes

---

## Exam Tips

- **Read every option before choosing** — the correct answer is often the most precise match to the scenario constraint, not just "correct in general"
- **Watch for distractor platforms** — questions often include all four platforms (Copilot Studio, Foundry, M365 Copilot, D365); eliminate by constraint
- **"Extend" answers are frequently correct** for M365 scenarios — don't default to "build custom"
- **Deploy domain is 40–45%** — if you're short on study time, prioritize Notebooks 08, 09, and 10
- **Responsible AI questions are straightforward** — know the six principles and you will get those questions right
- **A2A ≠ Copilot Studio agent-to-agent** — A2A is cross-platform/cross-org; Copilot Studio has its own agent-calling mechanism
