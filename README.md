# BDS-Data-Driven-Business-Modelling-and-Strategy-

Semantic Ambiguity in Trademark Classification
An NLP-Based Analysis of Nice Class 3 and Nice Class 5
Overview

This project investigates semantic ambiguity in trademark goods descriptions at the boundary between Nice Class 3 (cosmetics and cleaning preparations) and Nice Class 5 (pharmaceutical and medical products). Although these classes are legally distinct, they frequently overlap in terminology, creating uncertainty for applicants and examiners.

Using modern Natural Language Processing (NLP) techniques, this study examines whether semantic embeddings can support more consistent trademark classification by distinguishing clear cases from genuinely ambiguous ones.

The project combines supervised classification, unsupervised clustering, and semantic similarity analysis, and includes a Streamlit prototype deployed on Hugging Face Spaces.

Research Questions

To what extent do the semantic properties of trademark descriptions in Nice Class 3 and Class 5 overlap?

Can modern NLP models reliably distinguish between Class 3 and Class 5 despite their semantic similarity?

How can data-driven tools support examiners and applicants in navigating ambiguous class boundaries?

Data

Source: European Union Intellectual Property Office (EUIPO) trademark applications

Scope: Applications containing Nice Class 3, Class 5, or both

Unit of analysis: Trademark application (goods descriptions aggregated at application level)

Labels

3_only — only Class 3 goods

5_only — only Class 5 goods

both — goods from both classes

⚠️ Note: The full dataset is not publicly shared. The repository uses anonymised samples or reconstruction scripts for reproducibility.

Methods

The analysis pipeline includes:

Sentence-BERT (SBERT) for semantic text embeddings (multilingual)

Multinomial Logistic Regression for supervised classification

UMAP for dimensionality reduction and visualization

HDBSCAN for unsupervised clustering

Cosine similarity to quantify semantic proximity between classes

Manual validation of borderline cases

External validation using a large language model (LLM)
