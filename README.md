# Natural Language Processing – CIMAT (Spring 2025)

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![PyTorch](https://img.shields.io/badge/PyTorch-✓-ee4c2c)
![TensorFlow](https://img.shields.io/badge/TensorFlow-✓-ff6f00)
![Neural Networks](https://img.shields.io/badge/Neural%20Networks-✓-hotpink)
![Transformers](https://img.shields.io/badge/Transformers-✓-mediumvioletred)

**Author:** Ezau Faridh Torres Torres  
**Advisor:** Dr. Adrian Pastor López Monroy and Dr. Fernando Sanchez Vega  
**Course:** Natural Language Processing  
**Institution:** CIMAT – Centro de Investigación en Matemáticas  
**Term:** Spring 2025 

This repository contains all course assignments and the final project from the graduate-level class *Natural Language Processing* at CIMAT (Spring 2025). The course covered core techniques in modern NLP, from classical text preprocessing to deep learning-based models for classification and sequence labeling. The final project involved building a hierarchical multitask model for social media user profiling using Spanish-language Twitter data.

## 📄 Table of Contents

- [Repository Structure](#repository-structure)  
- [Technical Stack](#technical-stack)  
- [Datasets Used](#datasets-used)  
- [Overview of Assignments](#overview-of-assignments)  
  - [Assignment 1 – Corpus Construction and Preprocessing](#assignment-1--corpus-construction-and-preprocessing)  
  - [Assignment 2 – Basic Text Mining and SVM Classification](#assignment-2--basic-text-mining-and-svm-classification)  
  - [Assignment 3 – Feature Selection and Text Visualization](#assignment-3--feature-selection-and-text-visualization)  
  - [Assignment 4 – Language Modeling from Political Speeches](#assignment-4--language-modeling-from-political-speeches)  
  - [Assignment 5 – Neural Language Modeling](#assignment-5--neural-language-modeling)  
  - [Assignment 6 – Hierarchical Attention Network](#assignment-6--hierarchical-attention-network)  
  - [Final Project – Multimodal Meme Classification with CLIP and Textual Inversion](#final-project--multimodal-meme-classification-with-clip-and-textual-inversion)  
- [Tests](#tests)  
  - [Test 1 – Tourist Opinion Mining and Text Analytics](#test-1---tourist-opinion-mining-and-text-analytics)  
  - [Test 2 – Multitask Tweet Classification with RoBERTuito and TF-IDF](#test-2---multitask-tweet-classification-with-robertuito-and-tf-idf)  
- [Learning Outcomes](#learning-outcomes)  
- [References](#references)  
- [Contact](#-contact)

---

## Repository Structure

Each assignment includes:

- A single `.ipynb` notebook with code and commentary
- Manually added visualizations or outputs within the notebook
- Optional supporting files (e.g., pretrained embeddings, tokenizers) 

---

## Technical Stack

Developed and tested in Python 3.11, using the following tools across assignments and tests:

- **NLP Libraries:** `nltk`, `spaCy`, `gensim`, `torchtext`, `pysentimiento`
- **Machine Learning & Deep Learning:** `scikit-learn`, `PyTorch`, `transformers`, `lightning`
- **Text Processing:** `re`, `collections`, `TweetTokenizer`, `emoji`, `ftfy`
- **Pretrained Models:** `GloVe`, `Word2Vec`, `bert-base-multilingual-cased`, `PlanTL-GOB-ES/roberta-base-bne`, `pysentimiento/robertuito-base-uncased`, `CLIP`
-	**Visualization:** `matplotlib`, `seaborn`, `wordcloud`, `t-SNE`, `attention heatmaps`, `confusion_matrix`, `word frequency histograms`
-	**Auxiliary:** `argparse`, `glob`, `json`, `numpy`, `os`, `pandas`, `random`, `scipy`, `tqdm`, `xml.etree.ElementTree`
- **Environment:** `Jupyter Notebook` (for interactive development)

> Note: Most notebooks are self-contained and reproducible, with controlled randomness when applicable.

---

## Datasets Used

- **Presidential Press Conferences** (Scraped): Official transcripts from amlo.presidente.gob.mx and gob.mx used in Assignments 1 and 4
- **MEX-A3T 2020 Subtask 1:** Spanish tweets for text classification tasks in Assignments 2–3 and 5
- **PAN Author Profiling (CLEF 2017):** Multilingual tweet-based dataset used in Assignment 6 for nationality classification
  - https://pan.webis.de/clef17/pan17-web/author-profiling.html
- **Hateful Memes Challenge & HarMeme:** Used in the final project
  - https://facebook.ai/hatefulmemes
  - https://huggingface.co/datasets/harmeme
 
---

## Overview of Assignments

The following section presents a concise overview of each task, highlighting its primary objective:

### Assignment 1 – Corpus Construction and Preprocessing 
  Automates the creation of a text corpus from presidential press conferences through web scraping and HTML parsing with `wget` and `BeautifulSoup`. The resulting plain-text files serve as a foundation for later NLP tasks and include basic error handling during extraction.

  <div align="center">
    <img src="https://github.com/ezautorres/Natural-Language-Processing-CIMAT/blob/main/images/a1.png" alt="Frequency of words" width="600"/>
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
    <img src="https://github.com/ezautorres/Natural-Language-Processing-CIMAT/blob/main/images/a6.png" alt="Training" width="800"/>
  </div>

---

### Final Project – Multimodal Meme Classification with CLIP and Textual Inversion  
  Implements the [ISSUES framework](https://arxiv.org/abs/2310.08368) for hateful meme classification by combining a frozen `CLIP` model with textual inversion techniques and a two-stage training strategy. The system disentangles visual and textual embeddings and fuses them via a Combiner network, achieving robust multimodal representations for classification.

  <div align="center">
    <img src="https://github.com/ezautorres/Natural-Language-Processing-CIMAT/blob/main/images/p.png" alt="Training" width="600"/>
  </div>

---

## Tests

### Test 1 - Tourist Opinion Mining and Text Analytics
  Applies text preprocessing, exploratory analysis, and feature selection techniques to thousands of tourist reviews from 10 landmarks in Guanajuato. Includes sentiment classification based on rating scores, frequency-based word filtering, and `TF-IDF + Chi²` for identifying discriminative terms across destinations.

  <div align="center">
    <img src="https://github.com/ezautorres/Natural-Language-Processing-CIMAT/blob/main/images/t1.png" alt="Review Evolution" width="600"/>
  </div>

### Test 2 - Multitask Tweet Classification with RoBERTuito and TF-IDF
  Implements a multitask neural pipeline for predicting both gender and nationality from Spanish-language tweets using RoBERTuito and TF-IDF features. The model is trained with joint loss, incorporates a Transformer-based encoder and sparse lexical features, and is evaluated using joint accuracy and F1 metrics across both tasks.

  <div align="center">
    <img src="https://github.com/ezautorres/Natural-Language-Processing-CIMAT/blob/main/images/t2.png" alt="Results" width="800"/>
  </div>

---

## Learning Outcomes

Through this course, I developed hands-on skills in:

- Constructing text classification pipelines with custom tokenization and feature extraction
- Training and evaluating classical models (Naive Bayes, SVMs) and neural models (BiGRU, Transformers, HAN)
- Designing hierarchical and multitask neural networks for user profiling
- Using attention mechanisms to interpret model behavior
- Applying pretrained multilingual embeddings and fine-tuning transformer-based encoders
- Implementing neural language models and evaluating them via perplexity and sentence likelihood
- Combining vision-language models (CLIP) with textual inversion for multimodal classification
- Writing reproducible research code and presenting results effectively with visualizations

---

## References

- Giovanni Burbi, Alberto Baldrati, Lorenzo Agnolucci, Marco Bertini, Alberto Del Bimbo.  
  *Mapping Memes to Words for Multimodal Hateful Meme Classification*.  
  arXiv:2310.08368, 2023.  
  https://arxiv.org/abs/2310.08368

---

## 📫 Contact

- 📧 Email: ezau.torres@cimat.mx  
- 💼 LinkedIn: [linkedin.com/in/ezautorres](https://linkedin.com/in/ezautorres)