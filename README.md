# _Nesciun Lengaz Lascià Endò_: Machine Translation for Fassa Ladin

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

This repository contains code and data associated with the CLiC-it 2024 paper:

Giovanni Valer, Nicolò Penzo and Jacopo Staiano. 2024. **Nesciun Lengaz Lascià Endò: Machine Translation for Fassa Ladin**. In _Proceedings of the Tenth Italian Conference on Computational Linguistics_, Pisa, Italy. [[cite]](#citation) [[paper]](https://clic2024.ilc.cnr.it/wp-content/uploads/2024/12/104_main_long.pdf)

## Overview
- [Introduction](#introduction)
- [Data](#data)
- [Experiments](#experiments)
  - [Preliminary Experiments](#preliminary-experiments)
  - [Finetuning](#finetuning)
  - [Evaluation](#evaluation) (with Transfer learning across domains and Forgetting of previous knowledge)

## Introduction
We built the first Fassa Ladin-Italian-English parallel corpus, and trained a machine translation model on it.

### 🔥 English → Ladin demo
You can try translating text from **English**/**Italian** to **Fassa Ladin** using the model [on Hugging Face Spaces](https://huggingface.co/spaces/jo-valer/fassa-ladin-machine-translation) 🦀


## Data
The dataset draws from multiple resources in 5 different domains: literature, news, games, laws, and brochures. It is available in the [`data`](https://github.com/jo-valer/machine-translation-ladin-fascian/tree/main/data) directory, either as a single file or split into train, validation, in-domain test, and out-of-domain test sets.

## Experiments

### Preliminary Experiments

<a target="_blank" href="https://colab.research.google.com/github/jo-valer/machine-translation-ladin-fascian/blob/main/preliminary.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

Evaluate the performance of the pre-trained models.

### Finetuning
<a target="_blank" href="https://colab.research.google.com/github/jo-valer/machine-translation-ladin-fascian/blob/main/finetune.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

Fine-tune the pre-trained models on the Fassa Ladin-Italian-English parallel corpus, with the two approaches: **Multilingual translation** and **_Zero-shot_ Pivot-based transfer learning**.

### Evaluation
<a target="_blank" href="https://colab.research.google.com/github/jo-valer/machine-translation-ladin-fascian/blob/main/evaluate.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

Evaluate the models' **performance**, investigate **Transfer learning across domains**, and **Forgetting of previous knowledge**.

## Citation
If you use or build on top of this work, please cite our paper as follows:

```
@inproceedings{valer-etal-2024-nesciun,
    title={Nesciun Lengaz Lascià Endò: {M}achine Translation for {F}assa {L}adin},
    author={Valer, Giovanni and Penzo, Nicolò and Staiano, Jacopo},
    booktitle={Proceedings of the 10th Italian Conference on Computational Linguistics},
    publisher={CEUR-ws.org},
    year={2024},
    month={december},
    address={Pisa, Italy}
}
```
