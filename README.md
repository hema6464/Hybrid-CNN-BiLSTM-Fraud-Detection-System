🛡️ Hybrid CNN‑LSTM with Adaptive Sampling for Temporal Fraud Detection
📖 Overview
This project presents a Hybrid CNN‑LSTM architecture enhanced with an Adaptive Sampling Module (ASM) to detect temporal fraud patterns in UPI transaction data.
The model combines CNN for local motif extraction, Bi‑LSTM for long‑range temporal dependencies, and attention mechanisms to highlight critical time steps.

🎯 Objectives
Detect fraudulent transactions in UPI payment systems.

Handle class imbalance using adaptive sampling.

Improve robustness against concept drift in temporal data.

Achieve higher precision, recall, and F1 scores compared to baseline models.

🛠️ Methodology
CNN Front‑End: Extracts spatial features from transaction sequences.

Bi‑LSTM Layer: Captures temporal dependencies across sequences.

Attention Mechanism: Focuses on critical time steps for fraud detection.

Adaptive Sampling Module (ASM):

Computes informativeness score (anomaly, novelty, class weight).

Uses reservoir sampling with time decay.

Detects drift via KL divergence.

📊 Results
Outperformed baseline models (Random Forest, XGBoost, CNN, LSTM).

Achieved higher recall and AUPRC values.

Demonstrated resilience to concept drift in transaction streams.

⚙️ Implementation
Frameworks: PyTorch, TensorFlow

Hardware: GPU acceleration

Hyperparameters:

CNN filters: [64, 128, 256]

LSTM hidden size: 256

Batch size: 256

Learning rate: 1e‑3

Loss Function: Weighted focal loss
