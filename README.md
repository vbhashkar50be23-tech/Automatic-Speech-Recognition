# Automatic-Speech-Recognition
End-to-End ASR Error Analysis &amp; WER Optimization Pipeline  This project focuses on building an end-to-end Automatic Speech Recognition (ASR) evaluation and improvement pipeline using the Whisper model. Instead of training a model from scratch, the project emphasizes error analysis, evaluation, and post-processing techniques to improve transcription

# 🚀 End-to-End ASR Error Analysis & WER Optimization Pipeline

This project builds an **end-to-end Automatic Speech Recognition (ASR) pipeline** using OpenAI Whisper, with a strong focus on **evaluation, error analysis, and post-processing improvements**.

Instead of training a model from scratch, the project demonstrates how **systematic analysis and lightweight transformations** can significantly improve transcription quality.

---

## 🔍 Overview

The pipeline:
- Processes audio inputs  
- Generates transcriptions using Whisper  
- Evaluates performance using **Word Error Rate (WER)**  
- Identifies error patterns  
- Applies post-processing corrections  

👉 The goal is to **reduce transcription errors through intelligent data processing**, not model retraining.

---

## ⚙️ Pipeline Architecture



---

## 🧠 Key Features

- ✔ End-to-end ASR pipeline  
- ✔ Batch processing of audio samples  
- ✔ WER-based evaluation  
- ✔ Error taxonomy (phonetic, substitution, tokenization)  
- ✔ Rule-based post-processing (normalization & correction)  
- ✔ Data quality improvement framework  
- ✔ Visualization of WER improvement  

---

## 📊 Results

| Stage | WER |
|------|------|
| Baseline | 0.21 |
| After Abbreviation Fix | 0.18 |
| After Cleaning | 0.06 |
| Final (No Data Leakage) | **0.10** |

👉 Achieved **~50% relative reduction in WER**

---

## 🔬 Error Analysis

Common error types observed:

- **Phonetic Errors**  
  - *leighton → layton*  

- **Substitution Errors**  
  - *jingo → jingle*  

- **Tokenization Errors**  
  - *shampooer → shampoo or*  

👉 Insight: Most errors are due to **lexical and formatting inconsistencies**, not acoustic failures.

---

## 🛠 Tech Stack

- Python  
- OpenAI Whisper  
- Hugging Face Datasets  
- JiWER  
- Pandas / NumPy  
- Matplotlib  

---

## 📦 Installation

```bash
pip install openai-whisper datasets jiwer soundfile pandas matplotlib
