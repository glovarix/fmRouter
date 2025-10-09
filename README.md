# fmRouter 0.1 
### by B. Alexander 2025  - MIT license
<img width="2262" height="912" alt="000295 CleanShot 2025-10-08 at 19 24 57" src="https://github.com/user-attachments/assets/e58ef585-c67e-462b-8f45-9c3b9e3d7e28" />


## Prompt Library and Multi-Model  AI Playground  for Claris FileMaker Pro
Lightweight, yet comprehensive prompt playground architecture that lets FileMaker developers create, version, and compare prompts and their outputs across multiple LLMs through free or paid models via  any provider e.g.  [OpenRouter](https://openrouter.ai)  or locally via [LM Studio](https://lmstudio.ai) . Endpoints, Models, Sources can all be dynamic making it a trully exciting way to track your prompt libaries and see them in action and compare results over time with a prompting and execution log.

This uses  only native FileMaker 2025 script steps. No plugins or addons . 
FileMaker 2025 makes all of this possible without the Insert From URL step too.

---

This repository includes the **full XML copy and DDR**, so you can explore the schema in detail using DDR tools like [**FM Perception**](https://www.geistinteractive.com/products/fm-perception/) or [**InspectorPro**](https://www.productivecomputing.com/inspectorpro).



## Core Use Cases

- Create a New Prompt / Edit Existing Prompts.
- Edit and  Automatically save Version History.
- Run a Prompt from Playground with dynamic variables for models, endpoint, temperature settings etc.
- Keep track of executions, models, prompts and version.
---

### 🚀 Summary

* 🔀 **Route prompts to multiple models** and compare outputs side by side
* 📝 **Create and version JSON based prompts directly inside FileMaker and also pass in data from the database**
* 🧪 **Run controlled experiments**
* 💾 **Log every execution** 

```flowchart TB
    %% Style definitions
    classDef title fill:#293462,stroke:none,color:#fff,font-size:22px,font-weight:bold;
    classDef main fill:#f7fafc,stroke:#3867d6,stroke-width:2px,color:#222,rx:10,ry:10,font-size:16px;
    classDef sub fill:#e3f0fa,stroke:#3867d6,stroke-width:2px,color:#1a3963,rx:8,ry:8,font-size:15px;
    classDef log fill:#fff8e6,stroke:#ebb000,stroke-width:2px,color:#b29300,rx:8,ry:8;
    classDef note fill:#eef6ff,stroke-dasharray: 5, 5,stroke-width:2px,stroke:#3867d6;

    %% Nodes
    T["fmRouter 0.1"]:::title

    PROMPT["<b>Edit / Create Prompts</b><br><span style='font-size:13px'>Version history, structure</span>"]:::main

    subgraph PG
      direction TB
      SETTINGS["<b>Select Model / Endpoint</b><br><span style='font-size:13px'>Choose model, endpoint, temperature etc.</span>"]:::sub
      RUN["<b>Run Prompt</b><br><span style='font-size:13px'>Execute on selected model(s)</span>"]:::sub
    end

    COMPARE["<b>Compare Outputs</b><br><span style='font-size:13px'>Side by side results</span>"]:::main
    LOG["<b>Execution & Version Log</b>"]:::log

    %% Main flow
    T --> PROMPT
    PROMPT --> SETTINGS
    SETTINGS --> RUN
    RUN --> COMPARE
    COMPARE --> LOG

    %% Iteration feedback
    SETTINGS -. "Tweak Model/Settings" .-> RUN
    RUN -. "Revise Prompt" .-> PROMPT

    %% Spacing for better layout
    PROMPT ---| | PG
    PG ---| | COMPARE

    %% Some hidden nodes to increase vertical spacing (for beauty in some renderers)
    linkStyle 5,6 stroke:#0000,stroke-width:0;
```
## Bonus - You can create and manage JSON prompts directly inside **fmRouter**
or there is also a custom GPT from the same authaor for creating powerful, structured JSON Prompts  . 
This GPT is based on the smart metamprompting technique outlined at 
https://github.com/binu-alexander/metaprompter by the same author. 
https://chatgpt.com/g/g-68aea2a957a8819186af31f366b178df-baxter-prompt-butler-json.

---
## Screenshots

**Playground Screen**

<img width="3360" height="1828" alt="000296 CleanShot 2025-10-08 at 23 42 03" src="https://github.com/user-attachments/assets/55f75988-92dd-44c8-b991-14158ef8e8e5" />


**Prompt Management and Execution History**

<img width="1506" height="960" alt="000285 CleanShot 2025-10-08 at 09 59 10" src="https://github.com/user-attachments/assets/7bb51bb9-b862-4a7a-a877-81c4832c74b7" />


## 📄 Licensing - MIT 
The MIT License is a permissive, free software license developed at MIT that allows users to freely use, copy, modify, merge, publish, distribute, sublicense, and sell software with very few restrictions. The only main requirements are to include the original copyright and license notice with all copies or substantial portions of the software. It comes with no warranty and no liability for the authors
### Request demo file 

[fmrouter@thedatadrivenlife.com](mailto:fmrouter@thedatadrivenlife.com)


---

