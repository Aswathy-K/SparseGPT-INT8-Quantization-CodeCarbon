# SparseGPT-INT8-Quantization-CodeCarbon
This notebook implements:  SparseGPT (Frantar &amp; Alistarh, 2023) — Hessian-guided one-shot pruning INT8 Quantization — post-pruning absmax symmetric quantization CodeCarbon — CO₂ emission tracking for each pipeline phase

**Results**

Using T4 GPU
Stage 	PPL	Mem (MB) 	CO₂ (mg) 
Baseline (dense fp16) 	5.03	2098	0
SparseGPT 50% sparse 	5.07	2098	687.6209
SparseGPT 50% + INT8 	5.19	1049	11.9056
SparseGPT 50% sparse 	PPL Δ: +0.9% 	Mem: 100% of baseline 	
SparseGPT 50% + INT8 	PPL Δ: +3.1% 	Mem: 50% of baseline 	
<img width="427" height="222" alt="image" src="https://github.com/user-attachments/assets/89e12497-f168-45bf-bf8e-7bb5cbb95e20" />

Using TPU v5e
Stage 	PPL 	Mem (MB) 	CO₂ (mg) 
Baseline (dense fp16) 	5.03	4196	0
SparseGPT 50% sparse 	5.08	4196	7843.6195
SparseGPT 50% + INT8 	5.19	1049	69.3847
SparseGPT 50% sparse 	PPL Δ: +1.0% 	Mem: 100% of baseline 	
SparseGPT 50% + INT8 	PPL Δ: +3.2% 	Mem: 25% of baseline 	
<img width="427" height="222" alt="image" src="https://github.com/user-attachments/assets/5f21d814-0dc8-419f-977d-de8e2bd50fba" />
