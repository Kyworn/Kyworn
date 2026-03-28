# Zorko / Kyworn

Independent ML researcher. Building efficient LLMs for edge deployment.

## Projects

**PentaNet** — Native pentanary {-2,-1,0,+1,+2} quantization for LLMs  
−6.4% PPL vs BitNet at 124M params · 3 seeds · WikiText-103  
[Paper]([lien](https://github.com/Kyworn/PentaNet-v1.0/blob/main/paper/PentaNet_Technical_Report.pdf)) · [Code]([lien](https://github.com/Kyworn/PentaNet-v1.0)) · [Model]([lien](https://huggingface.co/Kyworn/pentanet-124m) HuggingFace)

**ShiftQuant** — Systematic analysis of shift-based PTQ on existing LLMs  
Proves no 7-value grid escapes the coverage/gap tradeoff · AWQ recovers 22%  
[Paper]([lien](https://github.com/Kyworn/ShiftQuant/blob/main/paper/shiftquant.pdf)) · [Code]([lien](https://github.com/Kyworn/ShiftQuant))

## Stack
PyTorch · Triton · AVX2 · WikiText-103 · RTX 5080
