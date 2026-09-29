# research-reproducability

This is a personal learning project where I reproduce machine learning research papers as runnable Jupyter
notebooks, targeting Google Colab. The goal is to build intuition for ML research by re-implementing the core
ideas, models, and experiments from published papers, rather than just reading about them.

## Disclaimer

The papers in [`research-papers/`](research-papers/) are copies of publicly available publications, downloaded
from free, open-access sources such as [arXiv](https://arxiv.org/). **I am not the author or owner of any of
this research.** All credit for the papers themselves belongs entirely to their original authors.

This repository exists purely as a practice manual for me to learn machine learning by reproducing published
results. The code here is my own independent reimplementation, written for educational purposes, and any
reproduction is a small-scale approximation of the original work (see each paper's folder for exactly what was
scaled down and why) — not an official or authoritative replication.

## Convention

Each paper gets its own folder at the repo root, named as a kebab-case slug of the paper title
(e.g. `on-calibration-of-modern-neural-networks/`), containing:

- `reproduction.ipynb` — the notebook itself.
- `README.md` — what's reproduced, what's scaled down vs. the paper and why, and how to run it.

## Papers

- [`on-calibration-of-modern-neural-networks/`](on-calibration-of-modern-neural-networks/) — Guo et al.,
  *On Calibration of Modern Neural Networks* (ICML 2017).
