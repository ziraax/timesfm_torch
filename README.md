# timesfm_torch

This notebook attend to replicate the model presented in the paper : 

[A DECODER-ONLY FOUNDATION MODEL FOR TIME-SERIES FORECASTING](https://arxiv.org/pdf/2310.10688) 

from **Google Research** using **Pytorch**. Note that everything here is granted as-is, and without any guarantee. 

I'm trying to follow this architecture :

```
  Input Time-Series Data
     ↓
  Patch Extraction (Patches of fixed size)
     ↓
  Embedding Layer (Transforms patches into vectors)
     ↓
  Residual Block (Stabilizes and enhances embeddings)
     ↓
  Stacked Transformer Layers (N layers)
     ↓
     └─ Multi-Head Self-Attention (Captures dependencies across patches)
     ↓
     └─ Feed-Forward Network (Processes each patch independently)
     ↓
     └─ Residual Connections & Layer Normalization (Stabilizes training)
     ↓
  Output Prediction Layer (Maps transformer outputs to predicted values)
     ↓
  Predicted Time-Series Values
```

This repo welcomes any PR, issues, etc, as I'm still fairly new to Pytorch and happy to learn!
