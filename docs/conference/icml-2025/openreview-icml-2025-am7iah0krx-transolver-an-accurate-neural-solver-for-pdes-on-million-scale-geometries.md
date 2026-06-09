---
title: "Transolver++: An Accurate Neural Solver for PDEs on Million-Scale Geometries"
title_zh: Transolver++：面向百万规模几何的精确神经PDE求解器
authors: "Huakun Luo, Haixu Wu, Hang Zhou, Lanxiang Xing, Yichen Di, Jianmin Wang, Mingsheng Long"
date: 2025-05-01
pdf: "https://openreview.net/pdf?id=AM7iAh0krx"
tags: ["query:falling-film"]
score: 6.0
evidence: 可处理复杂工业几何的大规模神经PDE求解器，可用于降膜CFD
tldr: 针对现有神经PDE求解器仅适用于数万网格点规模的局限，Transolver++通过优化并行机制和局部自适应策略，实现了百万级复杂几何上的精确求解。其在工业仿真基准上表现优异，为降膜换热器的计算流体力学模拟提供了高效替代方案。
source: ICML-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-icml-2025-am7iah0krx/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1728, \"height\": 458, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-am7iah0krx/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1737, \"height\": 443, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-am7iah0krx/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1664, \"height\": 482, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-am7iah0krx/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1756, \"height\": 519, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-am7iah0krx/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 835, \"height\": 380, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-am7iah0krx/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1725, \"height\": 547, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-am7iah0krx/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 847, \"height\": 383, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-am7iah0krx/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1739, \"height\": 390, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-am7iah0krx/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1744, \"height\": 373, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-am7iah0krx/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1771, \"height\": 466, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-am7iah0krx/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1768, \"height\": 466, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-am7iah0krx/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1755, \"height\": 442, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-am7iah0krx/fig-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1761, \"height\": 446, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-am7iah0krx/fig-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 1743, \"height\": 704, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-am7iah0krx/fig-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 1755, \"height\": 686, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-am7iah0krx/fig-016.webp\", \"caption\": \"\", \"page\": 0, \"index\": 16, \"width\": 1678, \"height\": 510, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-icml-2025-am7iah0krx/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 880, \"height\": 404, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-am7iah0krx/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1796, \"height\": 695, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-am7iah0krx/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 876, \"height\": 269, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-am7iah0krx/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 840, \"height\": 290, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-am7iah0krx/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 836, \"height\": 346, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-am7iah0krx/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 872, \"height\": 236, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-am7iah0krx/table-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 837, \"height\": 214, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-am7iah0krx/table-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1779, \"height\": 764, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-am7iah0krx/table-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1784, \"height\": 440, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-am7iah0krx/table-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1793, \"height\": 496, \"label\": \"Table\"}]"
motivation: 工业仿真通常涉及百万网格的复杂几何，现有神经求解器难以胜任。
method: 在Transolver基础上，引入高度优化的并行框架和局部自适应机制，高效捕捉物理状态。
result: 在百万网格的工业级PDE测试中达到高精度，速度远超传统数值方法。
conclusion: Transolver++可用于加速复杂几何下的CFD仿真，对降膜换热器模拟具有潜在价值。
---

## Abstract
Although deep models have been widely explored in solving partial differential equations (PDEs), previous works are primarily limited to data only with up to tens of thousands of mesh points, far from the million-point scale required by industrial simulations that involve complex geometries. In the spirit of advancing neural PDE solvers to real industrial applications, we present Transolver++, a highly parallel and efficient neural solver that can accurately solve PDEs on million-scale geometries. Building upon previous advancements in solving PDEs by learning physical states via Transolver, Transolver++ is further equipped with an extremely optimized parallelism framework and a local adaptive mechanism to efficiently capture eidetic physical states from massive mesh points, successfully tackling the thorny challenges in computation and physics learning when scaling up input mesh size. Transolver++ increases the single-GPU input capacity to million-scale points for the first time and is capable of continuously scaling input size in linear complexity by increasing GPUs. Experimentally, Transolver++ yields 13\% relative promotion across six standard PDE benchmarks and achieves over 20\% performance gain in million-scale high-fidelity industrial simulations, whose sizes are 100$\times$ larger than previous benchmarks, covering car and 3D aircraft designs.

---

## 论文详细总结（自动生成）

# Transolver++：面向百万规模几何的精确神经 PDE 求解器

## 1. 核心问题与研究背景
- 工业级仿真（如汽车、飞机设计）需要求解偏微分方程（PDE），其计算网格通常包含百万量级的点，传统数值方法耗时数天甚至数月。
- 现有神经 PDE 求解器（如 Transolver）最多只能处理数十万网格点，无法直接应用于大规模复杂几何，且存在**物理状态均质化**和**计算效率**两个关键瓶颈。
- 论文致力于将神经求解器的输入规模首次提升至百万级，并保持高精度，推动其走向实际工业应用。

## 2. 方法论
核心思路是在 Transolver 的 Physics-Attention 基础上，引入 **Eidetic States（逼真物理状态）** 与 **高度并行化实现**。

### 2.1 物理注意力与逼真状态
- **问题**：原有 Physics-Attention 通过可学习的切片权重 `w` 将 `N` 个网格点聚合为 `M` 个物理状态，再在状态间做注意力。当 `N` 极大时，权重趋向均匀，状态变得同质，模型退化为平均池化。
- **局部自适应机制（Ada‑Temp）**：为每个网格点学习一个温度 `τ_i`，动态调节 Softmax 的尖锐程度，使状态分布更好地反映局部物理特性。
  - `τ_i = τ_0 + Linear(x_i)`
  - 高温 → 均匀分布；低温 → 集中在关键状态。
- **切片重参数化（Rep‑Slice）**：采用 Gumbel-Softmax 进行可微分离散采样，从分类分布中“抽取”状态分配，避免直接 Softmax 造成的模糊性，使物理状态更逼真、更具区分度。
  - `w = Softmax((Linear(x) - log(-log ε)) / τ)`，其中 `ε ~ U(0,1)`。

### 2.2 并行 Transolver++
- **并行策略**：将输入网格按点拆分成多份，分配到多个 GPU。
- 每个 GPU 独立计算局部部分和 `Σ w_ij x_i` 与 `Σ w_ij`，随后通过 **AllReduce** 全局聚合，得到完整物理状态 `s_j`。
- **通信开销**：仅需传输 `M(C+1)` 量级的数据（`M` 为状态数，`C` 为通道数），与输入点数 `N` **无关**，远优于 Ring Attention 的 `O(N²)` 或模型并行的 `O(N)`。
- **进一步加速**：去除原 Transolver 中重复的投影项 `f`（仅保留用于生成权重的 `x`），内存占用降低约 50%，单卡可处理点数提升至 120 万。

## 3. 实验设计
### 数据集与场景
- **标准基准（6 个）**：Elasticity, Plasticity, Airfoil, Pipe, NS2d, Darcy，网格点数从 972 到 16,641，覆盖固体力学、流体力学等。
- **工业级数据集（2 个，百万规模）**：
  - **DrivAerNet++**：汽车外流场，表面网格约 70 万点，完整三维场约 250 万点。
  - **AirCraft**：3D 飞机气动力学，约 30 万点，需预测压力系数、密度、速度等 6 个物理量。

### 评估指标
- 相对 L2 误差（主度量）；对工业任务，进一步计算**升力系数 (C_L)、阻力系数 (C_D)** 及对应的 **R² 决定系数**。

### 对比方法
共对比 20 余个模型，包括：
- 神经算子：FNO, Geo‑FNO, U‑FNO, U‑NO, F‑FNO, LSM, LNO 等。
- Transformer 类：OFormer, FactFormer, GNOT, Transolver。
- 图网络：GraphSAGE, PointNet, Graph U‑Net, MeshGraphNet, GINO 等。

## 4. 资源与算力
- **GPU**：实验使用 **A100 40GB** GPU。单卡极限可处理 120 万点（经优化后）；DrivAerNet++（250 万点）需 4 张 A100 并行训练。
- **训练时长**：
  - 标准基准训练通常设 500 epochs。
  - 工业基准训练 200 epochs；AirCraft 数据集完整训练约需 **10 小时**。
  - 推理速度：单例推理不到 1 秒，对比传统 CFD 求解器（每例 5–6 小时）优势巨大。
- 并行框架的通信开销极小（0.25 MB），不随网格点数增长。

## 5. 实验数量与充分性
- **多数据集覆盖**：6 个标准基准 + 2 个百万级工业数据集，共计 8 套不同物理场景。
- **全面对比**：与 20+ 基线方法比较，涵盖神经算子、Transformer、GNN，且严格控制参数量以保证公平。
- **消融实验**：逐步添加 Ada‑Temp、Rep‑Slice、Speedup 组件，验证每个设计的贡献。
- **机制分析**：
  - 可视化切片权重分布，并计算 KL 散度，说明 Transolver++ 状态更具多样性。
  - 效率分析：对比不同模型的 GPU 内存占用、运行时间，显示 Transolver++ 在速度和内存上的优势。
  - 可扩展性分析：改变训练样本数、网络层数，验证模型性能随数据和参数规模持续提升。
- **补充公平性实验**：对无法处理大规模输入的基线，采用 patch‑infer 再拼接的方式进行对比，并额外测试了 Transolver++ 自己的 patch/unpatch 性能，确保比较客观。
- 总体实验扎实、消融完整，对比基准设置合理，具备充分性。

## 6. 主要结论与发现
- Transolver++ 首次实现**百万级复杂几何 PDE 的精确神经求解**，单卡容量突破 120 万点，多卡可线性扩展。
- 在六个标准基准上相对误差平均降低 **13%**，汽车和飞机工业任务上性能提升超过 **20%**，且对升/阻力系数的预测 R² 接近 1。
- 逼真物理状态机制有效避免了大规模网格下的注意力退化，学习的切片分布与物理量变化剧烈程度高度吻合。
- 并行实现通过仅传递物理状态的通信，实现了**与网格点数解耦的低开销**，大幅优于现有并行注意方案。

## 7. 优点
- **突破规模瓶颈**：首次将神经 PDE 求解器推至工业所需的百万点规模，具有重要应用价值。
- **模块化改良**：以轻量级的局部自适应和重参数化设计，显著提升物理状态学习质量，改动小、收益大。
- **计算高效**：通过去除冗余投影和创新的并行范式，在单卡上内存和速度大幅优化，多卡扩展效率极高。
- **实验全面且客观**：覆盖标准与工业场景，对比方法众多，消融分析详细，并充分考虑了基线无法原生处理大规模输入时的公平比较方式。
- **与工业指标对齐**：不仅预测物理场，还准确计算升/阻力等工程设计关键系数，直接面向应用。

## 8. 不足与局限
- **工业数据集样本量有限**：DrivAerNet++ 仅使用 200 个案例 (190 训练 / 10 测试)，AirCraft 为 150 个案例，存在过拟合风险，泛化能力需更多样例验证。
- **主要为稳态或准静态问题**：工业基准未明确包含时间序列演化，对于后续时时变、大规模非定常问题的适用性尚未展示。
- **并行化强依赖模型结构**：当前高效并行基于 Transolver 特有的“聚合物理状态”设计，迁移至其他架构可能仍需重新设计通信模式。
- **未在超大规模集群测试**：文中最多仅使用 4 张 A100，未展示在数十或上百 GPU 下的线性扩展表现，大规模集群下的通信瓶颈有待验证。
- **Gumbel‑Softmax 带来的随机性**：测试阶段需注意采样噪声，虽然论文未报告相关问题，但在确定性要求高的场景或需额外处理。

（完）
