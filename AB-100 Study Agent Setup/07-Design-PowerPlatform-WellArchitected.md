# Notebook 7: Design — Power Platform AI & Well-Architected Framework

## Copilot Studio Agent Setup

**Agent:** AB-100 | Design: Power Platform AI & Well-Architected

**System Instructions:**
> "Focus on the Power Platform Well-Architected Framework applied to intelligent application workloads, how to design AI components in Power Apps canvas apps, the AI hub in Power Platform, how to use Copilot features in Power Automate and Power Apps, and the responsible AI design principles for Power Platform intelligent applications."

**Suggested Topics to create:**
- *WAF Pillar Quiz* — trigger: "quiz me on the well-architected framework" — agent presents AI workload scenarios and asks which pillar applies
- *Canvas App AI Design* — trigger: "add AI to a canvas app" — agent walks through options (Copilot control, agent feed, AI Builder)
- *AI Hub Explainer* — trigger: "what is the AI hub" — agent explains Power Platform AI hub governance role
- *Generative Pages vs Agent Feed* — trigger: "generative pages or agent feed" — agent compares the two approaches

---

## Exam Skills Covered

From the AB-100 Study Guide — *Design AI-powered business solutions (25–30%)*:

**Design AI and agents for business solutions**
- Apply the Microsoft Power Platform Well-Architected Framework to intelligent application workloads
- Design a business process to include AI components in a Power Apps canvas app
- Propose code-first generative pages and the use of an agent feed for apps

**Orchestrate configuration for prebuilt agents and apps**
- Propose Microsoft Power Platform AI features, including AI hub

---

## Sources to Add

### Power Platform Well-Architected Framework

| Title | URL |
|---|---|
| Power Platform Well-Architected Hub | https://learn.microsoft.com/en-us/power-platform/well-architected/ |
| Intelligent Application Workloads Overview | https://learn.microsoft.com/en-us/power-platform/well-architected/intelligent-application/overview |
| Design Principles for Intelligent Application Workloads | https://learn.microsoft.com/en-us/power-platform/well-architected/intelligent-application/design-principles |
| Responsible AI for Intelligent Application Workloads | https://learn.microsoft.com/en-us/power-platform/well-architected/intelligent-application/responsible-ai |

### Power Platform AI Features

| Title | URL |
|---|---|
| Copilots and Generative AI in Power Platform | https://learn.microsoft.com/en-us/power-platform/copilot |
| Power Platform 2026 Release Wave 1 Plan | https://learn.microsoft.com/en-us/power-platform/release-plan/2026wave1/ |
| Power Platform ALM Hub | https://learn.microsoft.com/en-us/power-platform/alm/ |

### Videos

| Title | URL |
|---|---|
| Power Apps Maker Copilot | https://www.youtube.com/watch?v=UwbCIZTx59I |
| Power Automate Copilot | https://www.youtube.com/watch?v=FMz0C6cY1qU |
| Power Platform on Microsoft Mechanics (playlist) | https://www.youtube.com/playlist?list=PLXtHYVsvn_b9MQ5eu2zb9ZYNLnDWsYAeL |
| Microsoft Power Platform channel | https://www.youtube.com/@MSPowerPlatform |

---

## Key Concepts to Understand

### Power Platform Well-Architected Pillars

| Pillar | Applied to AI Workloads |
|---|---|
| **Reliability** | Agent uptime, fallback behaviors, error handling, retry logic |
| **Security** | Data access controls, authentication, prompt injection protection |
| **Operational Excellence** | ALM, monitoring, telemetry, continuous improvement |
| **Performance Efficiency** | Model selection, caching, response latency targets |
| **Experience Optimization** | UX design for AI features, accessibility, user feedback loops |

### AI Features in Power Platform Apps

| Feature | App | Description |
|---|---|---|
| **Copilot in Power Apps** | Canvas & Model-driven | Natural language app building, Copilot control in canvas apps |
| **AI Hub** | Power Platform admin | Centralized management of AI connections, models, and governance |
| **Copilot in Power Automate** | Power Automate | Natural language flow creation, AI Builder integration |
| **Agent feed** | Canvas apps | Embeds an agent conversation into a canvas app surface |
| **Generative pages** | Code-first | Dynamic, AI-generated UI pages for apps |

---

## Exam Tips

- The Power Platform WAF is *distinct* from the Azure Well-Architected Framework — know the Power Platform-specific pillars and their names
- The AI hub is for *managing* AI models and connections across Power Platform — not for building models
- Agent feed allows embedding a Copilot Studio agent directly within a Power Apps canvas app as a conversational control
- Generative pages are code-first (not low-code) and use AI to dynamically render UI based on data and context
- Responsible AI for intelligent workloads maps to the same six Microsoft principles but applied specifically to Power Platform architecture decisions
