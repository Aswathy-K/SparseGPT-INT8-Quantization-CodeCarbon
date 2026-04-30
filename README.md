# SparseGPT-INT8-Quantization-CodeCarbon
This notebook implements:  SparseGPT (Frantar &amp; Alistarh, 2023) — Hessian-guided one-shot pruning INT8 Quantization — post-pruning absmax symmetric quantization CodeCarbon — CO₂ emission tracking for each pipeline phase

**Results**
======================================================================
  Stage                               PPL   Mem (MB)     CO₂ (mg)
======================================================================
  Baseline (dense fp16)              5.03       2098       0.0000
  SparseGPT 50% sparse               5.07       2098     687.6209
  SparseGPT 50% + INT8               5.19       1049      11.9056
======================================================================
  SparseGPT 50% sparse            PPL Δ: +0.9%  Mem: 100% of baseline
  SparseGPT 50% + INT8            PPL Δ: +3.1%  Mem: 50% of baseline
