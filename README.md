# Natural Language Processing – CIMAT (Spring 2025)

**Author:** Ezau Faridh Torres Torres  
**Advisor:** Dr. Adrian Pastor López Monroy and Dr. Fernando Sanchez Vega  
**Course:** Natural Language Processing  
**Institution:** CIMAT – Centro de Investigación en Matemáticas  
**Term:** Spring 2025 

This repository contains all course assignments and the final project from the graduate-level class *Natural Language Processing* at CIMAT (Spring 2025). The course covered core techniques in modern NLP, ranging from classical text preprocessing to deep learning-based models for text classification and sequence labeling. The final project involved building a hierarchical multitask model for social media user profiling using real-world Spanish-language data.

## 📄 Table of Contents

- [Repository Structure](#repository-structure)
- [Technical Stack](#technical-stack)
- [Overview of Assignments](#overview-of-assignments)
- [Contact](#-contact)

---

## Repository Structure

Each assignment comprises the following elements:

- a
- a
- a  

---

## Technical Stack

This project was developed in Python 3.11 using:

- **Core libraries:** `numpy`, `scipy`, `matplotlib`, `pandas`
- **Symbolic computation:** `sympy`
- **Statistical modeling & distributions:** `scipy.stats`
- **Plotting & visualization:** `seaborn`, `matplotlib`
- **Jupyter Notebooks** (for prototyping)

> Note: Some assignments use pretrained embeddings like GloVe or Word2Vec. Others employ multilingual transformer models (e.g., bert-base-multilingual-cased or robertuito-base-bne).

---

## Datasets Used

- hola
- hola

---

## Overview of Assignments

The following section presents a concise overview of each task, highlighting its primary objective:

### Assignment 1 – Corpus Construction and Preprocessing 
  Automates the creation of a text corpus from presidential press conferences through web scraping and HTML parsing with `wget` and `BeautifulSoup`. The resulting plain-text files serve as a foundation for later NLP tasks and include basic error handling during extraction.

  <div align="center">
    <img src="https://github.com/ezautorres/Natural-Language-Processing-CIMAT/blob/main/images/a1.png" alt="Frequency of words" width="500"/>
  </div>

### Assignment 2 – Basic Text Mining and SVM Classification
  Explores the construction of `Bag-of-Words` and bigram-based representations for text classification, using custom tokenization, frequency-based filtering, and Support Vector Machines (SVM) to evaluate performance through precision, recall, and confusion matrices.

### Assignment 3 – Feature Selection and Text Visualization 
  Implements frequency-based feature selection and dimensionality reduction to improve text classification, alongside visualizations such as word clouds and `t-SNE` for lexical exploration and representation analysis.

### Assignment 4 – Language Modeling from Political Speeches 
  Builds sentence-level corpora from political transcripts and explores n-gram language models, evaluating their ability to generate coherent sequences and estimate sentence probabilities.

### Assignment 5 – Neural Language Modeling  
  Implements a word-level neural language model using pretrained embeddings, trained on short tweet sequences. Includes nearest neighbor queries in embedding space, text generation, sentence likelihood estimation, and perplexity comparisons against probabilistic baselines.

### Assignment 6 – Hierarchical Attention Network  
  Trains a hierarchical neural model with word- and tweet-level attention mechanisms for user profiling based on multilingual tweet sequences. Evaluates model performance using F1-score and interprets attention weights for qualitative analysis.

  <div align="center">
    <img src="https://github.com/ezautorres/Natural-Language-Processing-CIMAT/blob/main/images/a6.png" alt="Training" width="500"/>
  </div>

---

### Final Project – Multimodal Meme Classification with CLIP and Textual Inversion  
  Implements the ISSUES framework for hateful meme classification by combining a frozen CLIP model with textual inversion techniques and a two-stage training strategy. The system disentangles visual and textual embeddings and fuses them via a Combiner network, achieving robust multimodal representations for classification.

  <div align="center">
    <img src="https://github.com/ezautorres/Natural-Language-Processing-CIMAT/blob/main/images/p.png" alt="Training" width="500"/>
  </div>
  
---

## Learning Outcomes

Throughout the course, I gained practical experience in:

- Implementing numerical linear algebra algorithms from scratch
- Performing polynomial and spline interpolation
- Solving ordinary differential equations using numerical schemes
- Designing and evaluating stochastic simulation pipelines (e.g., ARS, MCMC)
- Analyzing convergence and stability in numerical methods
- Applying Bayesian inference via MCMC techniques to real data
- Writing clear scientific reports with integrated visualizations

---

## 📫 Contact

- 📧 Email: ezau.torres@cimat.mx  
- 💼 LinkedIn: [linkedin.com/in/ezautorres](https://linkedin.com/in/ezautorres)