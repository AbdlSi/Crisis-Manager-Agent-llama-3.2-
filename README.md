# Crisis-Manager-Agent-llama-3.2
## Project Overview

- Fine-tuned a **LLaMA-based Causal Language Model** using instruction-formatted data.
- Built a complete training pipeline including **data preprocessing, formatting, training, and inference testing**.
- Converted raw prompts into structured **JSONL instruction format** for supervised fine-tuning.
- Used **Hugging Face Transformers + TRL (SFTTrainer)** for model training.
- Implemented evaluation using validation loss and behavioral prompt testing.
- Applied controlled generation settings to ensure stable and reproducible inference.
- Designed a structured repository layout for scalability and reproducibility.
- Tested model robustness using targeted behavioral prompts:
  - Refund escalation scenario
  - Insult handling scenario
  - Competitor comparison scenario
- Ensured clean separation between:
  - Training data
  - Validation data
  - Test / behavioral evaluation prompts


 ## Objectives

- Improve instruction-following behavior.
- Enforce polite refusal patterns.
- Handle adversarial or emotionally charged prompts appropriately.
- Evaluate generalization on unseen test prompts

## Files Structure
```
LLaMA-FineTuning-Project/
│
├── notebooks/
│   ├── data_preprocessing.ipynb        
│   └── finetunning.ipynb               
│
├── data/
│   ├── llama_formated_prompt.jsonl     
│   └── responses.jsonl                 
│                   
├── requirements.txt                   
└── README.md
```
