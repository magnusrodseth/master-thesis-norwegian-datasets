# Norwegian Financial NLP Datasets

[![License: CC BY-NC-SA 3.0](https://img.shields.io/badge/License-CC_BY--NC--SA_3.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/3.0/)

## Description

This repository hosts datasets developed for research into simplifying Norwegian financial information using Artificial Intelligence (AI) and Natural Language Processing (NLP). It includes a Norwegian translation of the widely used [Financial PhraseBank dataset](https://huggingface.co/datasets/takala/financial_phrasebank) and a manually curated Native Norwegian Financial Benchmark (NNFB) dataset.

## Background

The financial domain presents unique challenges for NLP due to its specialized terminology and the need for high accuracy. While many resources exist for English, there is a comparative lack of accessible, high-quality datasets specifically for the Norwegian financial sector. This repository aims to provide valuable resources for researchers and practitioners working on NLP tasks such as sentiment analysis, text classification, and language model training within the Norwegian financial context.

These datasets were compiled as part of a master's thesis project at the Norwegian University of Science and Technology (NTNU).

## Datasets

This repository contains two main datasets:

### 1. Translated Financial PhraseBank (FPB-NO)

- **Location:** [`financial_phrasebank/data.csv`](/financial_phrasebank/data.csv)

- **Description:** This dataset is a Norwegian translation of the English [Financial PhraseBank](https://huggingface.co/datasets/takala/financial_phrasebank) dataset created by Malo et al. (2014). The original dataset consists of sentences from English financial news, annotated by finance and economics experts according to their sentiment (positive, negative, neutral). This version provides the Norwegian translation of those sentences alongside the original sentiment labels.

- **Purpose:** Primarily useful for training and evaluating sentiment analysis models for Norwegian financial text.

- **Structure:** The `data.csv` file contains the following columns:

  - `english_sentence`: The original English sentence from the Financial PhraseBank.
  - `norwegian_sentence`: The Norwegian translation of the sentence.
  - `label`: The sentiment label assigned in the original Financial PhraseBank (0 for negative, 1 for neutral, 2 for positive).

- **License Note:** This dataset is an adaptation (translation) of the original Financial PhraseBank.

  - **Original work:** Malo, P., Sinha, A., Korhonen, P., Wallenius, J., & Takala, P. (2014). Good debt or bad debt: Detecting semantic orientations in economic texts. _Journal of the Association for Information Science and Technology_, _65_(4), 782–796. <https://doi.org/10.1002/asi.23062>
  - **Original Dataset Source:** Available on Hugging Face: <https://huggingface.co/datasets/takala/financial_phrasebank>
  - **License:** This adapted work is licensed under [CC BY-NC-SA 3.0](https://creativecommons.org/licenses/by-nc-sa/3.0/), the same license as the original, as required by the ShareAlike term. Please ensure you comply with all terms of this license if you use or adapt this translated dataset further.

### 2. Native Norwegian Financial Benchmark (NNFB)

- **Location:** [`native_norwegian_financial_benchmark/data.csv`](/native_norwegian_financial_benchmark/data.csv)

- **Description:** This dataset consists of 100 financial statements from [Dagens Næringsliv](https://www.dn.no/). It aims to provide a benchmark dataset composed of authentic Norwegian financial language.

- **Structure:** The `data.csv` file contains the following columns:

  - `sentence`: The financial statement or sentence.
  - `sentiment`: The sentiment label (0 for negative, 1 for neutral, 2 for positive).

- **License Note:** This dataset is also distributed under the CC BY-NC-SA 3.0 license.

## Licensing

The contents of this repository, including both datasets, are licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 3.0 Unported ([CC BY-NC-SA 3.0](https://creativecommons.org/licenses/by-nc-sa/3.0/)) license. You can find the full license text in the LICENSE file in this repository.

## Developer Information

**Developed By:** Magnus Rødseth and Jørgen Johannesen.
**Affiliation:** Norwegian University of Science and Technology (NTNU).
