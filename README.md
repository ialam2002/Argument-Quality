# Argument-Quality

This project focuses on training a RoBERTa model using PyTorch to assess the quality of arguments. The dataset used for this project is the IBM Debater (R) arg_quality_rank_30k.

## Overview
The aim of this project is to develop a model capable of evaluating the quality of arguments. This can be useful for various applications such as automated essay scoring, debate analysis, and enhancing educational tools.

## Dataset
The dataset used in this project is the `IBM Debater (R) arg_quality_rank_30k`. It contains arguments labeled with quality scores.

IBM_Debater_(R)_arg_quality_rank_30k: This dataset consists of arguments and their corresponding quality scores, which range between 0 and 1.

This dataset was obtained from IBM debator argument mining datasets and is available under this [license][http://creativecommons.org/licenses/by-sa/3.0/].

## Model Architecture
We use the RoBERTa model, a robustly optimized BERT pretraining approach, as the foundation for our argument quality assessment model. RoBERTa's effectiveness in various NLP tasks makes it an excellent choice for this project.

## Training
The model was trained using PyTorch. Key training details include:

- Optimizer: AdamW
- Learning Rate: 2e-5
- Batch Size: 16
- Epochs: 3
  
We fine-tuned the pre-trained RoBERTa model on our dataset to specialize it for argument quality assessment.

Evaluation
The model's performance was evaluated using metrics such as Mean Squared Error (MSE) and R-squared (R²) to gauge how well it predicts argument quality.
