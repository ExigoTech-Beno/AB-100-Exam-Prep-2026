# Notebook 11 (Extra): Prompt Engineering, Language Models & Model Selection

## NotebookLM Setup

**Notebook title:** AB-100 | Extra: Prompt Engineering & Language Models

**Audio Overview Focus Prompt:**
> "Focus on prompt engineering techniques and best practices for AI-powered business solutions, how to build a prompt library, the use of few-shot learning, chain-of-thought, and system message design, how to evaluate grounding data quality, how to select between large and small language models, and how to use generative AI and knowledge sources effectively in agents."

**Suggested audio formats to generate:**
- Standard: Core prompt engineering techniques architects must know
- Extended: Deep dive on system message design, few-shot examples, and prompt library structure
- Quiz: Test yourself on which prompt technique applies to which scenario

---

## Exam Skills Covered

> These skills are part of the **Plan domain** (25–30%) and the **Design domain** (25–30%) of AB-100. They appear in this supplementary notebook because they cut across multiple topic areas — but they are exam-weighted skills, not background reading.

From the AB-100 Study Guide — *Plan AI-powered business solutions (25–30%)*:

**Design overall AI strategy for business solutions**
- Provide guidelines for creating a prompt library
- Provide prompt engineering guidelines and techniques for AI-powered business solutions
- Determine the use of generative AI and knowledge sources in agents built with Copilot Studio *(see also Notebook 02)*
- Develop the use cases for customized small language models for the solution *(see also Notebook 02)*
- Determine when custom AI models should be created *(see also Notebook 02)*

**Analyze requirements for AI-powered business solutions**
- Review data for grounding, including accuracy, relevance, timeliness, cleanliness, and availability *(see also Notebook 01)*

From the AB-100 Study Guide — *Design AI-powered business solutions (25–30%)*:

**Design AI and agents for business solutions**
- Design prompt actions in Copilot Studio *(see also Notebook 03)*
- Design data processing for AI models and grounding *(see also Notebook 03)*

**Design extensibility of AI solutions**
- Design AI solutions by using custom models in Microsoft Foundry *(see also Notebook 05)*

---

## Sources to Add

### Prompt Engineering Documentation

| Title | URL |
|---|---|
| Prompt Engineering Techniques (Foundry) | https://learn.microsoft.com/en-us/azure/foundry/openai/concepts/prompt-engineering |
| Advanced System Message Design (Foundry) | https://learn.microsoft.com/en-us/azure/foundry/openai/concepts/advanced-prompt-engineering |
| Write Effective Prompts for Azure Copilot | https://learn.microsoft.com/en-us/azure/copilot/write-effective-prompts |
| Configure High-Quality Instructions for Generative Orchestration | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/generative-mode-guidance |
| Apply Generative Orchestration | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/generative-orchestration |

### Grounding & Knowledge

| Title | URL |
|---|---|
| Knowledge Sources Summary (Copilot Studio) | https://learn.microsoft.com/en-us/microsoft-copilot-studio/knowledge-copilot-studio |
| Enhance Responses with RAG | https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/retrieval-augmented-generation |
| Module: Build a RAG Solution with Foundry | https://learn.microsoft.com/en-us/training/modules/build-copilot-ai-studio/ |

### Model Selection & SLMs

| Title | URL |
|---|---|
| Foundry Models Overview | https://learn.microsoft.com/en-us/azure/foundry/foundry-models/concepts/models-sold-directly-by-azure |
| Foundry Models from Partners and Community | https://learn.microsoft.com/en-us/azure/foundry/foundry-models/concepts/models-from-partners |
| Module: Fine-Tune a Language Model with Foundry | https://learn.microsoft.com/en-us/training/modules/finetune-model-copilot-ai-studio/ |
| Tech Community: Model Router Cost Optimization | https://techcommunity.microsoft.com/blog/azuredevcommunityblog/optimising-ai-costs-with-microsoft-foundry-model-router/4494776 |
| Model Mondays Playlist (model news & selection) | https://www.youtube.com/watch?v=fjSxraAmGMI&list=PLmsFUfdnGr3wzz6a4E-Szksg92JPng-AL |

---

## Key Concepts to Understand

### Prompt Engineering Techniques

| Technique | When to Use |
|---|---|
| **Zero-shot** | Simple, well-understood tasks where examples aren't needed |
| **Few-shot** | Complex tasks where showing examples improves output format and quality |
| **Chain-of-thought** | Multi-step reasoning tasks; ask the model to "think step by step" |
| **System message design** | Always use to define role, tone, constraints, and output format |
| **Grounding** | Always include relevant data in context when accuracy is critical (RAG) |
| **Output formatting** | Specify format explicitly (JSON, bullet list, table) to improve reliability |

### Prompt Library Structure
A prompt library should include:
- **Purpose:** What the prompt is designed to do
- **Template:** The actual prompt text with placeholders
- **Variables:** What data is injected at runtime
- **Model settings:** Temperature, max tokens, top-p
- **Examples:** Few-shot examples if applicable
- **Quality metrics:** How to evaluate if the prompt performs correctly
- **Version history:** Changes over time with rationale

### LLM vs. SLM Decision Criteria

| Use LLM (e.g., GPT-4o) | Use SLM (e.g., Phi-4) |
|---|---|
| Complex reasoning required | Simple, focused task |
| Broad general knowledge needed | Domain-specific, narrow task |
| Cloud deployment acceptable | On-device or edge deployment needed |
| Cost is not primary constraint | Cost per token is critical |
| Long context window needed | Short, structured inputs/outputs |

### Grounding Data Quality Criteria (exam skill: "Review data for grounding")
- **Accuracy:** Is the data correct and up to date?
- **Relevance:** Is the data applicable to the agent's domain?
- **Timeliness:** Is the data fresh enough for the use case?
- **Cleanliness:** Is the data free of duplicates, noise, and formatting issues?
- **Availability:** Is the data accessible to the agent at runtime?

---

## Exam Tips

- The exam tests whether you can *advise* on prompt engineering — not whether you can write perfect prompts yourself
- Know the grounding data quality criteria (the five listed in the exam skills: accuracy, relevance, timeliness, cleanliness, availability)
- A prompt library is a *governance artifact* — it ensures consistency, reuse, and quality across the organization
- SLMs are increasingly important — know the Phi model family (Phi-4, Phi-4 mini) as Microsoft's primary SLM offering
- System messages define the agent's *persona, constraints, and capabilities* — they are the most important prompt element to get right
