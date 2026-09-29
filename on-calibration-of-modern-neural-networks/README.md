# On Calibration of Modern Neural Networks

Reproduction of: Guo, Pleiss, Sun, Weinberger. *On Calibration of Modern Neural Networks.* ICML 2017.
[arXiv:1706.04599](https://arxiv.org/abs/1706.04599) · source PDF: `../research-papers/CalibrationOfModernNeuralNetwork.pdf`

## Contents

- `reproduction.ipynb` — the reproduction notebook. Designed to run on **Google Colab with a GPU runtime**
  (Runtime → Change runtime type → GPU). Total runtime: roughly 15–25 minutes.

## Scope

This is a **small-scale reproduction**, not a full replication of every table/figure in the paper. It trains two
models from scratch on CIFAR-100 — a shallow 5-layer ConvNet and a 56-layer ResNet — to reproduce the paper's
central finding:

- Higher-capacity networks are more accurate but more miscalibrated (Figure 1).
- Temperature scaling (a single learned scalar, Eq. 9) substantially reduces calibration error without
  changing accuracy (Section 4.2, Table 1, Figure 4).
- Histogram binning (Eq. 7) is implemented as a second, simplified calibration baseline for comparison.

The notebook itself documents, in a comparison table, exactly what's scaled down relative to the paper (fewer
datasets, shallower/fewer models, fewer training epochs) and why. An optional, compute-heavier appendix cell
reproduces the depth-vs-ECE trend from Figure 2, off by default.

## How to run

1. Open `reproduction.ipynb` in Google Colab (upload it, or open from GitHub/Drive if this repo is synced there).
2. Set the runtime to GPU.
3. Run all cells top to bottom.

It can also run locally (CPU/MPS/CUDA) with `torch`, `torchvision`, `matplotlib`, `pandas`, and `numpy` installed,
but will be much slower on CPU.
