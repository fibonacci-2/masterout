### Cross-Lingual Transfer Learning for Mental Health Applications

This is the repository for our group project for the course CSCI 6907 "NLP for Health" Fall 2025 at the George Washington University.

---

## Members

chqiu@gwu.edu  
(TODO: Put emails of others here) 

---

## Introduction

This project focuses on cross-lingual transfer learning for mental health prediction tasks, specifically examining how knowledge transfers from large English mental health datasets to smaller datasets in low-resource languages such as Russian and Arabic.  
The research addresses the critical need for multilingual mental health screening tools that overcome language barriers and offer culturally sensitive support across diverse linguistic communities.  
We focus on Large Language Models for their well-established ability to capture linguistic patterns at scale.  
We employ finetuning (E1) and prompting (E2) on two datasets, D1 and D2, in Arabic and Russian respectively, with an intermediary large English corpus from which we transfer knowledge.  
We curated all datasets from social media due to availability of annotated samples.  
Our results highlight the difficulty of transferring mental health knowledge from English to Arabic, which we attribute to Arabic cultural context and mental health stigma that shape unique linguistic expressions.  
More specifically, transferring knowledge through finetuning achieves higher recall on a binary classification task but lower accuracy, maintaining the same F1 as the baseline.  
For English-to-Russian transfer learning, we observe better knowledge transfer through prompting on the same binary classification task, achieving stronger performance from transfer learning than from the baseline. 

---

## Dataset & Model

The dataset and models are located at https://drive.google.com/file/d/1KUVHGOP6vEaYAt9usv-BDLccSeP6lCHW/view?usp=share_link, this is a private link so you need to request for permission as a member of the class to access it.
