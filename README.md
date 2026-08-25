# **MWE–Google Translate Evaluation**  
A corpus‑linguistics project evaluating Google Translate’s handling of English→Arabic multiword expressions (MWEs) using the UN Parallel Corpus.

## 📌 Overview  
This project analyzes how accurately Google Translate renders English multi‑word expressions (MWEs) into Arabic.  
MWEs were extracted from the UN English corpus using AntConc’s N‑gram tool, aligned with UN human Arabic translations, and evaluated using the MQM Core Typology.  
The goal is to identify where Google Translate succeeds, where it fails, and which error types occur most frequently in domain‑specific UN texts.

---

## 🎯 Project Goals  

### ✔ MWE Extraction (AntConc)  
- Extract 2‑, 3‑, 4‑, 5‑, and 6‑grams  
- Merge, sort, and deduplicate  
- Manually clean non‑idiomatic or noisy N‑grams  
- Produce a refined MWE list

### ✔ Parallel Corpus Construction  
- Use UN English + UN Arabic files  
- Align by **line breaks** (IDs were unreliable)  
- Extract a 5,000‑line sample  
- Generate Google Arabic translations for the same lines  
- Build a 3‑row parallel corpus:
  - English  
  - UN Arabic  
  - Google Arabic  

### ✔ MQM Evaluation  
Evaluate each MWE using MQM categories:
- **Accuracy** (mistranslation, omission, addition, undertranslation)  
- **Terminology** (wrong term, inconsistent term)  
- **Style** (unidiomatic, awkward, register issues)  
- **Linguistic conventions** (grammar, writing norms)

### ✔ Results & Analysis  
- Identify correct vs. incorrect MT output  
- Analyze error patterns  
- Compare MT behavior across idiomatic, legal, financial, and institutional MWEs

---

### ⚠️ Corpus Notice  
The UN Parallel Corpus is copyrighted.  
This repository **does NOT include**:
- full UN corpus files  
- 5,000-line English/Arabic/Google samples  
- alignment databases  
- UNv1.0.* files  

Only a **tiny illustrative sample** (10–20 lines) may be included.

---

## 📊 Key Findings  

### ✔ Correct Translations  
Google Translate correctly rendered **29 MWEs**, especially common expressions with stable Arabic equivalents.

### ❌ Frequent Error Types  
- Wrong term (9)  
- Awkward style (6)  
- Mistranslation (4)  
- Unidiomatic style (3)  
- Inconsistent terminology (3)  
- Grammar (1)  
- Writing norms (1)  
- Do‑not‑translate (1)

### 🔍 Patterns  
Google Translate struggles with:
- legal terminology  
- financial expressions  
- UN institutional language  
- idiomatic meaning  
- stylistic naturalness  
- context‑dependent expressions  

It performs better on general MWEs with predictable Arabic equivalents.

---

## 👩‍💻 Tools & Technologies  
- **AntConc** (N‑gram extraction)  
- **AntPConc** (parallel corpus building)  
- **MQM Core Typology** (error evaluation)  
- **Python** (alignment attempts, preprocessing)  
- **UN Parallel Corpus v1.0** (English–Arabic)

---

## 🚀 How to Reproduce  
1. Download the UN Parallel Corpus v1.0  
2. Extract English + Arabic files  
3. Align by line breaks  
4. Extract MWEs using AntConc  
5. Clean and refine the MWE list  
6. Build a 3‑row parallel corpus using AntPConc  
7. Evaluate MWEs using MQM  
8. Analyze error patterns

---

## 📥 UN Corpus Download  
The corpus used in this project is the **UN Parallel Corpus v1.0 (English–Arabic)**.  
Due to licensing restrictions, the corpus **cannot be redistributed** in this repository.

Download from the official UN website:  
🔗 **UN Parallel Corpus – Official UN Download Page**  
[https://www.un.org/dgacm/en/content/uncorpus/Download](https://www.un.org/dgacm/en/content/uncorpus/Download)

---

## 📄 Report  
The full project write‑up is available in:  
`report/Final_Project.pdf`

---

## 📜 License  
This project was created for academic purposes.  
UN corpus files are **not redistributed**.
