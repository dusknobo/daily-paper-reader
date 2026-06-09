---
title: "M2PDE: Compositional Generative Multiphysics and Multi-component PDE Simulation"
title_zh: M2PDE：组合式生成多物理场和多组件PDE模拟
authors: "Tao Zhang, Zhenhai Liu, Feipeng Qi, Yongjun Jiao, Tailin Wu"
date: 2025-05-01
pdf: "https://openreview.net/pdf?id=Pwr2LznsQc"
tags: ["query:falling-film"]
score: 4.0
evidence: 面向多物理场及多组件PDE模拟的组合式生成模型，可直接用于多相流CFD
tldr: 多物理场仿真通常需要集成多个专用求解器，开发复杂且难以处理大规模多组件结构。本文提出M2PDE，利用扩散模型进行组合式生成，统一模拟多物理和多组件PDE。实验表明该方法能有效耦合不同物理过程，生成高保真仿真结果，降低了多物理仿真的门槛。
source: ICML-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-icml-2025-pwr2lznsqc/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1702, \"height\": 843, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pwr2lznsqc/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 816, \"height\": 371, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pwr2lznsqc/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 863, \"height\": 390, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pwr2lznsqc/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1776, \"height\": 615, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pwr2lznsqc/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1747, \"height\": 451, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pwr2lznsqc/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1773, \"height\": 1786, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pwr2lznsqc/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1648, \"height\": 604, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pwr2lznsqc/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1343, \"height\": 612, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pwr2lznsqc/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 759, \"height\": 1646, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pwr2lznsqc/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 757, \"height\": 1632, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pwr2lznsqc/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 773, \"height\": 1642, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pwr2lznsqc/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 766, \"height\": 1628, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pwr2lznsqc/fig-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 760, \"height\": 1645, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pwr2lznsqc/fig-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 765, \"height\": 1647, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pwr2lznsqc/fig-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 1734, \"height\": 483, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pwr2lznsqc/fig-016.webp\", \"caption\": \"\", \"page\": 0, \"index\": 16, \"width\": 1743, \"height\": 336, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pwr2lznsqc/fig-017.webp\", \"caption\": \"\", \"page\": 0, \"index\": 17, \"width\": 1733, \"height\": 478, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-icml-2025-pwr2lznsqc/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1124, \"height\": 336, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pwr2lznsqc/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1474, \"height\": 342, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pwr2lznsqc/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1399, \"height\": 491, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pwr2lznsqc/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 932, \"height\": 546, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pwr2lznsqc/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1040, \"height\": 327, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pwr2lznsqc/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1134, \"height\": 547, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pwr2lznsqc/table-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1155, \"height\": 328, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pwr2lznsqc/table-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 694, \"height\": 545, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pwr2lznsqc/table-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1088, \"height\": 326, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pwr2lznsqc/table-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1136, \"height\": 375, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pwr2lznsqc/table-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 763, \"height\": 508, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pwr2lznsqc/table-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 547, \"height\": 197, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pwr2lznsqc/table-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 406, \"height\": 281, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pwr2lznsqc/table-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 603, \"height\": 240, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pwr2lznsqc/table-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 1147, \"height\": 507, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pwr2lznsqc/table-016.webp\", \"caption\": \"\", \"page\": 0, \"index\": 16, \"width\": 1005, \"height\": 421, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pwr2lznsqc/table-017.webp\", \"caption\": \"\", \"page\": 0, \"index\": 17, \"width\": 1354, \"height\": 420, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pwr2lznsqc/table-018.webp\", \"caption\": \"\", \"page\": 0, \"index\": 18, \"width\": 1078, \"height\": 429, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pwr2lznsqc/table-019.webp\", \"caption\": \"\", \"page\": 0, \"index\": 19, \"width\": 1004, \"height\": 275, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pwr2lznsqc/table-020.webp\", \"caption\": \"\", \"page\": 0, \"index\": 20, \"width\": 1767, \"height\": 290, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pwr2lznsqc/table-021.webp\", \"caption\": \"\", \"page\": 0, \"index\": 21, \"width\": 1460, \"height\": 435, \"label\": \"Table\"}]"
motivation: 多物理场仿真需集成多个专用求解器，复杂结构仿真困难。
method: 提出基于扩散模型的组合式多物理场多组件PDE模拟框架M2PDE。
result: 该框架能灵活耦合不同物理过程，生成高质量仿真数据。
conclusion: M2PDE为多物理多组件系统提供了通用高效的生成式仿真途径。
---

## Abstract
Multiphysics simulation, which models the interactions between multiple physical processes, and multi-component simulation of complex structures are critical in fields like nuclear and aerospace engineering. Previous studies use numerical solvers or ML-based surrogate models for these simulations. However, multiphysics simulations typically require integrating multiple specialized solvers-each for a specific physical process-into a coupled program, which introduces significant development challenges. Furthermore, existing numerical algorithms struggle with highly complex large-scale structures in multi-component simulations. Here we propose compositional Multiphysics and Multi-component PDE Simulation with Diffusion models (M2PDE) to overcome these challenges. During diffusion-based training, M2PDE learns energy functions modeling the conditional probability of one physical process/component conditioned on other processes/components. In inference, M2PDE generates coupled multiphysics and multi-component solutions by sampling from the joint probability distribution. We evaluate M2PDE on two multiphysics tasks-reaction-diffusion and nuclear thermal coupling--where it achieves more accurate predictions than surrogate models in challenging scenarios. We then apply it to a multi-component prismatic fuel element problem, demonstrating that M2PDE scales from single-component training to a 64-component structure and outperforms existing domain-decomposition and graph-based approaches. The code is available at github.com/AI4Science-WestlakeU/M2PDE.

---

## 论文详细总结（自动生成）

好的，这是基于您提供的论文内容生成的结构化中文总结。

### 1. 核心问题与整体含义
*   **核心问题**：在核工程、航空航天等领域，多物理场模拟（如反应-扩散、核-热耦合）和多组件模拟（如由大量重复燃料元件组成的反应堆）至关重要，但现有方法面临巨大挑战。
    *   **多物理场模拟**：需要将多个针对不同物理过程的专业数值求解器集成到一个耦合程序中，开发难度大、计算成本高。
    *   **多组件模拟**：对整个大规模复杂结构直接求解常因自由度激增而导致计算困难或收敛失败，传统子结构方法缺乏普适性。
    *   **机器学习替代模型**：虽然能加速模拟，但仍依赖耦合数据训练，这意味着必须先开发出耦合数值程序，未能从根本上解决开发难题。
*   **整体含义（研究动机）**：本文旨在提出一种全新范式，从根本上规避耦合程序的开发。其核心思想是：能否**仅在解耦数据（或小组件数据）上训练模型，却在推理时生成耦合的多物理场解（或大规模多组件结构的解）**？论文将这一构想定义为生成式概率建模问题。

### 2. 论文提出的方法论：M2PDE
M2PDE 的全称是“组合式多物理场和多组件偏微分方程模拟”（Compositional Multiphysics and Multi-component PDE Simulation）。其核心是将物理过程/组件的求解视作条件概率分布，并通过组合这些条件分布来采样联合分布，从而获得耦合/大规模解。

*   **核心思想**：利用扩散模型学习每个物理过程（或组件）在其他过程（或相邻组件）条件下的条件概率分布的能量函数。在推理时，通过马尔可夫链蒙特卡洛（MCMC）式的迭代采样过程，从组合后的联合概率分布中生成耦合解。

*   **关键技术细节与算法流程**：
    *   **多物理场模拟 (Section 3.1)**：
        *   **概率建模**：将多物理场耦合解 \\(z = (z_1, ..., z_N)\\) 视为联合分布 \\(p(z)\\)，每个物理过程 \\(z_i\\) 视为条件分布 \\(p(z_i|z_{\neq i})\\)。
        *   **理论基础**：通过能量函数推导得出关键公式 \\(\nabla_{z_i} E(z_1, ..., z_N) = \nabla_{z_i} E(z_i|z_{\neq i})\\)，意味着联合分布的梯度可以由条件分布的梯度组合而成。
        *   **训练**：使用**解耦数据**（即固定其他物理场，仅求解当前物理场的数据）独立训练每个物理过程的扩散模型，学习其条件分布的得分函数 \\(\epsilon_\theta(z_{i,s} | z_{\neq i}, s)\\)。
        *   **推理 (Algorithm 1)**：采用类似期望最大化（EM）的迭代过程。从随机噪声开始，在每个扩散去噪步 \\(s\\) 中，基于其他物理过程当前的最佳估计值 \\(\tilde{z}_{\neq i}\\)，顺序更新每个物理场 \\(z_i\\)。可引入外部循环 \\(K\\) 和权重参数 \\(\lambda\\) 来优化估计。

    *   **多组件模拟 (Section 3.2)**：
        *   **概率建模**：将大规模结构视为无向图，每个组件的物理场 \\(z_{v_i}\\) 视为图节点，满足局部马尔可夫性，即其条件分布仅依赖于邻居节点：\\(p(z_{v_i}|z_{\partial v_i})\\)。
        *   **训练**：使用**小组件结构数据**（如16组件）训练一个单一的扩散模型，该模型学习根据中心组件邻居的状态预测其解。
        *   **推理 (Algorithm 2)**：在更大规模结构（如64组件）的图拓扑上，迭代地对所有组件同时进行扩散去噪。每一步都使用当前所有组件的估计值 \\(\tilde{z}\\) 来更新每个组件的邻居信息 \\(z_{\partial v}\\)。

### 3. 实验设计
论文设计了三个实验场景，覆盖了多物理场和多组件模拟，并使用统一的网络架构（FNO/U-Net或Geo-FNO/Transolver）来公平比较M2PDE和替代模型的性能。

*   **数据集/场景**：
    1.  **反应-扩散方程 (Reaction-Diffusion)**：1D FitzHugh-Nagumo 方程，有两个耦合的浓度场 (u, v)。训练数据为解耦数据，测试数据为全耦合解。
    2.  **核-热耦合 (Nuclear Thermal Coupling)**：针对板状燃料元件的瞬态问题，涉及中子物理、固体热传导、流体传热三个物理场的多种耦合模式（区域/界面、强/弱、单向/双向耦合）。训练数据为通过预迭代生成的解耦数据，测试数据为算子分裂法生成的耦合解。
    3.  **棱柱状燃料元件 (Prismatic Fuel Element)**：预测高温反应堆中由64个重复元件组成的复杂结构的温度和应变。训练数据是从一个包含16个元件的“中等结构”模拟中提取的单组件数据，测试数据为包含16和64个元件的整体结构解。

*   **Benchmark/对比方法**：
    *   **替代模型 (Surrogate Model)**：为每个物理场/组件独立训练的直接映射神经网络，在推理时通过迭代（类似Gauss-Seidel）收敛至耦合解。这是核心基线。
    *   **图神经网络 (GNN) / 图变换器 (Graph Transformer)**：在实验3中，用于对比在多组件模拟上的性能，包括GIN、SAN和MeshGraphNet。

### 4. 资源与算力
*   论文**未明确提及**所使用的GPU型号、数量以及具体的训练时长。虽然附录部分详细列出了网络结构、训练步数（\\(10^5\\) 到 \\(2 \times 10^5\\)步）、批次大小等超参数，但缺少关于算力成本的描述。

### 5. 实验数量与充分性
*   **实验数量**：论文进行了3大组主要实验，并在每个实验中对比了不同的骨干网络（U-Net vs. FNO， Transolver vs. Geo-FNO）。此外，附录中包含了丰富的分析：
    *   **消融实验**：对推算物理场的方法、外部循环次数K、权重λ进行了消融研究。
    *   **分布差异分析**：量化并可视化了训练数据（解耦/小型）与测试数据（耦合/大型）之间的Wasserstein距离。
    *   **加速采样实验**：测试了DDIM在不同参数下的加速效果与精度损失。
    *   **效率分析**：对比了M2PDE、替代模型和数值求解器的运行时间。
    *   **耦合数据训练对比**：训练了使用耦合数据的扩散模型作为精度上限参考。
*   **充分性与公平性**：实验设计较为**充分且公平**。从简单到复杂的任务验证了核心能力。对比基线设置合理（替代模型是最直接的竞争方法），且使用相同的网络架构和超参数进行对比，保证了公平性。消融实验和分析也详实地支撑了方法设计的合理性。

### 6. 主要结论与发现
*   **多物理场模拟准确性**：M2PDE能成功从解耦训练数据中预测耦合解。尤其在复杂的**核-热耦合任务**中，替代模型在固体和流体温度场上完全失效，而M2PDE则给出了物理上合理且更精确的预测（相对误差显著降低）。
*   **多组件模拟可扩展性**：M2PDE能够从单组件（16组件结构）训练推广到预测包含64个组件的更大规模结构，且精度超越了替代模型和基于图的方法（MeshGraphNet等）。
*   **加速潜力**：结合DDIM采样加速后，相比传统数值求解器，M2PDE在复杂问题上最高可取得**41倍的加速**，且随着问题规模和复杂度增加，加速效果更明显。

### 7. 优点：方法或实验设计上的亮点
*   **视角新颖**：首次将组合式生成模型引入PDE模拟领域，将物理模拟问题巧妙地转化为概率分布的组合与采样问题。
*   **降低开发门槛**：该方法的最大优势在于**仅需解耦（或小组件）数据即可训练**，完全规避了开发复杂的耦合数值求解器或大规模的整场求解器，具有显著的工程应用价值。
*   **理论基础扎实**：通过能量函数和概率图模型（马尔可夫随机场）清晰地推导了方法原理，而非纯粹的“黑盒”应用。
*   **实验设计系统**：三个实验层层递进，并行对比了多种骨干网络和基线方法，验证了方法在不同耦合类型和物理场景下的有效性和泛化能力。开源了数据集和代码，有助于社区发展。

### 8. 不足与局限
*   **精度差距**：M2PDE预测的耦合解精度，相较于直接使用**耦合数据**训练的模型，大约低一个数量级，仍有提升空间。
*   **数据集生成挑战**：M2PDE仍需要数值求解器来生成训练数据。对于复杂问题，高效生成高质量的解耦训练数据本身是一个挑战。
*   **应用范围假设**：多组件模拟的理论推导基于**局部马尔可夫子性**，这不适用于需要确定全局本征值（如某些特征值问题）的PDEs。同时，训练数据必须充分覆盖大型结构中可能出现的所有边界条件。
*   **算力未披露**：未提供任何关于计算资源消耗的信息，这使得评估其实际应用成本和可行性时存在盲区。
*   **工程简化**：实验问题是对真实工程场景的简化，真实世界中更复杂的几何、物理和尺度效应仍需进一步验证。

（完）
