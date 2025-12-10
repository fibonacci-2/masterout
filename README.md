### Cross-Lingual Transfer Learning for Mental Health Applications

This is the repository for our group project for the course CSCI 6907 "NLP for Health" Fall 2025 at the George Washington University.

---

## Members

javidalakbarli@gwmail.gwu.edu ([Javid Alakbarli](https://github.com/1javid))
- contribution in branch [Javid](https://github.com/fibonacci-2/masterout/tree/Javid?tab=readme-ov-file)

saadm@gwmail.gwu.edu ([fibonacci-2](https://github.com/fibonacci-2))  
chqiu@gwmail.gwu.edu ([AmCh-Q](https://github.com/AmCh-Q))  
nikitaravi@gwmail.gwu.edu ([Nikita Ravi](https://github.com/nikita-ravi))  

---

## Introduction

This project focuses on cross-lingual transfer learning for mental health prediction tasks, specifically examining how knowledge transfers from large English mental health datasets to smaller datasets in low-resource languages such as Russian and Arabic.  
The research addresses the critical need for multilingual mental health screening tools that overcome language barriers and offer culturally sensitive support across diverse linguistic communities.  
We focus on Large Language Models for their well-established ability to capture linguistic patterns at scale.  
We employ finetuning (E1) and prompting (E2) on two datasets, D1 and D2, in Arabic and Russian, respectively, with an intermediary large English corpus from which we transfer knowledge.  
We curated all datasets from social media due to the availability of annotated samples.  
Our results highlight the difficulty of transferring mental health knowledge from English to Arabic, which we attribute to the cultural context of Arabic and the stigma of mental health that shape unique linguistic expressions.  
More specifically, transferring knowledge through finetuning achieves higher recall on a binary classification task but lower accuracy, maintaining the same F-1 score as the baseline.  
For English-to-Russian transfer learning, we observe better knowledge transfer by prompting on the same binary classification task, achieving stronger performance from transfer learning than from the baseline.  

---

## Dataset & Model

The dataset and models are located [here](https://drive.google.com/file/d/1KUVHGOP6vEaYAt9usv-BDLccSeP6lCHW/view?usp=share_link), this is a private link so you need to request for permission as a member of the class to access it.

## Running the notebooks

The notebook file "NLP4Health_Local.ipynb" is intended to be run locally while others are run on Google Colab.  
The local version is run on 4x NVIDIA RTX 6000 Ada, but would likely be able to run on much lighter hardware.  
The Colab Notebooks are run using NVIDIA A100 which requires a paid subscription.  
