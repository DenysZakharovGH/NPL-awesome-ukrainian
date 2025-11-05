# 🧠 Ukrainian Emotion Detection 🇺🇦  
### Fine-tuned XLM-RoBERTa for Emotion Recognition in Ukrainian Text  

[![Hugging Face](https://img.shields.io/badge/🤗-Transformers-yellow.svg)](https://huggingface.co/transformers)
[![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white)](https://pytorch.org/)
[![Dataset](https://img.shields.io/badge/Dataset-COSMUS-blue.svg)](https://huggingface.co/datasets/YShynkarov/COSMUS)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## 🚀 Overview  
This project fine-tunes **XLM-RoBERTa** on the [**COSMUS** dataset](https://huggingface.co/datasets/YShynkarov/COSMUS) to detect emotions in **Ukrainian text**.  
The model can recognize emotional tones such as:  
 *positive*,  *negative*,  *mixed*,  *neutral*  

> Emotion recognition for low-resource languages like Ukrainian helps make AI more inclusive and emotionally intelligent 🌍.

---

## 🧩 Features
✅ Fine-tuned multilingual transformer (`xlm-roberta-base`)  
✅ Handles noisy real-world labels (cleaning & normalization included)  
✅ Hugging Face `Trainer` integration for easy training  
✅ Ready-to-use `pipeline()` for inference  
✅ Extendable to other emotion datasets  

---
## 🧾 Model Card  

| 🧩 **Property** | 💡 **Description** |
|-----------------|-------------------|
| **Model Name** | Ukrainian Emotion Detection |
| **Base Model** | [`xlm-roberta-base`](https://huggingface.co/xlm-roberta-base) |
| **Dataset** | [YShynkarov/COSMUS](https://huggingface.co/datasets/YShynkarov/COSMUS) |
| **Task** | Emotion Classification |
| **Languages** | 🇺🇦 Ukrainian |
| **Frameworks** | 🤗 Transformers, 🔥 PyTorch |
| **Problem Type** | Single-label classification |
| **Number of Classes** | 4 (*positive*,  *negative*,  *mixed*,  *neutral* ) |
| **Input Format** | Plain Ukrainian text |
| **Output Format** | Emotion label + confidence score |
| **Trained On** | 80% of COSMUS (cleaned & preprocessed) |
| **Evaluation Metric** | F1-score, Precision, Recall |
| **License** | MIT |

> 🧠 *This model is designed to help NLP systems better understand emotional context in the Ukrainian language.*

---

## 📊 Results  

| 🎭 Emotion | 🎯 F1-Score | 🧮 Precision | 📈 Recall |
|------------|-------------|--------------|------------|
| 😊 **Positive** | 0.90 | 0.91 | 0.89 |
| 😡 **Negative** | 0.84 | 0.85 | 0.83 |
| 😱 **Mixed** | 0.81 | 0.80 | 0.82 |
| 😐 **Neutral** | 0.87 | 0.88 | 0.85 |

📈 **Average F1-score:** `0.86`  
🧪 **Evaluation Dataset:** COSMUS (Validation Split)  

---
