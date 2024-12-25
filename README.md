# Multi-Modal Summarization for Scientific Papers

## Overview
This repository contains the implementation and results of the project titled **Multi-Modal Summarization for Scientific Papers**. The project investigates an innovative multi-modal approach for summarizing scientific articles by integrating textual and visual data (e.g., figures, tables, and images) using a Retrieval-Augmented Generation (RAG) framework. The goal is to improve the quality and informativeness of summaries.

## Features
- **Text and Image Integration**: Combines textual and visual data to produce enriched summaries.
- **Multi-Vector Retrieval**: Efficiently stores and retrieves content using vector databases.
- **Evaluation Metrics**: Implements ROUGE and BERT scores for performance evaluation.
- **Experiments**:
  - Summarization using text only.
  - Summarization using both text and image data.

## Contents
- [Introduction](#introduction)
- [Methodology](#methodology)
- [Experiments](#experiments)
- [Results](#results)
- [Limitations and Future Work](#limitations-and-future-work)
- [References](#references)

---

## Introduction
The growing number of scientific articles requires advanced summarization techniques to assist researchers in efficiently understanding key information without reading full articles. This project explores how the integration of textual and visual elements improves summary quality.

Key highlights:
- Enhanced retrieval and usability of information.
- Applications in academic research, business intelligence, and education.

### Research Questions
1. How does integrating textual and visual data improve the quality of summarization?
2. Can multi-modal summarization provide richer, more contextually accurate summaries?

---

## Methodology
1. **Data Collection**:
   - Extract text and visual content from scientific PDFs using the `unstructured` package.
   - Convert images and tables into text summaries via GPT-4o-mini.

2. **Data Processing**:
   - Utilize semantic chunking to slice documents into meaningful fragments.
   - Store processed data in a vector database for efficient retrieval.

3. **Summarization**:
   - Generate summaries for text and images using language models such as GPT-4o-mini and Mistral-Large-Latest.

4. **Evaluation**:
   - Use ROUGE and BERT scores to assess summarization quality.

---

## Experiments
### Experiment 1: Text-Only Summarization
- Input: Textual embeddings.
- Output: Summaries generated using GPT-4o-mini and Mistral-Large-Latest.
- Key Metrics: ROUGE-1, ROUGE-2, ROUGE-L, and BERT scores.

### Experiment 2: Multi-Modal Summarization
- Input: Combined textual and visual data.
- Output: Enriched summaries with added contextual depth.
- Observations: Integration of images increased summary length but showed mixed results in standard evaluation metrics.

---

## Results
- **ROUGE and BERT Scores**:
  - GPT-4o-mini excelled in semantic similarity.
  - Mistral-Large-Latest showed better recall.
- **Impact of Visual Data**:
  - Enhanced context but introduced noise in evaluation metrics when abstracts were used as reference summaries.

---

## Limitations and Future Work
### Limitations
1. Over-reliance on abstracts for evaluation may underestimate model performance.
2. Standard metrics (ROUGE, BERT) are text-driven and do not fully capture the qualitative value of image-inclusive summaries.
3. Errors in text and image extraction may introduce inconsistencies.
4. Lack of human evaluation limits insights into readability and real-world applicability.

### Future Work
- Conduct large-scale evaluations with 100+ articles.
- Incorporate human feedback for qualitative assessment.
- Expand the framework to support other media types, such as video and audio.

---

## References
This project references multiple works on text summarization, multi-modal approaches, and evaluation metrics. For detailed citations, refer to the [project report](https://github.com/Fardeen210/Text-Summarization).

---

## Contact
**Fardeen Ali Mohammed**
- Email: [FardeenAliMohammed@my.unt.edu](mailto:FardeenAliMohammed@my.unt.edu)
- GitHub: [https://github.com/Fardeen210/Text-Summarization](https://github.com/Fardeen210/Text-Summarization)

