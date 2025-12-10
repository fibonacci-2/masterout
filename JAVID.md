# Depression Detection in English and Russian Text

This repository contains machine learning models for depression detection in English and Russian text using transformer-based approaches with fine-tuning and transfer learning techniques.

## Project Structure

```
masterout/
├── english-depression/
│   └── english-depression.ipynb    # Baseline English depression classification model
├── russian-depression/
│   ├── russian-baseline.ipynb      # Baseline Russian depression model
│   └── english-russian-tl.ipynb    # Transfer learning from English to Russian
...                    
```

## Contributions

### English Depression Detection

**Location:** `english-depression/english-depression.ipynb`

This notebook implements a baseline model for detecting depression in English text using:

- **Model Architecture:** XLM-RoBERTa-base with LoRA (Low-Rank Adaptation) fine-tuning
- **Dataset:** Preprocessed English depression datasets from Reddit
- **Training Approach:** 
  - Parameter-efficient fine-tuning using LoRA adapters
  - Binary classification (depression vs. control)
  - Train/validation/test split (70%/15%/15%)

**Resources:**
- Datasets, checkpoints, and results: [Google Drive - English Depression](https://drive.google.com/drive/folders/1zo9Ajyg1-NiEiWEdJsZ5uo9w45_vZTXq?usp=sharing)

### Russian Depression Detection

**Location:** `russian-depression/`

#### 1. Baseline Model
**File:** `russian-baseline.ipynb`

Baseline Russian depression model:

- **Model Architecture:** XLM-RoBERTa-base with LoRA fine-tuning
- **Training Configuration:**
  - Class weight balancing for imbalanced datasets
  - Evaluation on validation and test sets
- **Performance Tracking:** Integration with Weights & Biases (wandb) for experiment tracking

#### 2. Transfer Learning Model
**File:** `english-russian-tl.ipynb`

Transfer learning English to Russian:

- **Transfer Learning Strategy:**
  1. Load pre-trained English depression model (trained on English data)
  2. Fine-tune on Russian dataset using the English model as initialization
  3. Compare performance with baseline Russian-only model
- **Key Features:**
  - Few-shot learning experiments with varying training set sizes
  - Full-shot training using the complete Russian dataset
  - Cross-lingual knowledge transfer evaluation
  - Performance comparison between baseline and transfer learning approaches

**Resources:**
- Datasets, checkpoints, and results: [Google Drive - Russian Depression](https://drive.google.com/drive/folders/1lXoaFw_fns5t92XmJSs1tLgntbu9Rs9m?usp=sharing)

## Datasets

The datasets used in this project are stored in the Google Drive folders linked above. The datasets include:

- Preprocessed and tokenized text data
- Labeled examples (depression vs. control)
- Train/validation/test splits
- Additional metadata (age, text length, word count, etc.)