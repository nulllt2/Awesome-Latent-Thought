<div align="center">

<img src="figs/banner.png" alt="Awesome Latent Thought — Reasoning Beyond Language" width="100%">

## Awesome Latent Thought — Papers, Models & Research on Reasoning Beyond Language

[![Awesome](https://img.shields.io/badge/Awesome-0066CC?style=for-the-badge&logo=awesome-lists&logoColor=white)](https://github.com/sindresorhus/awesome)

</div>

> Contributions of relevant papers, models, code, and benchmarks are welcome.

## 📖 Contents

- [🗺️ Overview](#️-overview)
- [📄 Paper List](#-paper-list)
  - [Implicit CoT Distillation](#implicit-cot-distillation)
  - [Continuous Thought Representations](#continuous-thought-representations)
  - [Adaptive Latent Reasoning](#adaptive-latent-reasoning)
  - [Latent Search](#latent-search)
  - [Recurrent Reasoning Models](#recurrent-reasoning-models)
  - [Theory, Interpretability, Evaluation](#theory-interpretability-evaluation)
  - [Multimodal Latent Reasoning](#multimodal-latent-reasoning)
  - [Surveys](#surveys)
- [Star History](#star-history)

## 🗺️ Overview

A curated collection of research on **latent reasoning, continuous thoughts, and implicit chain-of-thought**, including related models, code, and benchmarks.

The collection covers methods, training, inference-time computation, interpretability, evaluation, and multimodal extensions involving reasoning in latent states. Ordinary textual chain-of-thought and generic model acceleration are outside its core scope.

<p align="center">
  <a href="figs/roadmap.png">
    <img src="figs/roadmap.png" alt="Latent Thought research roadmap: 28 representative works, 2023–2026" width="100%">
  </a>
</p>

## 📄 Paper List

<!-- BEGIN BIBLIOGRAPHY CATALOG -->

### Implicit CoT Distillation

Internalize explicit reasoning in model weights or compress it into supervised latent states; direct-answer distillation does not by itself establish stepwise latent computation.

| Date | Name | Title | Conference / Journal | Paper | Github |
|:-:|:-:|:-|:-:|:-:|:-:|
| 2025-10 | `SemCoT` | **SemCoT: Accelerating Chain-of-Thought Reasoning through Semantically-Aligned Implicit Tokens** | [NeurIPS 2025](https://proceedings.nips.cc/paper_files/paper/2025/hash/3ddbd473456a57e3cafb1ee51ddf8ff6-Abstract-Conference.html) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.24940) | [![GitHub Stars](https://img.shields.io/github/stars/YinhanHe123/SemCoT?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/YinhanHe123/SemCoT) |
| 2025-09 | `SIM-CoT` | **SIM-CoT: Supervised Implicit Chain-of-Thought** | [ICLR 2026](https://proceedings.iclr.cc/paper_files/paper/2026/hash/5d087955ee13fe9a7402eedec879b9c3-Abstract-Conference.html) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.20317) | [![GitHub Stars](https://img.shields.io/github/stars/InternLM/SIM-CoT?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/InternLM/SIM-CoT) |
| 2025-06 | `DART` | **DART: Distilling Autoregressive Reasoning to Silent Thought** | [EMNLP 2025](https://aclanthology.org/2025.emnlp-main.256/) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.11752) | — |
| 2025-02 | `CODI` | **CODI: Compressing Chain-of-Thought into Continuous Space via Self-Distillation** | [EMNLP 2025](https://aclanthology.org/2025.emnlp-main.36/) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.21074) | [![GitHub Stars](https://img.shields.io/github/stars/zhenyi4/codi?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/zhenyi4/codi) |
| 2024-12 | `CCoT` | **Compressed Chain of Thought: Efficient Reasoning Through Dense Representations** | arXiv preprint | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2412.13171) | — |
| 2024-09 | `HCoT` | **Expediting and Elevating Large Language Model Reasoning via Hidden Chain-of-Thought Decoding** | arXiv preprint | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2409.08561) | — |
| 2024-07 | `System-2 Distillation` | **Distilling System 2 into System 1** | arXiv preprint | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2407.06023) | — |
| 2024-05 | `Stepwise Internalization` | **From Explicit CoT to Implicit CoT: Learning to Internalize CoT Step by Step** | arXiv preprint | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2405.14838) | [![GitHub Stars](https://img.shields.io/github/stars/da03/Internalize_CoT_Step_by_Step?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/da03/Internalize_CoT_Step_by_Step) |
| 2023-11 | `Implicit-CoT` | **Implicit Chain of Thought Reasoning via Knowledge Distillation** | arXiv preprint | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2311.01460) | [![GitHub Stars](https://img.shields.io/github/stars/da03/implicit_chain_of_thought?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/da03/implicit_chain_of_thought) |

### Continuous Thought Representations

Represent intermediate thoughts with hidden vectors, soft token mixtures, or learned continuous concepts.

| Date | Name | Title | Conference / Journal | Paper | Github |
|:-:|:-:|:-|:-:|:-:|:-:|
| 2026-06 | `NF-CoT` | **Latent Reasoning with Normalizing Flows** | [ICLR 2027 (under review)](https://openreview.net/forum?id=jBge92WJps) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2606.06447) | — |
| 2025-10 | `Latent-SFT` | **LLM Latent Reasoning as Chain of Superposition** | arXiv preprint | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.15522) | [![GitHub Stars](https://img.shields.io/github/stars/DJC-GO-SOLO/Latent-SFT?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/DJC-GO-SOLO/Latent-SFT) |
| 2025-09 | `MarCos` | **Deep Thinking by Markov Chain of Continuous Thoughts** | arXiv preprint | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.25020) | [![GitHub Stars](https://img.shields.io/github/stars/Ljyustc/MarCos?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Ljyustc/MarCos) |
| 2025-05 | `Soft Thinking` | **Soft Thinking: Unlocking the Reasoning Potential of LLMs in Continuous Concept Space** | [NeurIPS 2025](https://proceedings.neurips.cc/paper_files/paper/2025/file/f7396d1c54d51416958d63e285377103-Paper-Conference.pdf) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.15778) | [![GitHub Stars](https://img.shields.io/github/stars/UCSB-AI/Soft-Thinking?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/UCSB-AI/Soft-Thinking) |
| 2025-05 | `Latent Tokens` | **Enhancing Latent Computation in Transformers with Latent Tokens** | arXiv preprint | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.12629) | — |
| 2025-02 | `SoftCoT` | **SoftCoT: Soft Chain-of-Thought for Efficient Reasoning with LLMs** | [ACL 2025](https://aclanthology.org/2025.acl-long.1137/) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.12134) | [![GitHub Stars](https://img.shields.io/github/stars/xuyige/SoftCoT?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/xuyige/SoftCoT) |
| 2025-02 | `CoCoMix` | **LLM Pretraining with Continuous Concepts** | [ICLR 2026](https://www.microsoft.com/en-us/research/publication/llm-pretraining-with-continuous-concepts/) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.08524) | [![GitHub Stars](https://img.shields.io/github/stars/facebookresearch/RAM?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/facebookresearch/RAM/tree/main/projects/cocomix) |
| 2024-12 | `Coconut` | **Training Large Language Models to Reason in a Continuous Latent Space** | [COLM 2025](https://proceedings.colm.cc/paper_files/paper/2025/hash/ed032b08a8822c3635cdcd961012ce60-Abstract-Conference.html) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2412.06769) | [![GitHub Stars](https://img.shields.io/github/stars/facebookresearch/coconut?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/facebookresearch/coconut) |

### Adaptive Latent Reasoning

Combine latent and textual computation, including discrete latent codes, adaptive compression, routing, and stopping.

| Date | Name | Title | Conference / Journal | Paper | Github |
|:-:|:-:|:-|:-:|:-:|:-:|
| 2026-09 | `A*-Thought-V2` | **A*-Thought-V2: Efficient Latent Reasoning via Geometric Dynamics of LLM** | [ICLR 2027 (under review)](https://openreview.net/forum?id=2LgNhdTelM) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2609.07821) | [![GitHub Stars](https://img.shields.io/github/stars/AI9Stars/AStar-Thought?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/AI9Stars/AStar-Thought) |
| 2026-07 | `SLPO` | **SLPO: Scaling Latent Reasoning via a Surrogate Policy** | [ICLR 2027 (under review)](https://openreview.net/forum?id=fHbDsua46v) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2607.19691) | [![GitHub Stars](https://img.shields.io/github/stars/ModalityDance/SLPO?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/ModalityDance/SLPO) |
| 2025-11 | `Adaptive Latent Reasoning` | **Learning When to Stop: Adaptive Latent Reasoning via Reinforcement Learning** | arXiv preprint | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.21581) | [![GitHub Stars](https://img.shields.io/github/stars/apning/adaptive-latent-reasoning?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/apning/adaptive-latent-reasoning) |
| 2025-10 | `SwiReasoning` | **SwiReasoning: Switch-Thinking in Latent and Explicit for Pareto-Superior Reasoning LLMs** | [ICLR 2026](https://swireasoning.github.io/) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.05069) | [![GitHub Stars](https://img.shields.io/github/stars/sdc17/SwiReasoning?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/sdc17/SwiReasoning) |
| 2025-08 | `SynAdapt` | **SynAdapt: Learning Adaptive Reasoning in Large Language Models via Synthetic Continuous Chain-of-Thought** | arXiv preprint | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.00574) | — |
| 2025-05 | `System-1.5` | **System-1.5 Reasoning: Traversal in Language and Latent Spaces with Dynamic Shortcuts** | [NeurIPS 2025](https://proceedings.neurips.cc/paper_files/paper/2025/hash/5e66b9f710a8e38351da690f3806cba9-Abstract-Conference.html) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.18962) | — |
| 2025-05 | `HRPO` | **Hybrid Latent Reasoning via Reinforcement Learning** | [NeurIPS 2025](https://proceedings.nips.cc/paper_files/paper/2025/hash/087f7678af2abbe0c37ecc30bd7d1adf-Abstract-Conference.html) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.18454) | [![GitHub Stars](https://img.shields.io/github/stars/Yueeeeeeee/HRPO?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Yueeeeeeee/HRPO) |
| 2025-05 | `CoLaR` | **Think Silently, Think Fast: Dynamic Latent Compression of LLM Reasoning Chains** | [NeurIPS 2025](https://proceedings.neurips.cc/paper_files/paper/2025/hash/0706261aedab63814a2b73c32564b4c4-Abstract-Conference.html) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.16552) | [![GitHub Stars](https://img.shields.io/github/stars/xiaomi-research/colar?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/xiaomi-research/colar) |
| 2025-02 | `LightThinker` | **LightThinker: Thinking Step-by-Step Compression** | [EMNLP 2025](https://aclanthology.org/2025.emnlp-main.673/) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.15589) | [![GitHub Stars](https://img.shields.io/github/stars/zjunlp/LightThinker?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/zjunlp/LightThinker) |
| 2025-02 | `Token Assorted` | **Token Assorted: Mixing Latent and Text Tokens for Improved Language Model Reasoning** | [ICML 2025](https://proceedings.mlr.press/v267/su25g.html) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.03275) | — |
| — | `Adaptive Soft Thinking` | **Beyond Uniform Soft Thinking: Adaptive Gating and Calibration of Soft Tokens for Latent Reasoning** | [ICLR 2027 (under review)](https://openreview.net/forum?id=Jn6kASdwgk) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=openreview&logoColor=white)](https://openreview.net/forum?id=Jn6kASdwgk) | — |

### Latent Search

Explore, optimize, refine, or rank intermediate latent trajectories during inference.

| Date | Name | Title | Conference / Journal | Paper | Github |
|:-:|:-:|:-|:-:|:-:|:-:|
| 2025-10 | `Continuous-Space Scaling` | **Towards Inference-time Scaling for Continuous Space Reasoning** | [ACL 2026 Findings](https://aclanthology.org/2026.findings-acl.1338/) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.12167) | — |
| 2025-10 | `LatentTTS` | **Parallel Test-Time Scaling for Latent Reasoning Models** | [ACL 2026](https://aclanthology.org/2026.acl-long.2069/) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.07745) | [![GitHub Stars](https://img.shields.io/github/stars/ModalityDance/LatentTTS?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/ModalityDance/LatentTTS) |
| 2025-10 | `LaDiR` | **LaDiR: Latent Diffusion Enhances LLMs for Text Reasoning** | [ICLR 2026](https://proceedings.iclr.cc/paper_files/paper/2026/hash/843e1d8ab4819c8c8a4221fce2c8d455-Abstract-Conference.html) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.04573) | [![GitHub Stars](https://img.shields.io/github/stars/mk322/LaDiR?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/mk322/LaDiR) |
| 2025-10 | `LTPO` | **Thinking on the Fly: Test-Time Reasoning Enhancement via Latent Thought Policy Optimization** | [ICLR 2026](https://iclr.cc/Downloads/2026) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.04182) | [![GitHub Stars](https://img.shields.io/github/stars/ltpo2025/LTPO?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/ltpo2025/LTPO) |
| 2025-09 | `LTO` | **Latent Thinking Optimization: Your Latent Reasoning Language Model Secretly Encodes Reward Signals in Its Latent Thoughts** | [ICLR 2026](https://proceedings.iclr.cc/paper_files/paper/2026/hash/a4b1a25e1b37a17733c1fea50d0b7446-Abstract-Conference.html) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.26314) | — |
| 2025-09 | `LatentEvolve` | **LatentEvolve: Self-Evolving Test-Time Scaling in Latent Space** | [EMNLP 2026](https://aclanthology.org/2026.emnlp-main.1263/) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.24771) | [![GitHub Stars](https://img.shields.io/github/stars/jins7/LatentEvolve?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/jins7/LatentEvolve) |
| 2025-05 | `LatentSeek` | **Seek in the Dark: Reasoning via Test-Time Instance-Level Policy Gradient in Latent Space** | arXiv preprint | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.13308) | — |
| 2025-05 | `SoftCoT++` | **SoftCoT++: Test-Time Scaling with Soft Chain-of-Thought Reasoning** | arXiv preprint | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.11484) | [![GitHub Stars](https://img.shields.io/github/stars/xuyige/SoftCoT?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/xuyige/SoftCoT) |

### Recurrent Reasoning Models

Reuse layers or recurrent modules to increase internal computation without requiring longer textual reasoning chains.

| Date | Name | Title | Conference / Journal | Paper | Github |
|:-:|:-:|:-|:-:|:-:|:-:|
| 2025-10 | `Encode-Think-Decode` | **Encode, Think, Decode: Scaling test-time reasoning with recursive latent thoughts** | [ICLR 2026 Latent and Implicit Thinking Workshop](https://openreview.net/pdf/9aba3c214f53c504cdc2da3e6835b366786ec66c.pdf) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.07358) | — |
| 2025-10 | `TRM` | **Less is More: Recursive Reasoning with Tiny Networks** | arXiv preprint | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.04871) | [![GitHub Stars](https://img.shields.io/github/stars/SamsungSAILMontreal/TinyRecursiveModels?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/SamsungSAILMontreal/TinyRecursiveModels) |
| 2025-06 | `HRM` | **Hierarchical Reasoning Model** | arXiv preprint | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.21734) | [![GitHub Stars](https://img.shields.io/github/stars/sapientinc/HRM?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/sapientinc/HRM) |
| 2025-05 | `PonderLM` | **PonderLM: Pretraining Language Models to Ponder in Continuous Space** | [ICLR 2026](https://proceedings.iclr.cc/paper_files/paper/2026/hash/94572a66c6b0710c5263f15d8ef6b463-Abstract-Conference.html) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.20674) | [![GitHub Stars](https://img.shields.io/github/stars/LUMIA-Group/PonderingLM?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/LUMIA-Group/PonderingLM) |
| 2025-02 | `Looped Transformers` | **Reasoning with Latent Thoughts: On the Power of Looped Transformers** | [ICLR 2025](https://proceedings.iclr.cc/paper_files/paper/2025/hash/2676109d49d1eb26d6bc584a8f556305-Abstract-Conference.html) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.17416) | — |
| 2025-02 | `ITT` | **Inner Thinking Transformer: Leveraging Dynamic Depth Scaling to Foster Adaptive Internal Thinking** | [ACL 2025](https://aclanthology.org/2025.acl-long.1369/) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.13842) | — |
| 2025-02 | `Huginn` | **Scaling up Test-Time Compute with Latent Reasoning: A Recurrent Depth Approach** | [NeurIPS 2025](https://proceedings.neurips.cc/paper_files/paper/2025/hash/3b01972cf31e6fa0fe29e4b8b5c2a0a1-Abstract-Conference.html) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.05171) | [![GitHub Stars](https://img.shields.io/github/stars/seal-rg/recurrent-pretraining?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/seal-rg/recurrent-pretraining) |
| 2023-10 | `CoTFormer` | **CoTFormer: A Chain of Thought Driven Architecture with Budget-Adaptive Computation Cost at Inference** | [ICLR 2025](https://proceedings.iclr.cc/paper_files/paper/2025/hash/1eaa5146756be028ad6fff1efcc8e6bd-Abstract-Conference.html) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2310.10845) | — |

### Theory, Interpretability, Evaluation

Study the capacity, mechanisms, faithfulness, and limits of latent reasoning; theoretical constructions and controlled-task findings are not general guarantees for deployed LLMs.

| Date | Name | Title | Conference / Journal | Paper | Github |
|:-:|:-:|:-|:-:|:-:|:-:|
| 2026-01 | `Sequential CODI Study` | **Do Latent-CoT Models Think Step-by-Step? A Mechanistic Study on Sequential Reasoning Tasks** | arXiv preprint | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.00449) | [![GitHub Stars](https://img.shields.io/github/stars/jialiang19/latent-cot-thinking?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/jialiang19/latent-cot-thinking) |
| 2025-12 | `Causal Coconut Analysis` | **Do Latent Tokens Think? A Causal and Adversarial Analysis of Chain-of-Continuous-Thought** | [EMNLP 2026](https://aclanthology.org/2026.emnlp-main.186/) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.21711) | — |
| 2025-07 | `Huginn Probing` | **Latent Chain-of-Thought? Decoding the Depth-Recurrent Transformer** | [COLM 2025 LLM Explainability Workshop](https://arxiv.org/abs/2507.02199) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.02199) | [![GitHub Stars](https://img.shields.io/github/stars/wenquanlu/huginn-latent-cot?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/wenquanlu/huginn-latent-cot) |
| 2025-05 | `CoT2` | **Continuous Chain of Thought Enables Parallel Exploration and Reasoning** | [ICLR 2026](https://proceedings.iclr.cc/paper_files/paper/2026/hash/85ec26ef94c3acb4c195e905df1ff4f7-Abstract-Conference.html) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.23648) | — |
| 2025-05 | `Internal CoT` | **Internal Chain-of-Thought: Empirical Evidence for Layer‐wise Subtask Scheduling in LLMs** | [EMNLP 2025](https://aclanthology.org/2025.emnlp-main.1147/) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.14530) | [![GitHub Stars](https://img.shields.io/github/stars/yzp11/Internal-Chain-of-Thought?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/yzp11/Internal-Chain-of-Thought) |
| 2025-05 | `Reasoning by Superposition` | **Reasoning by Superposition: A Theoretical Perspective on Chain of Continuous Thought** | [NeurIPS 2025](https://proceedings.neurips.cc/paper_files/paper/2025/hash/72c363c2a573ca2128bd176d3317696b-Abstract-Conference.html) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.12514) | — |
| 2025-04 | `Latent-Space Benchmark` | **Beyond Chains of Thought: Benchmarking Latent-Space Reasoning Abilities in Large Language Models** | arXiv preprint | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.10615) | — |
| 2025-03 | `Shortcut Reasoning` | **Implicit Reasoning in Transformers is Reasoning through Shortcuts** | [ACL 2025 Findings](https://aclanthology.org/2025.findings-acl.493/) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.07604) | — |
| 2024-11 | `Implicit-CoT Probing` | **Do LLMs Really Think Step-by-step In Implicit Reasoning?** | arXiv preprint | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2411.15862) | [![GitHub Stars](https://img.shields.io/github/stars/yuyijiong/if_step_by_step_implicit_CoT?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/yuyijiong/if_step_by_step_implicit_CoT) |
| 2024-05 | `Grokked Transformers` | **Grokking of Implicit Reasoning in Transformers: A Mechanistic Journey to the Edge of Generalization** | [NeurIPS 2024](https://proceedings.neurips.cc/paper_files/paper/2024/hash/ad217e0c7fecc71bdf48660ad6714b07-Abstract-Conference.html) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2405.15071) | [![GitHub Stars](https://img.shields.io/github/stars/OSU-NLP-Group/GrokkedTransformer?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/OSU-NLP-Group/GrokkedTransformer) |
| 2024-02 | `Latent Multi-Hop` | **Do Large Language Models Latently Perform Multi-Hop Reasoning?** | [ACL 2024](https://aclanthology.org/2024.acl-long.550/) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2402.16837) | — |

### Multimodal Latent Reasoning

Use latent visual or spatiotemporal thoughts for multimodal understanding, visual planning, and action.

| Date | Name | Title | Conference / Journal | Paper | Github |
|:-:|:-:|:-|:-:|:-:|:-:|
| 2026-10 | `AURAL` | **AURAL: Adaptive Latent Reasoning with Joint Chunk for Speech Language Models** | [ICLR 2027 (under review)](https://openreview.net/forum?id=3uuuDJFo5I) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2610.01560) | [![GitHub Stars](https://img.shields.io/github/stars/JensenYX/AURAL?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/JensenYX/AURAL) |
| 2026-09 | `ReaLVR` | **Rethinking Latent Visual Reasoning: Grounding Latent Reasoning in Visual Evidence** | [ICLR 2027 (under review)](https://openreview.net/forum?id=GAaKiNHi5i) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2609.34563) | [![GitHub Stars](https://img.shields.io/github/stars/xixiaouab/ReaLVR-code?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/xixiaouab/ReaLVR-code) |
| 2026-01 | `Fast-ThinkAct` | **Fast-ThinkAct: Efficient Vision-Language-Action Reasoning via Verbalizable Latent Planning** | [CVPR 2026](https://openaccess.thecvf.com/content/CVPR2026/html/Huang_Fast-ThinkAct_Efficient_Vision-Language-Action_Reasoning_via_Verbalizable_Latent_Planning_CVPR_2026_paper.html) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.09708) | — |
| 2026-01 | `LaST0` | **LaST₀: Latent Spatio-Temporal Chain-of-Thought for Robotic Vision-Language-Action Model** | arXiv preprint | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.05248) | [![GitHub Stars](https://img.shields.io/github/stars/ZhuoyangLiu2005/last0?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/ZhuoyangLiu2005/last0) |
| 2025-11 | `COVT` | **Chain-of-Visual-Thought: Teaching VLMs to See and Think Better with Continuous Visual Tokens** | [ECCV 2026](https://github.com/Wakals/CoVT) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.19418) | [![GitHub Stars](https://img.shields.io/github/stars/Wakals/CoVT?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Wakals/CoVT) |
| 2025-11 | `LaRe` | **LaRe: Latent Refocusing for Multimodal Reasoning** | [EMNLP 2026 Findings](https://aclanthology.org/2026.findings-emnlp.181/) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.02360) | — |
| 2025-10 | `Latent Sketchpad` | **Latent Sketchpad: Sketching Visual Thoughts to Elicit Multimodal Reasoning in MLLMs** | arXiv preprint | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.24514) | [![GitHub Stars](https://img.shields.io/github/stars/hwanyu112/Latent-Sketchpad?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/hwanyu112/Latent-Sketchpad) |
| 2025-10 | `IVT-LR` | **Reasoning in the Dark: Interleaved Vision-Text Reasoning in Latent Space** | [ACL 2026 Findings](https://aclanthology.org/2026.findings-acl.1949/) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.12603) | [![GitHub Stars](https://img.shields.io/github/stars/FYYDCC/IVT-LR?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/FYYDCC/IVT-LR) |
| 2025-09 | `LVR` | **Latent Visual Reasoning** | [ICLR 2026](https://proceedings.iclr.cc/paper_files/paper/2026/hash/efa0939caa8a906fd0a61a9c60e46e8b-Abstract-Conference.html) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.24251) | — |
| 2025-08 | `MCOUT` | **Multimodal Chain of Continuous Thought for Latent-Space Reasoning in Vision-Language Models** | [NeurIPS 2025 Efficient Reasoning Workshop](https://github.com/Hanhpt23/OmniMod) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.12587) | [![GitHub Stars](https://img.shields.io/github/stars/Hanhpt23/OmniMod?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Hanhpt23/OmniMod) |
| 2025-06 | `Mirage` | **Machine Mental Imagery: Empower Multimodal Reasoning with Latent Visual Tokens** | [CVPR 2026](https://openaccess.thecvf.com/content/CVPR2026/html/Yang_Machine_Mental_Imagery_Empower_Multimodal_Reasoning_with_Latent_Visual_Tokens_CVPR_2026_paper.html) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.17218) | [![GitHub Stars](https://img.shields.io/github/stars/UMass-Embodied-AGI/Mirage?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/UMass-Embodied-AGI/Mirage) |
| — | `Fused Multi-Latent Reasoning` | **Fused Multi-Latent Reasoning: Unified Multimodal Reasoning in Latent Space** | [ICLR 2027 (under review)](https://openreview.net/forum?id=6ewwTZLXbK) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=openreview&logoColor=white)](https://openreview.net/forum?id=6ewwTZLXbK) | — |
| — | `Confident Thinking` | **Confident Thinking: Multi-Layer Entropy-Guided Latent Reasoning for Multimodal Long-Context RAG** | [ICLR 2027 (under review)](https://openreview.net/forum?id=MLjcAknjGU) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=openreview&logoColor=white)](https://openreview.net/forum?id=MLjcAknjGU) | — |
| — | `Action-Trajectory Reasoning` | **Uncovering Latent Reasoning from Action Trajectories for Long-Horizon Agents** | [ICLR 2027 (under review)](https://openreview.net/forum?id=gdMWYAoVj0) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=openreview&logoColor=white)](https://openreview.net/forum?id=gdMWYAoVj0) | — |
| — | `ALICE` | **ALICE: Aligning Latent Reasoning with Chain-of-Thought for Multimodal-LLM Embeddings** | [ICLR 2027 (under review)](https://openreview.net/forum?id=ltHM5JkEJq) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=openreview&logoColor=white)](https://openreview.net/forum?id=ltHM5JkEJq) | — |
| — | `Structured Latent Reasoning` | **Structured Latent Reasoning: Refactoring Reasoning with Reusable Primitives for Multimodal LLMs** | [ICLR 2027 (under review)](https://openreview.net/forum?id=t1R6F2fdM0) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=openreview&logoColor=white)](https://openreview.net/forum?id=t1R6F2fdM0) | — |

### Surveys

Field overviews and taxonomies, counted separately from original research papers.

| Date | Name | Title | Conference / Journal | Paper | Github |
|:-:|:-:|:-|:-:|:-:|:-:|
| 2025-07 | `Latent Reasoning Survey` | **A Survey on Latent Reasoning** | arXiv preprint | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.06203) | [![GitHub Stars](https://img.shields.io/github/stars/multimodal-art-projection/LatentCoT-Horizon?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/multimodal-art-projection/LatentCoT-Horizon) |
| 2025-05 | `Reasoning Beyond Language` | **Reasoning Beyond Language: A Comprehensive Survey on Latent Chain-of-Thought Reasoning** | [EMNLP 2026 Findings](https://aclanthology.org/2026.findings-emnlp.55/) | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.16782) | [![GitHub Stars](https://img.shields.io/github/stars/EIT-NLP/Awesome-Latent-CoT?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/EIT-NLP/Awesome-Latent-CoT) |

<!-- END BIBLIOGRAPHY CATALOG -->

## Star History

<a href="https://www.star-history.com/?repos=nulllt2%2Fawesome-latent-thought&type=date&legend=top-left">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chart?repos=nulllt2/awesome-latent-thought&type=date&theme=dark&legend=top-left" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chart?repos=nulllt2/awesome-latent-thought&type=date&legend=top-left" />
   <img alt="Star History Chart" src="https://api.star-history.com/chart?repos=nulllt2/awesome-latent-thought&type=date&legend=top-left" />
 </picture>
</a>
