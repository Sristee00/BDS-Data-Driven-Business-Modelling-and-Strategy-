# Semantic Ambiguity in Trademark Classification
## An NLP-Based Analysis of Nice Class 3 and Nice Class 5

## Project Overview
This repository contains the code and documentation for a data science project investigating semantic ambiguity in trademark goods descriptions, focusing on the boundary between Nice Class 3 (cosmetics and cleaning preparations) and Nice Class 5 (pharmaceutical and medical products).

Although these two classes are legally distinct, they frequently overlap in terminology, creating uncertainty for trademark applicants and examiners. This project explores whether modern Natural Language Processing (NLP) techniques can help distinguish clear cases from genuinely ambiguous ones.

---

## Research Questions
1. To what extent do the semantic properties of trademark descriptions in Nice Class 3 and Class 5 overlap?
2. Can NLP models reliably distinguish between Class 3 and Class 5 despite their semantic similarity?
3. How can data-driven tools support examiners and applicants in borderline classification cases?

---

## Data
- Source: European Union Intellectual Property Office (EUIPO) trademark applications  
- Scope: Applications containing Nice Class 3, Class 5, or both  
- Unit of analysis: Trademark application (goods descriptions aggregated per application)

### Labels
- `3_only` – applications containing only Class 3 goods  
- `5_only` – applications containing only Class 5 goods  
- `both` – applications containing goods from both classes  


---

## Methods
The analytical pipeline includes:
- **Sentence-BERT (SBERT)** for multilingual semantic embeddings
- **Multinomial Logistic Regression** for supervised classification
- **UMAP** for dimensionality reduction and visualization
- **HDBSCAN** for unsupervised clustering
- **Cosine similarity** to measure semantic proximity
- **Manual validation** of borderline cases
- **External validation** using a large language model (LLM)

---


