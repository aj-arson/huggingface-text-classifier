---
library_name: transformers
license: apache-2.0
base_model: distilbert/distilbert-base-uncased
tags:
- generated_from_trainer
metrics:
- accuracy
model-index:
- name: food_v_not_food-distil-bert-text-classifier
  results: []
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# food_v_not_food-distil-bert-text-classifier

This model is a fine-tuned version of [distilbert/distilbert-base-uncased](https://huggingface.co/distilbert/distilbert-base-uncased) on an unknown dataset.
It achieves the following results on the evaluation set:
- Loss: 0.0015
- Accuracy: 1.0

## Model description

More information needed

## Intended uses & limitations

More information needed

## Training and evaluation data

More information needed

## Training procedure

### Training hyperparameters

The following hyperparameters were used during training:
- learning_rate: 0.0001
- train_batch_size: 64
- eval_batch_size: 64
- seed: 42
- optimizer: Use OptimizerNames.ADAMW_TORCH_FUSED with betas=(0.9,0.999) and epsilon=1e-08 and optimizer_args=No additional optimizer arguments
- lr_scheduler_type: linear
- num_epochs: 10

### Training results

| Training Loss | Epoch | Step | Validation Loss | Accuracy |
|:-------------:|:-----:|:----:|:---------------:|:--------:|
| 0.4492        | 1.0   | 4    | 0.1381          | 0.98     |
| 0.0845        | 2.0   | 8    | 0.0229          | 1.0      |
| 0.0168        | 3.0   | 12   | 0.0082          | 1.0      |
| 0.0071        | 4.0   | 16   | 0.0044          | 1.0      |
| 0.0040        | 5.0   | 20   | 0.0029          | 1.0      |
| 0.0029        | 6.0   | 24   | 0.0022          | 1.0      |
| 0.0024        | 7.0   | 28   | 0.0018          | 1.0      |
| 0.0019        | 8.0   | 32   | 0.0016          | 1.0      |
| 0.0019        | 9.0   | 36   | 0.0015          | 1.0      |
| 0.0017        | 10.0  | 40   | 0.0015          | 1.0      |


### Framework versions

- Transformers 5.20.1
- Pytorch 2.14.1+cu130
- Datasets 5.1.0
- Tokenizers 0.23.3
