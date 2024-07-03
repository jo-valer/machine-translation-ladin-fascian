# Machine Translation for Fassa Ladin

## Overview
This repo contains my final project for _Applied Natural Language Processing_ (University of Trento, a.y. 2023/24).

- [Introduction](#introduction)
- [Data](#data)
- [Experiments](#experiments)
  - [Preliminary Experiments](#preliminary-experiments)
  - [Transfer Learning Experiments](#training)
  - [Transfer Learning Across Domains](#evaluation)

## Introduction
I construct the first Fassa Ladin-Italian-English parallel corpus, and train a machine translation model on it. More information can be found in the accompanying report.

### 🛠 English → Ladin demo
You can try translating text from **English**/**Italian** to **Fassa Ladin** using the model [on Hugging Spaces](https://huggingface.co/spaces/jo-valer/fassa-ladin-machine-translation) 🦀


## Data
The dataset draws from multiple resources in 5 different domains: literature, news, games, laws, and brochures. It is available in the [`data`](https://github.com/jo-valer/machine-translation-ladin-fascian/tree/main/data) directory, either as a single file or split into train, validation, in-domain test, and out-of-domain test sets.

## Experiments

### Preliminary Experiments

<a target="_blank" href="https://colab.research.google.com/github/jo-valer/machine-translation-ladin-fascian/blob/main/preliminary.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

Evaluate the performance of the pre-trained models.

### Training
<a target="_blank" href="https://colab.research.google.com/github/jo-valer/machine-translation-ladin-fascian/blob/main/finetune.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

Fine-tune the pre-trained models on the Fassa Ladin-Italian-English parallel corpus, with the two approaches: **Pivot-based transfer learning** and **Multilingual translation**.

### Evaluation
<a target="_blank" href="https://colab.research.google.com/github/jo-valer/machine-translation-ladin-fascian/blob/main/evaluate.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

Evaluate the models' **performance**, investigate **Transfer learning across domains**, and **Forgetting of previous knowledge**.
