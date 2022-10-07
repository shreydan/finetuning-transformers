# finetuning-transformers

- **`bert-base-uncased` : part of feedback prize 3.0 kaggle competition**
  - huggingface pretrained autoModel and autoTokenizer
  - from scratch pytorch trainer
  - optimizer with weight decay as recommended by huggingface
  - unfreezed encoder block: full finetuning
  - multiple scheduler support: CosineAnnealingWarmRestarts, StepLR, ReduceLROnPlateau
  - GPU Memory consumption on average (with dataset): 12.6 GB

- **`deBERTa-v3-base`: part of feedback prize 3.0 kaggle competition**
  - huggingface pretrained autoModel and autoTokenizer
  - scratch pytorch trainer + huggingface accelerate
  - freezed base_model
  - pooler: mean-pooling
  - scheduler: CosineAnnealingWarmRestarts
  - optimization to improve training: Gradient Accumulation [steps=2]
