# fmRouter 0.1 
### by B. Alexander 2025  - MIT license
<img width="610" height="260" alt="image" src="https://github.com/user-attachments/assets/10ea67e1-faf7-4551-a981-2e7eeded1f5d" />

## Prompt Library and Multi-Model  AI Playground  for Claris FileMaker Pro
Lightweight, yet comprehensive prompt playground architecture that lets FileMaker developers create, version, and compare prompts and their outputs across multiple LLMs through free or paid models via  any provider e.g.  [OpenRouter](https://openrouter.ai)  or locally via [LM Studio](https://lmstudio.ai) . Endpoints, Models, Sources can all be dynamic making it a trully exciting way to track your prompt libaries and see them in action and compare results over time with a prompting and execution log.

This uses  only native FileMaker 2025 script steps. No plugins or addons . 
FileMaker 2025 makes all of this possible without the Insert From URL step too.

---

## Use Cases

- Create a New Prompt / Edit Existing Prompts.
- Edit and  Automatically save Version History.
- Run a Prompt from Playground with dynamic variables for models, endpoint, temperature settings etc.
- Keep track of executions, models, prompts and version.
---
## 🧭 Data Model Overview

This repository includes the **full XML copy and DDR**, so you can explore the schema in detail using DDR tools like [**FM Perception**](https://www.geistinteractive.com/products/fm-perception/) or [**InspectorPro**](https://www.productivecomputing.com/inspectorpro).

| Table | What It Does |
|-------|--------------|
| Playgrounds | Define endpoints (OpenRouter, LM Studio, custom APIs) |
| Prompts | Your prompt library with metadata and tags |
| Versions | Auto-saved history—rollback to any previous version |
| Executions | Complete audit trail: model, temperature, tokens, cost, response |
| Models | Pre-configured model list (easily add custom models) |
| Datasets | Inject FileMaker data into prompts for context-aware AI |
| Entries (External)*| Secure credential storage in separate filemaker file |
---
### 🚀 Summary

* 🔀 **Route prompts to multiple models** and compare outputs side by side
* 📝 **Create and version JSON based prompts directly inside FileMaker and also pass in data from the database**
* 🧪 **Run controlled experiments**
* 💾 **Log every execution** 

## Bonus - You can create and manage JSON prompts directly inside **fmRouter**
or there is also a custom GPT from the same authaor for creating powerful, structured JSON Prompts  . 
This GPT is based on the smart metamprompting technique outlined at 
https://github.com/binu-alexander/metaprompter by the same author. 
https://chatgpt.com/g/g-68aea2a957a8819186af31f366b178df-baxter-prompt-butler-json.

---
## Screenshots

**Playground Screen**
<img width="1672" height="917" alt="000286 CleanShot 2025-10-08 at 10 00 29" src="https://github.com/user-attachments/assets/21943edc-f29d-4a3f-aac3-27d47849ca8f" />

**Prompt Management and Execution History**
![Uploading 000287 CleanShot 2025-10-08 at 10.01.00.png…]()


<img width="1506" height="960" alt="000285 CleanShot 2025-10-08 at 09 59 10" src="https://github.com/user-attachments/assets/7bb51bb9-b862-4a7a-a877-81c4832c74b7" />


## 📄 Licensing 

Released under the **MIT License** — free to use, modify, and extend as you like. 


### Request demo file 

[fmrouter@thedatadrivenlife.com](mailto:fmrouter@thedatadrivenlife.com)


---

