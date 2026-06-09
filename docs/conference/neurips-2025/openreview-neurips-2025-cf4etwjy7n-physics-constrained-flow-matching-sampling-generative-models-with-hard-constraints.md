---
title: "Physics-Constrained Flow Matching: Sampling Generative Models with Hard Constraints"
title_zh: 物理约束流匹配：带硬约束的生成模型采样
authors: "Utkarsh Utkarsh, Pengfei Cai, Alan Edelman, Rafael Gomez-Bombarelli, Christopher Vincent Rackauckas"
date: 2025-09-18
pdf: "https://openreview.net/pdf?id=cf4etwjY7n"
tags: ["query:falling-film"]
score: 4.0
evidence: 物理约束流匹配在生成式PDE模型中强制执行守恒律，有助于CFD
tldr: 该文提出物理约束流匹配(PCFM)，一种零样本推理框架，可在预训练的基于流的生成模型采样过程中持续施加任意非线性物理约束。与传统软惩罚不同，PCFM保证硬约束满足，为机械、热传导等由偏微分方程支配的系统提供了物理一致的生成模拟，对降膜换热等两相流CFD具有潜在价值。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-neurips-2025-cf4etwjy7n/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 722, \"height\": 413, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-cf4etwjy7n/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1408, \"height\": 477, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-cf4etwjy7n/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1437, \"height\": 424, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-cf4etwjy7n/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1332, \"height\": 374, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-cf4etwjy7n/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1369, \"height\": 853, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-cf4etwjy7n/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1429, \"height\": 760, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-cf4etwjy7n/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1413, \"height\": 462, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-cf4etwjy7n/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1418, \"height\": 377, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-cf4etwjy7n/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1375, \"height\": 508, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-neurips-2025-cf4etwjy7n/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1444, \"height\": 249, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-cf4etwjy7n/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1443, \"height\": 272, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-cf4etwjy7n/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1448, \"height\": 1125, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-cf4etwjy7n/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1114, \"height\": 473, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-cf4etwjy7n/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1450, \"height\": 425, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-cf4etwjy7n/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1432, \"height\": 474, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-cf4etwjy7n/table-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1145, \"height\": 346, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-cf4etwjy7n/table-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1079, \"height\": 340, \"label\": \"Table\"}]"
motivation: 现有生成式物理模型依赖软惩罚或架构偏差，无法保证质量及能量守恒等硬约束。
method: 提出物理约束流匹配(PCFM)，在采样过程中通过基于物理的校正逐步引导，确保中间状态满足守恒律。
result: 在多个PDE问题上实现了零样本且物理一致的模拟，优于仅靠软约束的方法。
conclusion: PCFM为需要严格物理一致性的科学模拟提供了新工具，有助于构建可靠的降膜蒸发仿真模型。
---

## Abstract
Deep generative models have recently been applied to physical systems governed by partial differential equations (PDEs), offering scalable simulation and uncertainty-aware inference. However, enforcing physical constraints, such as conservation laws (linear and nonlinear) and physical consistencies, remains challenging. Existing methods often rely on soft penalties or architectural biases that fail to guarantee hard constraints. In this work, we propose Physics-Constrained Flow Matching (PCFM), a zero-shot inference framework that enforces arbitrary nonlinear constraints in pretrained flow-based generative models. PCFM continuously guides the sampling process through physics-based corrections applied to intermediate solution states, while remaining aligned with the learned flow and satisfying physical constraints. Empirically, PCFM outperforms both unconstrained and constrained baselines on a range of PDEs, including those with shocks, discontinuities, and sharp features, while ensuring exact constraint satisfaction at the final solution. Our method provides a flexible framework for enforcing hard constraints in both scientific and general-purpose generative models, especially in applications where constraint satisfaction is essential.

---

## 论文详细总结（自动生成）

### 1. 论文的核心问题与整体含义
- **研究背景与动机**：深度生成模型（尤其是流匹配）已开始用于物理系统（如 PDE 求解），但如何**严格保证守恒律、边界条件等物理硬约束**仍是一大挑战。
- **现有局限**：主流方法依赖软惩罚（如 PINN 损失）或网络架构偏置，**无法保证约束精确满足**；另一些方法（如 ECI）仅能处理简单的线性、非重叠约束。
- **整体含义**：本文提出 **Physics-Constrained Flow Matching (PCFM)**，一种**零样本推理框架**，能够在预训练的流匹配生成模型中**施加任意非线性等式硬约束**，无需重新训练或修改模型结构。

### 2. 论文提出的方法论
- **核心思想**：在采样过程中，通过**投影到约束流形 + OT（最优传输）插值反向传播 + 松弛校正 + 最终投影**的方式，持续引导中间状态满足物理约束，最终生成精确满足约束的解。
- **关键技术细节**：
  - **正向射击与 Gauss‑Newton 投影**：将当前状态沿流推至终点 `u₁`，然后计算约束残差和雅可比，通过 `u_proj = u₁ - Jᵀ(JJᵀ)⁻¹h(u₁)` 投影到约束切空间。
  - **反向更新**：为避免 ODE 反向积分的不稳定性，使用 **OT 位移插值直线路径** (`u_proj - u₀`) 近似反向流，得到中间时间点 `û_{τ'}`。
  - **松弛约束校正**：在 `û_{τ'}` 处添加惩罚项，优化 `min ‖u - û_{τ'}‖² + λ‖h(u + (1-τ')v_θ)‖²`，增强数值鲁棒性。
  - **最终投影**：若剩余残差较大，求解约束优化问题 `min ‖u' - u₁‖² s.t. h(u') = 0`，利用自定义的批处理 Schur 补求解器确保精度。
- **算法流程**：每步流积分的前向、投影、反向近似、校正，步进迭代；终点处可附加最终硬投影。
- **公式与支持**：理论证明（附录 A）在满秩雅可比假设下，最终投影能收敛到满足 `h(u)=0` 的解；ECI 可视为 PCFM 在 λ=0 且约束为线性时的特例。

### 3. 实验设计
- **数据集/场景**（所有 PDE 数据集均构建双自由度变化）：
  - **Heat Equation**（2D，周期边界，线性全局质量守恒 + 初始条件）。
  - **Navier‑Stokes**（3D 涡量方程，周期边界，线性全局质量守恒 + 初始条件）。
  - **Reaction‑Diffusion**（非线性质量守恒 + Neumann 边界 + 初始条件）。
  - **Burgers Equation**（混合 Dirichlet/Neumann，非线性质量守恒，带激波；分别固定初始条件或边界条件）。
- **Benchmark 方法**：ECI、DiffusionPDE、D-Flow、PDM、Vanilla FFM（无约束）。
- **评价指标**：均值均方误差(MMSE)、标准差均方误差(SMSE)、约束误差(CE)、Fréchet Poseidon 距离(FPD)、功率谱 MSE 等。
- **对比方式**：所有方法使用**同一预训练 FFM 模型**，仅改变推理采样策略，保证公平。

### 4. 资源与算力
- **训练资源**：
  - Heat、Reaction‑Diffusion、Burgers：**1 块 NVIDIA V100**，各训练 20,000 步。
  - Navier‑Stokes：**4 块 NVIDIA A100**，训练 500,000 步。
- **推理资源**：在单块 V100 上完成全部推理成本计时与内存分析（见表 4），PCFM 比 D‑Flow 快 4‑6 倍，额外开销相对合理。

### 5. 实验数量与充分性
- **主要实验**：
  - 4 个 PDE 系统 ×（至少 2 种约束配置）= 8+ 组主实验（见表 3）。
  - 与 5 种基线方法对比，覆盖线性和非线性、全局和局部约束。
- **消融实验**：
  - 中间投影的必要性（表 6）。
  - 约束点数量增加对质量的影响（图 4）。
  - λ 惩罚权值在不同流步数下的作用（图 9）。
  - 加入 TV 约束的影响（表 7）。
  - 分布外（OOD）约束泛化性测试（表 8）。
- **充分性**：实验覆盖多种 PDE 类型、约束形式和难度，消融充足，指标全面，评估客观。

### 6. 论文的主要结论与发现
- PCFM 在**所有线性/非线性约束**任务中均实现**机器零残差**，同时 MMSE、SMSE、FPD 结果**全面优于**或与最强基线持平。
- 特别在**激波、间断**等困难场景下，PCFM 能准确捕获尖锐特征，而其他方法往往平滑或失效。
- 添加互补的硬约束（如更多配点）可**持续提升生成质量**，避免了软约束方法中常见的竞争退化问题。
- 所提出的 OT 反向更新可避免传统 ODE 反向积分的不稳定性，兼具高效与鲁棒。
- 最终投影步骤的 Schur 补批处理求解器开销极小（仅占总时间的 1‑3%），实际可用性高。

### 7. 优点
- **零样本、即插即用**：无需重训或修改预训练流匹配模型，直接后处理强制执行物理约束。
- **支持任意非线性等式约束**：覆盖质量守恒、边界条件、局部通量等，远超前人局限于线性约束的工作。
- **强理论支撑**：切空间投影、OT 插值合理性论证，以及收敛性保证。
- **数值工具完善**：提供 Python/Julia 开源代码，包含批处理可微 Schur 求解器，方便集成到深度学习管线。
- **实验丰富且对比公平**：统一预训练模型，多指标、多基线，消融系统。

### 8. 不足与局限
- **仅支持等式约束**：无法直接处理不等式约束（如 TVD 中的上界），需未来扩展。
- **雅可比结构未充分利用**：当约束维度很大时，`m×m` 矩阵求逆可能成为瓶颈；可利用稀疏或隐式结构改进。
- **依赖约束的显式形式**：需要能够写出并求导约束函数 `h(u)`，对完全隐式的复杂物理条件可能不适用。
- **仅在 PDE 数据集上验证**：尚未在其他科学领域（如分子设计、天体物理）展示，通用性待进一步验证。
- **反向近似依赖 OT 路径线性性**：在极度非线性流或大时间步长下，近似误差可能累积，虽然 λ 提供补偿，但最优性需进一步理论分析。

（完）
