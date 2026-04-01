# Notebook 9: Deploy — Monitoring, Telemetry, Testing & Performance

## Copilot Studio Agent Setup

**Agent:** AB-100 | Deploy: Monitoring, Telemetry & Testing

**System Instructions:**
> "Focus on the tools and processes for monitoring AI agents in production, how to interpret telemetry data from Application Insights and Microsoft Foundry, how to analyze agent performance metrics, how to use backlog and user feedback for continuous improvement, how to apply AI-based tools for issue identification and tuning, and how to design and manage the testing of AI-powered solutions including validation criteria for custom models and test case strategy."

**Suggested Topics to create:**
- *Metrics Interpreter* — trigger: "interpret my agent metrics" — agent explains what low resolution rate, high escalation rate, or poor groundedness scores mean and what to do
- *Monitoring Stack Quiz* — trigger: "quiz me on monitoring tools" — agent tests knowledge of Application Insights, Foundry Observability, and Copilot Studio analytics
- *Continuous Improvement Walkthrough* — trigger: "improve my agent" — agent steps through the 7-step improvement loop
- *Testing Strategy Builder* — trigger: "build a testing strategy" — agent asks about the agent type and generates appropriate test types

---

## Exam Skills Covered

From the AB-100 Study Guide — *Deploy AI-powered business solutions (40–45%)*:

**Analyze, monitor, and tune AI-powered business solutions**
- Recommend the process and tools required for monitoring agents
- Analyze backlog and user feedback of AI and agent usage
- Apply AI-based tools to analyze and identify issues and perform tuning
- Monitor agent performance and metrics
- Interpret telemetry data for performance and model tuning

**Manage the testing of AI-powered business solutions**
- Recommend the process and metrics to test agents
- Create validation criteria of custom AI models
- Validate effective Copilot prompt best practices
- Design end-to-end test scenarios of AI solutions that use multiple Dynamics 365 apps
- Build the strategy for creating test cases by using Copilot

---

## Sources to Add

### Monitoring & Observability Documentation

| Title | URL |
|---|---|
| Monitor AI Agents with Application Insights | https://learn.microsoft.com/en-us/azure/azure-monitor/app/agents-view |
| Application Insights OpenTelemetry Overview | https://learn.microsoft.com/en-us/azure/azure-monitor/app/opentelemetry-overview |
| Foundry Observability (Concepts) | https://learn.microsoft.com/en-us/azure/foundry/concepts/observability |
| Run Evaluations in Foundry Portal | https://learn.microsoft.com/en-us/azure/foundry/how-to/evaluate-generative-ai-app |
| Continuous Evaluation of AI Agents | https://learn.microsoft.com/en-us/azure/foundry/how-to/continuous-evaluation-agents |

### Copilot Studio Specific

| Title | URL |
|---|---|
| Copilot Studio: 6 Core Capabilities to Scale Agent Adoption | https://www.microsoft.com/en-us/microsoft-copilot/blog/copilot-studio/6-core-capabilities-to-scale-agent-adoption-in-2026/ |
| Configure High-Quality Instructions (Generative Orchestration) | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/generative-mode-guidance |

---

## Key Concepts to Understand

### Monitoring Stack for AI Agents

| Layer | Tool | What It Captures |
|---|---|---|
| **Agent runtime** | Application Insights (Agents view) | Conversations, tool calls, latency, errors, sessions |
| **Model performance** | Foundry Observability | Token usage, groundedness scores, model latency, evaluation results |
| **Infrastructure** | Azure Monitor | Resource health, scaling events, availability |
| **User feedback** | Copilot Studio analytics | Thumbs up/down ratings, escalation rate, topic coverage |
| **Conversation analysis** | Copilot Studio transcript review | Drop-off points, unresolved topics, unexpected paths |

### Key Metrics to Track

| Metric | What It Tells You |
|---|---|
| **Resolution rate** | % of conversations resolved without escalation |
| **Escalation rate** | % of conversations handed off to a human |
| **Topic coverage** | Which topics are triggered most / least |
| **CSAT / thumbs rating** | User satisfaction with agent responses |
| **Groundedness score** | How well responses are anchored in source data |
| **Latency (P50/P95)** | Response time distribution — P95 reveals slow outliers |
| **Tool call success rate** | % of tool/action calls that succeed |
| **Token usage** | Cost driver; spikes indicate inefficient prompts |

### Continuous Improvement Loop
1. Collect telemetry + user feedback
2. Identify top failure modes (unresolved topics, low-rated responses)
3. Review conversation transcripts for root cause
4. Update topics, instructions, or grounding data
5. Re-evaluate with Foundry evaluation framework
6. Deploy via ALM pipeline
7. Monitor for improvement

### Tuning Approaches
- **Prompt tuning:** Refine agent instructions, system messages, few-shot examples
- **Knowledge tuning:** Add, update, or reindex grounding data sources
- **Model tuning:** Fine-tune with additional domain data (Foundry)
- **Topic tuning:** Add trigger phrases, fix entity recognition, update conditions
- **Tool tuning:** Fix action parameters, update API connections, add retry logic

---

## Exam Tips

- Application Insights now has a unified **Agents view** that shows agents from Foundry, Copilot Studio, and third-party systems in one place — know this exists
- OpenTelemetry / GenAI semantic conventions are how Foundry Agent Service emits traces — you don't need deep OpenTelemetry knowledge, but understand what tracing provides
- The exam may present a scenario with low CSAT or high escalation rate and ask you to identify the right tuning action
- Distinguish between *monitoring* (production, ongoing) and *evaluation* (pre-production, model quality testing)
- User feedback (thumbs ratings, escalation signals) is a first-party signal — always analyze it alongside telemetry
