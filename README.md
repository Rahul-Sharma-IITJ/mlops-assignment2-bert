# MLOps Assignment 2 — Fine-Tuning BERT for Book Genre Classification

**IIT Jodhpur | PGD AI Program | MLOps**

## Overview

This project builds a complete MLOps pipeline: fine-tune a DistilBERT model on Goodreads book reviews to predict genre, track experiments with Weights & Biases, and publish the model to Hugging Face Hub.

## Model

**DistilBERT** (`distilbert-base-cased`) was chosen for this assignment because it is 40% smaller and 60% faster than full BERT while retaining 97% of its language understanding ability. This makes it ideal for classification tasks on limited compute. The model was fine-tuned on the [UCSD Goodreads dataset](https://mengtingwan.github.io/data/goodreads.html) to classify reviews into 8 genres: poetry, children, comics & graphic, fantasy & paranormal, history & biography, mystery/thriller/crime, romance, and young adult.

## Setup Instructions

```bash
# 1. Clone this repo
git clone https://github.com/Rahul-Sharma-IITJ/mlops-assignment2-bert
cd mlops-assignment2-bert

# 2. Install dependencies
pip install -r requirements.txt

# 3. Set environment variables
export WANDB_API_KEY=your_wandb_key
export HF_TOKEN=your_hf_token
```

Then open and run the notebook end-to-end on Kaggle (with GPU T4 enabled).

## Training Platform

Training was done on **Kaggle Notebooks** with free GPU (T4 x2).  
Kaggle Notebook: https://www.kaggle.com/code/rahulsharma2144/notebook116d013c39

## Results

| Metric     | Score |
|------------|-------|
| Accuracy   | 0.60062  |
| F1 Score   | 0.60159  |
| Eval Loss  | 2.25133  |


## Links

- 🤗 Hugging Face Model: https://huggingface.co/g25ait2144/distilbert-goodreads-genres
- 📊 W&B Dashboard: https://wandb.ai/g25ait2144/mlops-assignment2
- 📓 Kaggle Notebook: https://www.kaggle.com/code/rahulsharma2144/notebook116d013c39
