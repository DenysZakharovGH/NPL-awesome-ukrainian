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

| 🎭 Epoch | 🎯 F1-Score | 🧮 Acc | 📈 Valid Loss |
|------------|-------------|--------------|------------|
| **1** | 0.74 | 0.76 | 0.70 |

---

| Comment UA | Commect Eng | Detected emotion |
|------------|-------------|--------------|
| **Я дуже радий цьому!** | I am really happy about that! | positive (0.91) |
| **Мені страшно за майбутнє** | I am afraid about my future | negative (0.87) |
| **Це найгірший день у моєму житті.** | That is a worth day in my life | negative (0.86) |
| **не ну такого я ще не бачив** | emmm so, I haven't seen such thing before | negative (0.82) |
| **Отримав провід — працює, але горить червоним індикатором** | Got cable - works, but red indicator lights | neutral (0.91) |

---
