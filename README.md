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
  Automates the creation of a text corpus from presidential press conferences through web scraping and HTML parsing with wget and ´BeautifulSoup´. The resulting plain-text files serve as a foundation for later NLP tasks and include basic error handling during extraction.

  <div align="center">
    <img src="https://github.com/ezautorres/Natural-Language-Processing-CIMAT/blob/main/images/a1.png" alt="Frequency of words" width="500"/>
  </div>

### Assignment 2 – Basic Text Mining and SVM Classification
  Explores the construction of ´Bag-of-Words´ and bigram-based representations for text classification, using custom tokenization, frequency-based filtering, and Support Vector Machines (SVM) to evaluate performance through precision, recall, and confusion matrices.

### Assignment 3 – Feature Selection and Text Visualization 
  Implements frequency-based feature selection and dimensionality reduction to improve text classification, alongside visualizations such as word clouds and t-SNE for lexical exploration and representation analysis.

### Assignment 4 – Language Modeling from Political Speeches 
  Builds sentence-level corpora from political transcripts and explores n-gram language models, evaluating their ability to generate coherent sequences and estimate sentence probabilities.

### Assignment 5 – Stochastic Simulation  
  Exploration of methods for sampling from distributions, including inverse transform sampling, linear congruential generators, and SciPy’s discrete random utilities. The assignment culminates with a full implementation of Adaptive Rejection Sampling (ARS), applied to simulate from Gamma(2,1), Normal, and Beta distributions with high accuracy.

  <div align="center">
    <img src="https://github.com/ezautorres/Scientific-Computing-CIMAT/raw/main/assignment5/results/ARS_gamma.png" alt="Gamma(2,1) distribution sampled via ARS" width="500"/>
  </div>

### Assignment 6 – MCMC: Metropolis-Hastings  
  Simulation of Bernoulli data and posterior inference for the parameter 𝞺 using Metropolis-Hastings. Two proposal distributions were implemented: a Beta prior-informed proposal and a truncated Normal centered at the current state. The task includes analysis of irreducibility and ergodicity, along with convergence behavior as sample size increases.

  <div align="center">
    <img src="https://github.com/ezautorres/Scientific-Computing-CIMAT/raw/main/assignment6/results/MS_normal.png" alt="Posterior sampling with Metropolis-Hastings" width="500"/>
  </div>

### Assignment 7 – Metropolis-Hastings in Multivariate Settings  
  Implementation of Metropolis-Hastings for bivariate and Gamma distributions, including random walk proposals and convergence diagnostics under different sample sizes and proposal variances.

  <div align="center">
    <img src="https://github.com/ezautorres/Scientific-Computing-CIMAT/raw/main/assignment7/results/ex1/trayectory_ex1.png" alt="Posterior over alpha and beta" width="500"/>
  </div>

### Assignment 8 – MCMC with Hybrid Kernels and Gibbs Sampling  
  Simulation from complex posteriors using hybrid Metropolis-Hastings and Gibbs samplers. Includes examples with bivariate normals, Weibull likelihoods, and hierarchical Poisson-Gamma models for nuclear pump failure data.

  <div align="center">
    <img src="https://github.com/ezautorres/Scientific-Computing-CIMAT/raw/main/assignment8/results/p0.85.png" alt="Posterior" width="500"/>
  </div>

---

### Final Project – Bayesian Inference for Weibull Parameters  
  Full Bayesian treatment of a Weibull likelihood using MCMC. Implements both standard Metropolis-Hastings and adaptive proposals for posterior sampling of 𝛼 and λ, with convergence diagnostics and posterior summaries for simulated datasets.

  <div align="center">
    <img src="https://github.com/ezautorres/Scientific-Computing-CIMAT/raw/main/final_project/results/trayectory_ex2.png" alt="Trayectory of alpha and lambda for Weibull model" width="500"/>
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