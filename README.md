

# PalGeoLLM

**PalGeoLLM** is a mobile chatbot application that provides accurate and unbiased information about Palestine’s geography and history. It is powered by a fine-tuned Large Language Model (LLM) trained on over 20,564 Arabic question-answer pairs.

---

## Overview

Understanding Palestine’s geography and preserving its cultural identity is more important than ever. This project integrates machine learning and mobile development to offer a chatbot that can accurately answer questions about Palestine, from cities and landmarks to historical and demographic details.

---

## Core Features

- **Custom Arabic Dataset**: 20,564 manually and semi-synthetically curated Q&A pairs.
- **Fine-tuned LLMs**: Three models evaluated — `aya-expanse-8b`, `LLaMAX 3`, and `Mistral-7B-Instruct-v0.3`.  
  ✅ *Final Model: Mistral-7B-Instruct-v0.3* for its top accuracy.
- **Instruction Fine-Tuning** with QLoRA.
- [**APIs via Hugging Face** for seamless integration.](https://huggingface.co/abulbudz/mistral-palestinian-assistant)
- **Flutter-based Mobile App** (iOS & Android).
- **Local SQLite** database support.

---

## Dataset Summary

- **Manual QA Pairs**: 4,613
- **LLM-extracted Pairs**: 13,261 (semi-synthetic)
- **Structured Data Extraction**: 2,690 (from [Palestinian village encyclopedias](https://www.palquest.org/))

---

## Model Evaluation

| Model                | BERT F1 Score | LLM-as-a-Judge Rating |
|---------------------|---------------|------------------------|
| aya-expanse-8b      | 0.75          | ⭐⭐⭐⭐☆                |
| LLaMAX 3            | 0.70          | ⭐⭐⭐⭐☆                |
| **Mistral (Final)** | **0.74**      | ⭐⭐⭐⭐⭐                |

---

## 🛠️ Technologies Used

- **Python**: Model fine-tuning and data processing
- **Transformers / PEFT / QLoRA**
- **Label Studio**: Data annotation
- **Hugging Face Hub**: Model deployment
- **Flutter SDK**: Mobile development
- **SQLite**: Local storage

---

## 🔧 How to Run

1. Clone the repo:
   ```bash
   https://github.com/SinaLab/PalGeoLLM.git 
    ```

2. Set up the **Flutter app**:
    
    ```bash
    cd app
    flutter pub get
    flutter run
    ```
    
3. Backend (LLM) is hosted on Hugging Face and queried via HTTP API from the mobile app.
    

---

## Objectives

- Counter LLM biases against Palestine by fine-tuning on reliable Arabic sources.
    
- Build an accessible and educational mobile tool.
    
- Raise awareness of Palestine’s geographic and cultural identity.
    

---

## Support Palestine Through Technology

> “Technology is a tool — we chose to use it to preserve our truth.”

- [**Ahmad Budairi** ](https://github.com/ahmadbudz)
- [**Mitri Khoury** ](https://github.com/mitrikhoury)
- [**Belal Hamdeh** ](https://github.com/Hamdeh-Belal)

   
