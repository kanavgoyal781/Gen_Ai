# Fine-Tuning LLMs with QLoRA

This repository contains my work for **ADSP 32027 – Generative AI I: Principles & Applications**.  
The assignment involves fine-tuning a large language model using **Supervised Fine-Tuning (SFT)** with **QLoRA** (4-bit quantization + LoRA adapters).

---

## 🎯 Objective

- Fine-tune a language model of your choice using **QLoRA** (4-bit + LoRA).
- Choose a compatible model and dataset, then replicate and extend the lecture notebook.
- Track training performance and evaluate outputs.

---

## 🏗 Steps Followed

### ✅ Step 1: Choose a Model
Select a model from Hugging Face that supports LoRA adapters:
- **Mistral 7B** – `mistralai/Mistral-7B-v0.1`
- **Llama 2 7B** – `meta-llama/Llama-2-7b-hf`
- **Falcon 1B** – `tiiuae/falcon-rw-1b`
- **DeciLM 6B** – `Deci/DeciLM-6b`
- **BloomZ 1B1** – `bigscience/bloomz-1b1`

### ✅ Step 2: Choose a Dataset
Select one of the following:
- **Alpaca** – Instruction-following dataset (52k examples)
- **Dolly 15K** – Instruction-following dataset by Databricks
- **OpenAssistant Conversations** – Chat-style data
- **Samsum** – Dialogue summarization dataset
- **P3 (SuperNI)** – Diverse instructions

*(Only a small subset of 1k–5k examples is used to stay within compute limits.)*

### ✅ Step 3: Fine-Tuning & Evaluation
- Fine-tune model with **QLoRA** (4-bit).
- Track **training loss** during fine-tuning.
- Perform basic inference on test prompts.
- Evaluate results using:
  - **BLEU**
  - **ROUGE-L**
  - *(Optional)* Exact Match score

---

## 📦 Deliverables

- 📒 **Notebook (.ipynb + HTML export)** showing the fine-tuning process and results.
- 📑 **2–3 sample generated outputs** from the fine-tuned model.
- 🔍 Notes on hyperparameters and any changes made.

---

## 🛠 Notes & Tips
- Used **4-bit quantization** to reduce memory usage.
- Focused on improving instruction-following ability.
- Trained for **1 epoch** due to hardware limits.
- Optionally logged results via **Weights & Biases (W&B)**.

---

## 📂 Repository Structure
