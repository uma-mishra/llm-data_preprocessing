# ✨ Text Preprocessing Using LLMs on Amazon Reviews

This project focuses on improving the quality of product reviews from the Amazon Polarity dataset using Large Language Model (LLM) based text cleaning. The goal is to remove noise, enhance readability, and reduce vocabulary complexity — making the data more effective for downstream NLP tasks such as sentiment classification.

---

## 📌 Dataset Details

**Amazon Polarity Dataset — Hugging Face**  
- Two sentiment labels:  
  `0 = Negative`, `1 = Positive`
- Contains product reviews from multiple categories (electronics, books, home items, etc.)
- A **subset of 300 samples** was used for efficient LLM processing

---

## 🧹 Preprocessing Methods

| Technique | Description |
|----------|-------------|
| Traditional Cleaning | Lowercasing, removing website links, symbols, and extra spaces |
| LLM-based Cleaning (FLAN-T5) | Grammar correction, improved readability, removal of noisy wording |

The LLM preserves the **meaning and sentiment**, while improving language clarity.

---

## 📊 Results Summary

| Metric | Raw Corpus | Cleaned Corpus | Improvement |
|--------|------------|----------------|-------------|
| Vocabulary Size | 4090 | 3236 | 🔻 Reduced ~21% |
| Average Text Length | 79.17 | 63.83 | 🔻 Reduced ~19% |

✔ Text became more concise  
✔ Less redundant vocabulary  
✔ Better formatted and understandable reviews

---

## 📝 Example Output

- Original and cleaned text pairs were printed to verify correctness
- The sentiment was successfully preserved while improving structure

---

## 📈 Visualization

A comparison bar chart demonstrates:

- Drop in vocabulary size
- Shorter and cleaner review text

This confirms that preprocessing **positively impacts dataset quality**.

---

## ▶️ How to Run

1. Install Python libraries:  
   pip install transformers datasets sentencepiece matplotlib

2. Open and execute the notebook file:  
   Amazon_DataPreprocessing.ipynb

3. The cleaned dataset is exported as:  
   amazon_cleaned_llm.csv

---
