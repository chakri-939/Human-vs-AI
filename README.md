# Project Overview
The advent of advanced Large Language Models (LLMs) like GPT-3 and GPT-4 has made it increasingly difficult to distinguish between human-written and machine-generated text. This project aims to address challenges in content verification and academic integrity by developing a robust classification system.

## Dataset
1. We utilized the HC3 (Human ChatGPT Comparison Corpus) English dataset sourced from HuggingFace.
2. Total Samples: ~50,000 texts
3. Split: 43,780 Training / 4,864 Testing 
4. Balance: The dataset is balanced between Human and Machine labels (~24k each).

## Feature Engineering
1. Beyond raw text, we extracted linguistic and structural features to analyze statistical irregularities common in AI text:
2. Perplexity: Measures how well a probability model predicts a sample.
3. Burstiness: Identifies clustered appearances of words/phrases.
4. Readability Scores: Flesch-Kincaid and Gunning Fog index.
5. POS Tagging: Frequency distribution of Part-of-Speech tags.
5. Voice Detection: Analysis of active vs. passive voice usage.

## Tech Stack
1. Languages: Python
2. Deep Learning: PyTorch, Keras, TensorFlow
3. NLP: HuggingFace Transformers, NLTK, Spacy
4. Data Processing: Pandas, NumPy, Scikit-learn
5. Visualization: Matplotlib, Seaborn
