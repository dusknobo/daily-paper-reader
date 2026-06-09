---
title: "PDE-Transformer: Efficient and Versatile Transformers for Physics Simulations"
title_zh: PDE-Transformer：用于物理模拟的高效通用变换器
authors: "Benjamin Holzschuh, Qiang Liu, Georg Kohl, Nils Thuerey"
date: 2025-05-01
pdf: "https://openreview.net/pdf?id=3BaJMRaPSx"
tags: ["query:falling-film"]
score: 6.0
evidence: 用于物理模拟的通用变换器代理模型，可潜在用于降膜CFD
tldr: PDE-Transformer采用通道独立嵌入和时空自注意力，设计了一种面向大规模物理模拟的通用变换器架构。该模型在16种不同类型PDE数据集上超越现有视觉变换器，可作为科学机器学习的基础骨干，为降膜CFD等模拟提供高效代理模型。
source: ICML-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1762, \"height\": 490, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1778, \"height\": 649, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 850, \"height\": 416, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 841, \"height\": 793, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 849, \"height\": 645, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 839, \"height\": 391, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1690, \"height\": 615, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1359, \"height\": 706, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1567, \"height\": 911, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1590, \"height\": 915, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1595, \"height\": 602, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 792, \"height\": 886, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1719, \"height\": 363, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 1703, \"height\": 725, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 1703, \"height\": 1455, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-016.webp\", \"caption\": \"\", \"page\": 0, \"index\": 16, \"width\": 1712, \"height\": 1447, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-017.webp\", \"caption\": \"\", \"page\": 0, \"index\": 17, \"width\": 1711, \"height\": 1447, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-018.webp\", \"caption\": \"\", \"page\": 0, \"index\": 18, \"width\": 1714, \"height\": 1444, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-019.webp\", \"caption\": \"\", \"page\": 0, \"index\": 19, \"width\": 1720, \"height\": 1454, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-020.webp\", \"caption\": \"\", \"page\": 0, \"index\": 20, \"width\": 1762, \"height\": 1119, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-021.webp\", \"caption\": \"\", \"page\": 0, \"index\": 21, \"width\": 1760, \"height\": 1501, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-022.webp\", \"caption\": \"\", \"page\": 0, \"index\": 22, \"width\": 1763, \"height\": 1503, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-023.webp\", \"caption\": \"\", \"page\": 0, \"index\": 23, \"width\": 1763, \"height\": 1900, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-024.webp\", \"caption\": \"\", \"page\": 0, \"index\": 24, \"width\": 1686, \"height\": 1062, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-025.webp\", \"caption\": \"\", \"page\": 0, \"index\": 25, \"width\": 1746, \"height\": 1104, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-026.webp\", \"caption\": \"\", \"page\": 0, \"index\": 26, \"width\": 1586, \"height\": 2221, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-3bajmrapsx/fig-027.webp\", \"caption\": \"\", \"page\": 0, \"index\": 27, \"width\": 1750, \"height\": 1995, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-icml-2025-3bajmrapsx/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 862, \"height\": 387, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-3bajmrapsx/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 762, \"height\": 274, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-3bajmrapsx/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 855, \"height\": 405, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-3bajmrapsx/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1123, \"height\": 326, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-3bajmrapsx/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1757, \"height\": 580, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-3bajmrapsx/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 883, \"height\": 431, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-3bajmrapsx/table-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 745, \"height\": 413, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-3bajmrapsx/table-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 900, \"height\": 388, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-3bajmrapsx/table-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1475, \"height\": 705, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-3bajmrapsx/table-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1769, \"height\": 274, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-3bajmrapsx/table-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1766, \"height\": 272, \"label\": \"Table\"}]"
motivation: 现有物理模拟变换器难以兼顾可扩展性和通用性。
method: 结合扩散变换器架构改进与大规模模拟适配，提出通道独立嵌入和时空自注意力的PDE-Transformer。
result: 在多类PDE基准上优于最先进变换器，展现了通用性和效率。
conclusion: PDE-Transformer有望成为物理科学中的基础模型，加速包括降膜传热在内的CFD模拟。
---

## Abstract
We introduce PDE-Transformer, an improved transformer-based architecture for surrogate modeling of physics simulations on regular grids. We combine recent architectural improvements of diffusion transformers with adjustments specific for large-scale simulations to yield a more scalable and versatile general-purpose transformer architecture, which can be used as the backbone for building large-scale foundation models in physical sciences. We demonstrate that our proposed architecture outperforms state-of-the-art transformer architectures for computer vision on a large dataset of 16 different types of PDEs. We propose to embed different physical channels individually as spatio-temporal tokens, which interact via channel-wise self-attention. This helps to maintain a consistent information density of tokens when learning multiple types of PDEs simultaneously. We demonstrate that our pre-trained models achieve improved performance on several challenging downstream tasks compared to training from scratch and also beat other foundation model architectures for physics simulations.
Our source code is available at https://github.com/tum-pbs/pde-transformer.

---

## 论文详细总结（自动生成）

## 论文总结：PDE-Transformer：用于物理模拟的高效通用 Transformer

### 1. 研究动机与核心问题
*   **核心问题**：大规模物理模拟面临着**多尺度特征、多样化数据表示**（规则网格、不规则网格、粒子等）以及与传统数值方法**在精度/速度上竞争**的挑战。现有机器学习模型（如特定的卷积网络或用于视觉的 Transformer）难以作为通用骨干网络，同时兼顾模拟中的可扩展性、效率和物理通用性。
*   **研究背景**：基础模型在多个领域展现出对下游任务的强大泛化能力，但在科学机器学习 (SciML) 领域，尤其是在需要处理**多种不同偏微分方程 (PDE) 系统**的代理建模任务中，仍缺乏一个强大且高效的通用 Transformer 架构。

### 2. 方法论
论文提出了 **PDE-Transformer**，这是一种针对物理模拟数据量身定制的通用 Transformer 架构，其核心思想是通过对扩散 Transformer 架构进行多项关键改进，以提升其处理 PDE 数据的可扩展性和通用性。

*   **核心思想与关键技术细节**：
    *   **多尺度架构**：扩散 Transformer (DiT) 通常不使用上下采样，而 PDE-Transformer **引入了基于 PixelShuffle/PixelUnshuffle 的 Token 下采样和上采样**，构建了一个类 U-Net 的层次化结构。这为物理数据中天然的多尺度特征提供了强大的归纳偏置。
    *   **移位窗口自注意力**：为了应对高分辨率数据导致的全局自注意力计算量平方级增长问题，它采用了 **移位窗口多头自注意力 (Shifted Window MHSA)**。该操作将自注意力限制在局部窗口内，并交替移动窗口位置，以在保证信息流通的同时显著降低计算开销。模型使用**对数间隔的相对位置编码**，增强了平移不变性和对不同分辨率的泛化能力。
    *   **解耦的通道表示（关键技术）**：论文提出了一种新颖的**独立通道 (Separate Channel, SC) 嵌入方式**。对于具有多个物理量（如速度的x、y分量）的物理系统，传统方法将不同通道混合为一个 Token（混合通道 MC），这会导致信息密度不一致。SC 变体**为每个物理通道独立生成时空 Token，并通过在 Transformer 块中增加一个轴向的通道级自注意力操作来实现不同通道间的交互**。这保证了无论数据有多少物理通道，单个 Token 的信息密度保持不变，显著提升了多 PDE 学习和微调的性能。
    *   **深度条件机制**：沿用 DiT 的 **adaLN-Zero 块**，模型能够灵活地将 PDE 类型、物理通道类型（如密度、涡量）、扩散时间步以及**额外的仿真参数**（如粘度、域范围）作为条件注入网络。条件向量通过调节层归一化的尺度和位移参数来影响特征。
    *   **边界条件处理**：网络显式支持周期性和非周期性边界条件。对于非周期性条件，通过在计算注意力分数时进行掩码来阻止跨边界的 Token 交互。
    *   **训练范式**：模型支持**监督学习**（直接使用 MSE 损失）和**扩散训练**（基于流匹配，Flow Matching）。扩散训练允许模型从后验分布中采样，适用于解非唯一的反问题等任务。

### 3. 实验设计
实验分为两部分：在多种 PDE 上预训练以验证架构，并在具有挑战性的下游任务中微调以验证其泛化能力。

*   **预训练数据集与基准**：基于 APEBench 构建了一个包含 **16 种线性和非线性 PDE** 的大规模数据集，包括扩散方程、Fisher-KPP、Burgers'方程、多类 Gray-Scott 方程、Kolmogorov 流等。数据集由谱求解器在 \(2048 \times 2048\) 分辨率生成，并下采样到 \(256 \times 256\)。任务是给定前一时刻的状态，自回归地预测下一时刻。
*   **对比方法**：与多种最先进的 (SOTA) 架构进行了比较，包括：
    *   **DiT** (扩散 Transformer)
    *   **UDiT** (U形扩散 Transformer)
    *   **scOT** (可扩展算子 Transformer)
    *   **FactFormer** (基于因子化核积分的 Transformer)
    *   **现代 UNet**
*   **下游任务数据集**：使用了 **Well 数据集中的 3 个复杂任务**进行 Out-of-Distribution 测试：
    1.  **主动物质 (Active Matter)**：周期性边界，方形域。
    2.  **Rayleigh-Bénard 对流 (RBC)**：具有非周期性（壁面）边界，非方形域。
    3.  **剪切流 (Shear Flow)**：周期性边界，非方形域。
    在这些下游任务中，预训练的 PDE-Transformer 与从零训练的同架构模型以及 FNO（傅里叶神经算子）、OFormer 等进行了比较。

### 4. 资源与算力
*   **硬件配置**：预训练和大部分实验使用 **4 块 H100 GPU**。
*   **训练时长**：论文详细报告了训练 100 个 epoch 的时间。
    *   配置 (S) 训练耗时 7 小时 42 分钟。
    *   配置 (B) 训练耗时 10 小时 40 分钟。
    *   配置 (L) 训练耗时 20 小时 8 分钟。
*   相比之下，作为参考的 DiT-S 训练耗时 13 小时 4 分钟，UDiT-S 训练耗时 18 小时 30 分钟，显示出 PDE-Transformer 在训练效率上的优势。

### 5. 实验数量与充分性
实验设计非常详尽且客观公平，充分验证了模型的各方面性能。
*   **架构对比实验**：将 PDE-Transformer 与 5 种不同的 SOTA 架构在 **16 种 PDE** 上进行系统比较（表 1、图 3）。
*   **扩展性消融实验**：
    *   对模型参数（配置 S, B, L）进行了扩展分析（表 2）。
    *   深入研究了域大小变化对计算量（GFlops）和显存的影响（图 3）。
*   **关键超参数消融实验**：对**窗口大小和 Patch 大小**进行了精细的消融研究，探究其对精度和计算开销的权衡，找到了最佳设置（图 5）。
*   **通道嵌入方案对比**：详细对比了**混合通道（MC）和独立通道（SC）** 两种方案在预训练和下游任务微调中的性能（表 3、图 4）。
*   **训练范式对比**：比较了监督学习和扩散模型（流匹配）训练的结果（图 4）。
*   **下游任务泛化实验**：在 **3 个具有不同物理、几何和边界条件的复杂下游任务**上测试了预训练模型的迁移能力，并与多个从零训练的模型基线进行了公平比较（图 6、表 3）。

### 6. 主要结论与发现
*   **精度-效率优越性**：PDE-Transformer 在包含 16 种 PDE 的大规模数据集上，以**更少的参数量和更快的训练速度**（配置 S），取得了优于或媲美 SOTA Transformer 架构（如 UDiT）的预测精度。
*   **卓越的扩展性**：通过使用移位窗口自注意力和优化的上下采样策略，PDE-Transformer 在推理计算量 (GFlops) 和 GPU 显存占用方面，相较于 DiT 和 UDiT **表现出更优的扩展性**，尤其适合高分辨率模拟（图 3）。
*   **通道解耦表示的优势**：提出的**独立通道 (SC) 方案**，虽然在预训练中与 MC 方案精度相当，但在复杂的下游任务微调中，**性能提升显著优于 MC 方案**（平均提升是 MC 的 2.7 到 4.4 倍），证明其保留了更多可迁移知识。
*   **强大的泛化能力**：仅在规则方形域和周期边界数据上预训练的 PDE-Transformer，能够成功泛化到**非方形域、非周期边界**以及动力学特性迥异的复杂下游任务中，并**相较于从零训练的模型平均提升 42%**（相较于次优模型 FNO），超越了其他物理基础模型（如 Poseidon 的 scOT-B）。

### 7. 优点
*   **架构设计创新**：将多尺度 U形结构、移位窗口注意力和深度条件机制有机融合，同时提出了**物理直觉驱动的通道独立嵌入方案**，这是针对多物理场数据建模的重要贡献。
*   **全面且客观的实验评估**：实验覆盖了 **5 种以上基线模型、16 种 PDE的预训练和 3 种下游任务**，并且对关键超参数和设计方案进行了详尽的消融和可扩展性分析，结论可靠。
*   **实用性强**：不仅关注精度，还仔细分析了训练/推理时间、GPU 显存和计算量，为实际部署提供了高质量的指导。
*   **方法灵活性高**：同时支持监督学习和扩散生成式训练，使其既能作为确定性代理模型，也能用于不确定性和反问题求解。

### 8. 不足与局限
*   **维度限制**：当前模型仅设计和验证于 **二维（2D）规则网格数据**，未扩展到更复杂的三维（3D）模拟或不规则网格。
*   **任务限制**：实验聚焦于**自回归预测**任务，对于数据同化、处理噪声/部分观测数据、反问题等任务的验证，文中提及但仍是未来待开展的工作。
*   **对非规则数据的适应**：论文提出可以与图神经算子 (GNO) 结合以处理不规则几何，但该方案并未在实验中进行验证。

（完）
