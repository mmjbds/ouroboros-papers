# Ouroboros Research Program: Reflexive Intelligence & Multi-Reward GRPO

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

A six-paper research program exploring **reflexive intelligence**, **multi-reward GRPO training dynamics**, and **cognitive architectures** for autonomous AI decision-making. All research conducted on a single 35B-parameter Mixture-of-Experts model across 16 iterative training rounds.

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
| **ReflexBench v1.0** | [HuggingFace](https://huggingface.co/datasets/MMJBDS/reflexbench) | 7-dimension reflexive reasoning benchmark (234 prompts) |
| **ReflexBench Eval** | [GitHub](https://github.com/mmjbds/reflexbench) | Scoring scripts and evaluation protocol |
| **Reward Specs** | See Papers 3 & 6 | Full 9-tier, 50-subdimension reward architecture described in detail |

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
| Sub-dimensions | 50 |

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

## License

This work is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

## Contact

- **Author**: Mian Zhang
- **Email**: 373743743@qq.com
- **GitHub**: [@mmjbds](https://github.com/mmjbds)
- **HuggingFace**: [MMJBDS](https://huggingface.co/MMJBDS)
