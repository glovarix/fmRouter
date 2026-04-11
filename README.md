# fmRouter 0.2

## Prompt Library, Multi-Model AI Playground, and Evaluation Suite for Claris FileMaker Pro

Lightweight, yet comprehensive prompt playground architecture that lets FileMaker developers create, version, and compare prompts and their outputs across multiple LLMs — through free or paid models via any provider e.g. [OpenRouter](https://openrouter.ai) or locally via [LM Studio](https://lmstudio.ai). Endpoints, Models, and Sources are all dynamic, making it a powerful way to track your prompt libraries, see them in action, and rigorously evaluate results over time.

This uses only native FileMaker 2025 script steps. No plugins or addons.
FileMaker 2025 makes all of this possible without the Insert From URL step too.

This repository includes the **full XML copy and DDR**, so you can explore the schema in detail using DDR tools like [**FM Perception**](https://www.geistinteractive.com/products/fm-perception/), [**InspectorPro**](https://www.productivecomputing.com/inspectorpro), or [**FMDojo**](https://www.fmdojo.com).

---

## What's New in 0.2

### A) Non-JSON Prompt Support

Prompts are no longer limited to JSON format. You can now create and run prompts in **Markdown**, plain text, or any other format that your model and use case requires. This makes fmRouter suitable for a much wider range of workflows — from structured JSON tool-calling prompts to free-form creative or instructional prompts.

### B) Evaluations and LLM-as-Judge

This is the headline feature of 0.2. fmRouter now supports a full **evaluation pipeline** alongside prompt execution:

- **Trace prompt executions** — every run is logged with its full context: model, endpoint, temperature, prompt version, and output.
- **Custom evaluations** — attach evaluation criteria to any prompt and assess outputs using your own rubric or an LLM-as-Judge approach.
- **Compare across runs** — compare outputs from different models, parameter settings, or prompt versions side by side with structured scoring.
- **LLM-as-Judge** — route outputs to a designated judge model that scores and reasons about response quality, making automated quality assessment a first-class workflow inside FileMaker.

This turns fmRouter from a prompt runner into a proper **evaluation and observability platform** for AI workflows built in FileMaker.

### C) agentic-fm Integration

fmRouter now integrates with **[agentic-fm](https://www.agentic-fm.com)** — the Agentic FileMaker Coding framework. This enables agentic, multi-step AI coding workflows directly within the FileMaker ecosystem, connecting fmRouter's prompt and evaluation infrastructure to broader agent-driven development tasks.

---

## Core Use Cases and Flow

- Create a New Prompt / Edit Existing Prompts (JSON, Markdown, or plain text).
- Edit and automatically save Version History.
- Run a Prompt from the Playground with dynamic variables for models, endpoint, temperature settings etc.
- Evaluate outputs using LLM-as-Judge or custom scoring criteria.
- Trace, compare, and analyze executions across models, versions, and settings.

![fmRouter navigation](https://github.com/user-attachments/assets/ba6f91e8-d8d6-49bc-87a4-7f617cf3aa95)

---

## Summary

- **Route prompts to multiple models** and compare outputs side by side
- **Create and version prompts** in JSON, Markdown, or plain text — directly inside FileMaker, with database variable injection
- **Run controlled experiments** across models, parameters, and prompt versions
- **Evaluate outputs** with LLM-as-Judge and custom rubrics
- **Log and trace every execution** for full observability
- **Agentic workflows** via [agentic-fm](https://www.agentic-fm.com) integration

---

## Bonus — Prompt Creation Tools ( for JSON prompts )

You can create and manage prompts directly inside **fmRouter**, or use the companion custom GPT for building powerful, structured JSON prompts.
This GPT is based on the metaprompting technique outlined at
[github.com/binu-alexander/metaprompter](https://github.com/binu-alexander/metaprompter) by the same author.

[Baxter — Prompt Butler (JSON) on ChatGPT](https://chatgpt.com/g/g-68aea2a957a8819186af31f366b178df-baxter-prompt-butler-json)

---

## Screenshots

### Playground Screen

![Playground Screen](https://github.com/user-attachments/assets/55f75988-92dd-44c8-b991-14158ef8e8e5)

### Prompt Management and Execution History

![Prompt Management and Execution History](https://github.com/user-attachments/assets/7bb51bb9-b862-4a7a-a877-81c4832c74b7)

---

## Licensing - MIT

The MIT License is a permissive, free software license developed at MIT that allows users to freely use, copy, modify, merge, publish, distribute, sublicense, and sell software with very few restrictions. The only main requirements are to include the original copyright and license notice with all copies or substantial portions of the software. It comes with no warranty and no liability for the authors.

### Request demo file

[fmrouter@thedatadrivenlife.com](mailto:fmrouter@thedatadrivenlife.com)

---
