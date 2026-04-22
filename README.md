# Ouroboros Research Program: Reflexive Intelligence & Multi-Reward GRPO

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.19557261-blue)](https://doi.org/10.5281/zenodo.19557261)
[![ReflexBench](https://img.shields.io/badge/Benchmark-ReflexBench%20v1.0-green)](https://huggingface.co/datasets/MMJBDS/reflexbench)
[![Papers](https://img.shields.io/badge/Papers-6%20Published-orange)]()

A six-paper research program introducing **Reflexive Intelligence** — a new cognitive capability framework for LLMs that addresses reasoning in **observer-participant environments** where the agent's actions alter the ground truth. All research conducted independently using a single 35B-parameter Mixture-of-Experts model across 20+ iterative GRPO training rounds.

## Key Contributions

- **Reflexive Intelligence**: First formalization of self-referential reasoning about one's own causal impact on the environment (Paper 1)
- **Observer Depth (OD)**: Quantitative metric for measuring reflexive reasoning capability (Paper 2)
- **ReflexBench v1.0**: First benchmark for evaluating reflexive reasoning — 80 evaluation points across 6 domains (Paper 2)
- **Reward Interaction Problem (RIP)**: Discovery of structural interference patterns in multi-reward GRPO (Paper 3)
- **Phase Transition Dynamics**: Documentation of discontinuous cognitive emergence during GRPO training (Papers 1-3)
- **SCRGNDWMT Architecture**: Nine-tier, 50-subdimension cognitive reward topology (Paper 6)
- **Cognitive Lifecycle Framework**: 9-stage model extending standard AI pipelines with Reflection, Consolidation, and Evolution stages (Paper 5)

---

## Papers

### Paper 1: Reflexive Intelligence in LLMs
**Full Title**: *Reflexive Intelligence: Decision-Making in Observer-Participant Environments*

**DOI**: [10.5281/zenodo.19557261](https://doi.org/10.5281/zenodo.19557261)

**Abstract**: We introduce *Reflexive Intelligence* as a distinct cognitive capability — the capacity for genuine self-referential reasoning about one's own cognitive processes and their effects on the environment. We formalize this through the SCRGN multi-tier reward architecture and document phase transitions in reflexive reasoning emergence during GRPO training.

**File**: [`paper1_reflexive_intelligence.tex`](paper1_reflexive_intelligence.tex)

---

### Paper 2: Observer Depth (ReflexBench)
**Full Title**: *Observer Depth: Quantifying Reflexive Intelligence in LLMs via Phase Transition Analysis*

**DOI**: [10.5281/zenodo.19627242](https://doi.org/10.5281/zenodo.19627242)

**Abstract**: We introduce *Observer Depth* as a quantitative metric for reflexive intelligence and present **ReflexBench v1.0** — the first benchmark for evaluating reflexive reasoning in large language models. We document discontinuous phase transitions in reflexive capability during multi-reward GRPO training.

**File**: [`paper2_reflexbench.tex`](paper2_reflexbench.tex)

**Dataset**: [MMJBDS/reflexbench on HuggingFace](https://huggingface.co/datasets/MMJBDS/reflexbench)

**Evaluation Code**: [mmjbds/reflexbench on GitHub](https://github.com/mmjbds/reflexbench)

#### ReflexBench Results (7 Frontier LLMs)

| Model | OD-0 | OD-1 | OD-2 | OD-n | Total | Δ (Degradation) |
|-------|------|------|------|------|-------|------------------|
| Gemini 2.5 Pro | **1.00** | **0.95** | **0.85** | 0.45 | 3.25 | -0.33 |
| Claude Opus 4.6 | 0.93 | 0.88 | 0.75 | **0.63** | **3.19** | -0.43 |
| DeepSeek-R1 | 0.90 | 0.85 | 0.70 | 0.55 | 3.00 | -0.50 |
| Kimi-K2 | 0.88 | 0.83 | 0.68 | 0.53 | 2.92 | -0.50 |
| Doubao-Seed-2.0 | 0.90 | 0.83 | 0.65 | 0.45 | 2.83 | -0.47 |
| GLM-5.1 | 0.88 | 0.80 | 0.65 | 0.50 | 2.83 | -0.53 |
| Qwen3 | 0.85 | 0.78 | 0.60 | 0.48 | 2.71 | -0.55 |

**Key finding**: All models exhibit systematic degradation from OD-0 to OD-n (mean Δ = -0.47), regardless of scale or reasoning capability.

---

### Paper 3: Multi-Reward GRPO Dynamics
**Full Title**: *When Rewards Collide: Structural Interference and Phase Transitions in Multi-Objective GRPO*

**DOI**: [10.5281/zenodo.19665969](https://doi.org/10.5281/zenodo.19665969)

**Abstract**: We present a systematic study of multi-reward GRPO across 14 iterative training rounds. We introduce the *Reward Interaction Problem (RIP)*, document three interference patterns (suppressive, catalytic, phase-locked), and demonstrate that reflexive reasoning emerges *discontinuously* via a breakthrough-collapse-recovery cycle.

**File**: [`paper3_multi_reward_grpo.tex`](paper3_multi_reward_grpo.tex)

---

### Paper 4: Ouroboros V22 Architecture
**Full Title**: *Ouroboros V22: Bayesian Scenario Simulation and Recurrent Depth Cognition for Autonomous Financial Decision-Making*

**DOI**: [10.5281/zenodo.19666786](https://doi.org/10.5281/zenodo.19666786)

**Abstract**: We present the Ouroboros V22 cognitive architecture integrating a Bayesian Scenario Simulation Engine, a Recurrent Depth Cognitive Engine with adaptive computation time, and a 6-Layer Unified Memory System with Hawkes-process temporal decay. The system operates a 16-node parallel inference swarm across 8 financial market categories.

**File**: [`paper4_ouroboros_v22.tex`](paper4_ouroboros_v22.tex)

---

### Paper 5: Cognitive Lifecycle
**Full Title**: *The Cognitive Lifecycle: How AI Systems Learn to Remember, Forget, and Evolve in Non-Stationary Environments*

**DOI**: [10.5281/zenodo.19666806](https://doi.org/10.5281/zenodo.19666806)

**Abstract**: We formalize the 9-Stage Cognitive Lifecycle Framework, extending the standard AI pipeline with four missing stages: Outcome, Reflection, Consolidation, and Evolution. Five theoretical contributions including the Memory Half-Life Theorem, Dual-Stratum Memory Interaction, and Consolidation Paradox resolution.

**File**: [`paper5_cognitive_lifecycle.tex`](paper5_cognitive_lifecycle.tex)

---

### Paper 6: Cognitive Reward Topology
**Full Title**: *Cognitive Reward Topology: A Nine-Tier Architecture for Measuring and Shaping Intelligence via Multi-Reward GRPO*

**DOI**: [10.5281/zenodo.19666829](https://doi.org/10.5281/zenodo.19666829)

**Abstract**: We present a nine-tier reward architecture (SCRGNDWMT) with 50 sub-dimensions that transforms multi-reward GRPO into a structured cognitive measurement system. Twelve theoretical innovations in a six-level hierarchy, validated on a 35B MoE model.

**File**: [`paper6_cognitive_reward_topology.tex`](paper6_cognitive_reward_topology.tex)

---

## Resources

| Resource | Link | Description |
|----------|------|-------------|
| **ReflexBench v1.0 Dataset** | [HuggingFace](https://huggingface.co/datasets/MMJBDS/reflexbench) | 80 evaluation points across 6 domains, 4 Observer Depth levels |
| **ReflexBench Eval Code** | [GitHub](https://github.com/mmjbds/reflexbench) | Scoring scripts, scenarios, and evaluation protocol |
| **All Papers (Zenodo)** | [P1](https://doi.org/10.5281/zenodo.19557261) · [P2](https://doi.org/10.5281/zenodo.19627242) · [P3](https://doi.org/10.5281/zenodo.19665969) · [P4](https://doi.org/10.5281/zenodo.19666786) · [P5](https://doi.org/10.5281/zenodo.19666806) · [P6](https://doi.org/10.5281/zenodo.19666829) | Permanent DOIs |

### Key Hyperparameters (from papers)
| Parameter | Value |
|-----------|-------|
| Group size (g) | 8 |
| Max completion tokens | 800 |
| Learning rate | 5 × 10⁻⁷ |
| Temperature | 1.15 |
| Top-p | 0.92 |
| β-annealing window | N = 5 steps |
| Reward tiers | 9 (SCRGNDWMT) |
| Sub-dimensions | 50 (V22) → 54 (V24) |

---

## Compilation

All papers compile with standard `pdflatex` (tested on Overleaf):

```bash
pdflatex paper1_reflexive_intelligence.tex
pdflatex paper3_multi_reward_grpo.tex     # ACM sigconf format
pdflatex paper6_cognitive_reward_topology.tex  # Requires neurips_2026.sty (included)
```

Paper 6 requires `neurips_2026.sty` which is included in this repository.

---

## Citation

If you use any part of this work, please cite the relevant paper(s):

```bibtex
@article{zhang2026reflexive,
  title={Reflexive Intelligence: Decision-Making in Observer-Participant Environments},
  author={Zhang, Mian},
  year={2026},
  doi={10.5281/zenodo.19557261}
}

@article{zhang2026observerdepth,
  title={Observer Depth: Quantifying Reflexive Intelligence in LLMs via Phase Transition Analysis},
  author={Zhang, Mian},
  year={2026},
  doi={10.5281/zenodo.19627242}
}

@article{zhang2026rewardscollide,
  title={When Rewards Collide: Structural Interference and Phase Transitions in Multi-Objective GRPO},
  author={Zhang, Mian},
  year={2026},
  doi={10.5281/zenodo.19665969}
}

@article{zhang2026ouroborosv22,
  title={Ouroboros V22: Bayesian Scenario Simulation and Recurrent Depth Cognition},
  author={Zhang, Mian},
  year={2026},
  doi={10.5281/zenodo.19666786}
}

@article{zhang2026lifecycle,
  title={The Cognitive Lifecycle: How AI Systems Learn to Remember, Forget, and Evolve},
  author={Zhang, Mian},
  year={2026},
  doi={10.5281/zenodo.19666806}
}

@article{zhang2026topology,
  title={Cognitive Reward Topology: A Nine-Tier Architecture for Multi-Reward GRPO},
  author={Zhang, Mian},
  year={2026},
  doi={10.5281/zenodo.19666829}
}
```

---

## Related Terms

This research program introduces the following novel concepts:

- **Reflexive Intelligence** — Self-referential reasoning about causal impact on the environment
- **Observer Depth (OD)** — Quantitative metric for reflexive reasoning capability
- **Observer-Participant Environment** — Decision environments where the agent's actions alter the ground truth
- **Reward Interaction Problem (RIP)** — Structural interference between reward dimensions in multi-objective GRPO
- **Phase-Locked Interference** — Periodic oscillation between competing reward dimensions
- **Breakthrough-Collapse-Recovery Cycle** — Characteristic pattern of cognitive emergence in GRPO training
- **SCRGNDWMT Architecture** — Nine-tier cognitive reward topology (Structure, Content, Reasoning, Game Theory, Narrative, Data Fidelity, World Model, Metacognition, Temporal-Causal)
- **Cognitive Reward Topology** — Using reward architecture as a cognitive measurement and shaping system
- **Cognitive Lifecycle** — 9-stage framework extending AI pipeline with Reflection, Consolidation, and Evolution
- **Memory Half-Life Theorem** — Formal model of temporal decay in AI memory systems

---

## License

This work is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

## Author

- **Mian Zhang** — Independent AI Researcher
- **ORCID**: [0009-0001-9556-3839](https://orcid.org/0009-0001-9556-3839)
- **Email**: 373743743@qq.com
- **GitHub**: [@mmjbds](https://github.com/mmjbds)
- **HuggingFace**: [MMJBDS](https://huggingface.co/MMJBDS)
- **ResearchGate**: [Mian-Zhang-19](https://www.researchgate.net/profile/Mian-Zhang-19)
- **Twitter/X**: [@Henry_Avery666](https://x.com/Henry_Avery666)
- **LinkedIn**: [henryavery-mianzhang](https://linkedin.com/in/henryavery-mianzhang)
