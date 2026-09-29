<div align="center">

# Spatial Memory Intelligence (SMI)

### Endowing World Models with Understanding-Driven Long-Term Memory

[Project Website](https://spatial-memory-intelligence.github.io/) · [Video Comparisons](https://spatial-memory-intelligence.github.io/#demos) · [Method](https://spatial-memory-intelligence.github.io/#method)

**Code coming soon.**

</div>

## Overview

As historical memory grows, managing spatial memory becomes increasingly complex, requiring coordinated organization, maintenance, sparsification, and retrieval. This calls for a more intelligent and comprehensive memory-management approach.

**Spatial Memory Intelligence (SMI)** is the first understanding-driven unified spatial-memory manager for long-video world models. It uses a multimodal large language model (MLLM) to coordinate four atomic operations, bringing semantic and spatial reasoning into the memory-management pipeline.

Experiments across multiple baselines, benchmarks, and world-model backbones demonstrate improvements in **memory sparsity, spatial consistency, and generation stability**.

![SMI overview: organizing spatial memory, retrieving relevant observations, and improving consistency and stability.](https://spatial-memory-intelligence.github.io/assets/teaser.png)

## Method

SMI maintains persistent spatial memory through four coordinated operations:

| Operation | Role in spatial-memory management |
| --- | --- |
| **Spatial clustering** | Group spatially related observations into coherent memory clusters. |
| **Within-cluster sparsification** | Remove redundant observations while retaining useful spatial evidence. |
| **Action-aware retrieval** | Select relevant memories using recent context and the next user action. |
| **Reliability-aware filtering** | Keep unreliable generated observations from entering persistent memory. |

Dedicated instructions and supervision teach the MLLM the semantic and spatial judgments required by each operation. Together, these operations support both memory updates and retrieval throughout long-horizon generation.

![SMI framework: an understanding model coordinates four atomic operations around persistent spatial memory.](https://spatial-memory-intelligence.github.io/assets/framework.png)

## Video Comparisons

The project website provides synchronized comparisons on **HY1.5** and **Wan2.2**, organized by:

- **Spatial consistency:** preserving scene structure when revisiting previously observed regions.
- **Generation stability:** maintaining coherent generation over longer trajectories.

Compare SMI with Base and, where available, FramePack, Deep Forcing, MoC, VMem, and MemFlow. Red-box highlights identify selected visible inconsistencies.

**[Explore the interactive comparisons →](https://spatial-memory-intelligence.github.io/#demos)**

## Release Status

This repository currently contains the project introduction. The research implementation has not been uploaded yet.

| Resource | Status |
| --- | --- |
| Project website and video demonstrations | [Available](https://spatial-memory-intelligence.github.io/) |
| Training, inference, and evaluation code | Coming soon |
| Paper | Link to be added |
| Model weights on Hugging Face | Link to be added |
| Dataset | Link to be added |

Installation requirements, runnable examples, and reproduction instructions will accompany the code release.

## Authors

[Ying Yang](https://github.com/xbyym)\*, [Guiyu Zhang](https://grenoble-zhang.github.io/)\*, [Lianghua Huang](https://github.com/huanglianghua), [Chang Nie](https://github.com/Clare-Nie), [Chenyang Si](https://chenyangsi.top/), [Haofan Wang](https://haofanwang.github.io/), [Shaoshuai Shi](https://shishaoshuai.com/), and [Li Jiang](https://llijiang.github.io/)†.

\* Equal contribution. † Corresponding author.

The Chinese University of Hong Kong, Shenzhen · Alibaba Group · Nanjing University · Lovart AI · Voyager Research, Didi Chuxing
