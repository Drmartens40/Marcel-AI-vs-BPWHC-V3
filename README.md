# Marcel: Asymmetric Behavior in Hybrid Actor-Critic Architectures

This repository presents the experimental results and analysis of *Marcel*, a custom hybrid reinforcement learning agent on BipedalWalkerHardcore-V3 environment. The project explores seed sensitivity and reward convergence in continuous control tasks using two distinct training initializations (40090 and 202507). It is designed for transparency in reproducible deep RL research without disclosing implementation details.
Results are overpassed all expected.

## 📌 Overview

- **Agent Name**: Marcel
- **Type**: Hybrid Actor-Critic
- **Framework**: Custom modules (F, B, P, M)
- **Curriculum Learning**: 1,000 episodes pre-train
- **Evaluation**: 2,500 episodes benchmark
- **Environment**: Continuous control locomotion task

## 📊 Results Summary

| Metric                   | Seed 40090 | Seed 202507 |
|--------------------------|------------|--------------|
| Total Episodes           | 3,500      | 3,500        |
| Mean Reward              | –22.58     | –128.31      |
| Std Deviation            | 102.60     | 31.22        |
| Max Reward               | 261.55     | 250.87       |
| Min Reward               | –261.77    | –296.16      |
| Final 100 Ep Avg Reward  | +28.25     | –122.54      |

## 📁 Repository Structure

```bash
.
├── metadata.yaml               # arXiv-ready metadata
├── marcel_arxiv.tex            # Full LaTeX source
├── marcel_arxiv.pdf            # Compiled scientific paper (user-compiled)
├── data/
│   └── Comparatif_BWHC_seed40090_vs_202507.xlsx  # Episode-level reward comparison
├── docs/
│   └── figures/                # (Optional) Future performance charts
├── README.md                   # You are here
```

## 🔒 Code and License

The implementation details of the agent (F, B, P, M modules) are confidential and are not released. Only benchmark results and structural analysis are provided under the following license:

**License**: `CC BY-NC-ND 4.0`
🔗 https://creativecommons.org/licenses/by-nc-nd/4.0/

## 🔗 Citation

If you use these results or refer to Marcel's architecture in your work, please cite the accompanying paper an:

> "Asymmetric Convergence in Hybrid Actor-Critic Agents: A Comparative Study of Seed Effects Using Marcel", 2025.

---

© 2025 Franck-Olivier RIPOLL – All rights reserved.
