---
title: "Interpolating Neural Network-Tensor Decomposition (INN-TD): a scalable and interpretable approach for large-scale physics-based problems"
title_zh: 插值神经网络-张量分解：一种面向大规模物理问题可扩展且可解释的方法
authors: "Jiachen Guo, Xiaoyu Xie, Chanwook Park, Hantao Zhang, Matthew J. Politis, Gino Domel, Wing Kam Liu"
date: 2025-05-01
pdf: "https://openreview.net/pdf?id=xfWYB81p5O"
tags: ["query:falling-film"]
score: 4.0
evidence: 结合神经网络与张量分解的可扩展可解释框架，用于PDE描述的物理问题
tldr: 该论文提出插值神经网络与张量分解相结合的框架，解决标准深度学习在求解大规模物理PDE时计算资源高、精度低和可解释性差的问题。通过利用两种方法的优势，该框架在高维物理问题中表现出更好的可扩展性和可解释性，可作为降膜换热等工业CFD问题的潜在高效求解器。
source: ICML-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-icml-2025-xfwyb81p5o/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 760, \"height\": 515, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-xfwyb81p5o/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 584, \"height\": 1151, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-xfwyb81p5o/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 525, \"height\": 367, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-xfwyb81p5o/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 841, \"height\": 447, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-xfwyb81p5o/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 636, \"height\": 1752, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-xfwyb81p5o/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 554, \"height\": 404, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-xfwyb81p5o/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 847, \"height\": 467, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-xfwyb81p5o/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1684, \"height\": 1106, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-xfwyb81p5o/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1562, \"height\": 1294, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-xfwyb81p5o/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1784, \"height\": 474, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-xfwyb81p5o/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1759, \"height\": 708, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-xfwyb81p5o/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1754, \"height\": 525, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-xfwyb81p5o/fig-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1523, \"height\": 680, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-xfwyb81p5o/fig-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 1676, \"height\": 561, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-xfwyb81p5o/fig-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 1464, \"height\": 687, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-xfwyb81p5o/fig-016.webp\", \"caption\": \"\", \"page\": 0, \"index\": 16, \"width\": 1500, \"height\": 779, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-xfwyb81p5o/fig-017.webp\", \"caption\": \"\", \"page\": 0, \"index\": 17, \"width\": 1778, \"height\": 867, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-icml-2025-xfwyb81p5o/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 794, \"height\": 519, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xfwyb81p5o/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 902, \"height\": 457, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xfwyb81p5o/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 900, \"height\": 458, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xfwyb81p5o/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 901, \"height\": 179, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xfwyb81p5o/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1430, \"height\": 423, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xfwyb81p5o/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1752, \"height\": 458, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xfwyb81p5o/table-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1739, \"height\": 465, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xfwyb81p5o/table-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1730, \"height\": 463, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xfwyb81p5o/table-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1744, \"height\": 465, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xfwyb81p5o/table-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1769, \"height\": 494, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xfwyb81p5o/table-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1243, \"height\": 241, \"label\": \"Table\"}]"
motivation: 标准深度学习求解PDE面临资源消耗大、精度有限和黑箱不可解释问题。
method: 融合插值神经网络与张量分解，构建可扩展且可解释的物理求解框架。
result: 在大规模高维物理问题上实现高精度与可解释性，优于纯深度学习方法。
conclusion: 为工业级CFD等物理问题提供了一种兼顾效率与可解释性的方案。
---

## Abstract
Deep learning has been extensively employed as a powerful function approximator for modeling physics-based problems described by partial differential equations (PDEs). Despite their popularity, standard deep learning models often demand prohibitively large computational resources and yield limited accuracy when scaling to large-scale, high-dimensional physical problems. Their black-box nature further hinders their application in industrial problems where interpretability and high precision are critical. To overcome these challenges, this paper introduces Interpolating Neural Network-Tensor Decomposition (INN-TD), a scalable and interpretable framework that has the merits of both machine learning and finite element methods for modeling large-scale physical systems.  By integrating locally supported interpolation functions from finite element into the network architecture, INN-TD achieves a sparse learning structure with enhanced accuracy, faster training/solving speed, and reduced memory footprint. This makes it particularly effective for tackling large-scale high-dimensional parametric PDEs in training, solving, and inverse optimization tasks in physical problems where high precision is required.

---

## 论文详细总结（自动生成）

## 论文总结：插值神经网络‑张量分解 (INN‑TD) —— 一种面向大规模物理问题可扩展且可解释的方法

### 1. 核心问题与整体背景
- 深度学习方法已被广泛用于近似由偏微分方程 (PDE) 描述的物理问题，但其面临以下挑战：
  - **大规模高维问题**：标准深度学习模型 (如 MLP) 需要极大的计算资源和内存，精度有限。
  - **黑箱性质**：缺乏可解释性，难以满足航空航天、半导体制造、地震工程等对高精度和高可靠性要求苛刻的工业场景。
  - **数据驱动训练与无数据求解的差距**：纯数据驱动方法需大量高保真仿真数据，成本高昂；无数据求解器 (如PINN) 常面临精度低、不稳定、收敛性差、难以处理高维参数化PDE等问题。
- 本文旨在融合有限元插值理论的可解释性、收敛性以及张量分解的维度压缩能力，提出一个统一的框架，在训练、求解和反问题优化中同时实现高精度、可扩展性和可解释性。

### 2. 方法论
**核心思想**：将有限元中局部支撑的插值函数 (C‑HiDeNN) 与张量分解 (Canonical Polyadic, CP) 相结合，构建一种稀疏、可解释的神经网络结构。

**关键技术细节**：
- **C‑HiDeNN 插值**：采用一种广义有限元插值函数作为单变量基函数。它保留了传统有限元的优点：
  - Kronecker delta 性质，自动满足 Dirichlet 边界条件。
  - 局部支持、分区统一，便于采用高斯积分进行数值积分。
  - 可通过超参数 (patch size `s`、多项式阶数 `p`、扩张参数 `a`) 控制插值平滑度和精度。
- **张量分解近似**：将多变量函数近似为若干秩‑1 项的乘积和：
  \[
  u(x_1,\dots,x_D) \approx \sum_{m=1}^M \prod_{d=1}^D f^{(m)}_d(x_d)
  \]
  在每个单变量函数 \(f^{(m)}_d\) 中使用 C‑HiDeNN 插值，最终模型参数为各维度的节点值向量 \(U^{(m)}\)。
- **训练与求解**：
  - **数据驱动训练**：采用均方误差损失，可使用 boosting 式逐模式训练或 all‑at‑once 同时优化所有模式参数。训练代码公开。
  - **无数据求解**：利用 PDE 残差的加权积分形式 (Galerkin 方法)，将 PDE 转化为各维度一维积分，并通过子空间迭代交替求解稀疏线性系统。由于张量分解结构，用一维积分规避维度灾难，使得极精细网格下仍可高效求解。使用 boosting 算法逐模式添加并交替优化维度。求解代码公开。
- **可解释性**：
  - 网格密度 `n_d` 控制各维度的分辨率。
  - 模式数 `M` 与奇异值分解的奇异值数量相关 (当 D=2)。
  - 超参数 `s`, `p` 可针对局部非线性区域调整，实现局部加密和高阶光滑。
  - 整体可视为一种结构可解释的 “裁剪 MLP”(见论文图 9)。

### 3. 实验设计
实验覆盖三类任务，均与相关方法对比：

| 任务 | 问题描述 | 对比方法 | 评估指标 |
|------|---------|----------|---------|
| 数据驱动训练 | 学习含参数热传导PDE的解映射 `(x,y,k,P,t) → u`，训练集比例 10%/30%/100%，16个高斯热源 | MLP, SIREN, KAN | 训练/测试 RMSE |
| 无数据求解 (高维Poisson) | 求解 2D、5D、10D Poisson方程，域大小 `[0,1]^D` 和 `[0,12]^D` (高频) | CP-PINN, KAN | 相对 L2 误差、GPU 时间 |
| 无数据求解 (Helmholtz) | 2D Helmholtz方程 (PINN难以训练) | – (自身收敛性分析) | 点对点误差、收敛性 |
| 无数据求解 (S‑P‑T PDE) | 6D 空间‑参数‑时间热传导问题 `(x,y,z,k,P,t)` | FEM 作为 ground truth | 相对 L2 误差 |
| 逆优化 | 利用已求解的S‑P‑T模型，通过自动微分恢复参数 `(k,P)` | – | 参数误差、预测 L2 误差 |

### 4. 资源与算力
- 所有实验均在**单张 NVIDIA RTX A6000 GPU** 上运行。
- 训练任务中，INN‑TD 使用 12,300 个参数，约 100 epochs。
- 无数据求解任务：
  - 2D Poisson: 0.81 s；10D Poisson: 57.43 s。
  - 6D S‑P‑T 求解共用 155 s。
- 相对于对比方法 (CP‑PINN、KAN)，INN‑TD 在 GPU 时间和显存占用上均显著更优 (如10D时 INN‑TD 仅用 760 MB 显存，而 KAN 需 9988 MB)。

### 5. 实验数量与充分性
- **实验组数**：
  - 训练任务：3 种训练数据量 × 4 种模型，重复多次 (RMSE 表报告了均值与标准差)。
  - 求解任务：2 个域大小 × 3 种维度 (2,5,10) 对比 CP‑PINN 和 KAN，并重复 10 次统计。
  - Helmholtz 和 4D 时空方程收敛性验证：不同超参数 `s`、`p` 和模式数下的误差、时间、显存统计，每组 10 次。
  - S‑P‑T 6D 问题及逆优化 100 次随机参数测试。
  - 附录中额外验证了向量弹性问题、算子学习任务。
- **客观性与公平性**：
  - 对比方法均采用公开实现或合理配置 (如 KAN 使用 LBFGS、CP‑PINN 配置详)。
  - 对于 CP‑PINN 和 KAN 的潜在内存/时间劣势，文中均注明原因 (如增加 collocation 点数或降低 batch size)。
  - 多次实验报告均值和标准差，阴影区域表示标准差，结果可重复性较好。

### 6. 主要结论与发现
- **精度优势**：在数据驱动训练中，INN‑TD 的测试误差比 MLP、SIREN、KAN 低一个量级；在无数据求解中，比其他模型低数个数量级 (如 10D Poisson 下 INN‑TD 误差 ~1e‑8，而 CP‑PINN/KAN 仅达到 5e‑3～1e‑4 水平)。
- **收敛性保证**：通过增加模式数/网格点，误差单调下降，且可通过 `s`、`p` 控制收敛速率，这是黑箱模型所不具备的。
- **高效处理高维问题**：利用张量分解避免维度灾难，10D 问题仍可在 1 分钟内完成，显存占用极低。
- **可解释性支撑复杂任务**：非均匀网格和局部高阶插值可针对物理特征精细化建模；Dirichlet 边界自动满足。
- **框架统一**：同一架构可无缝切换于训练、无数据求解和逆优化，无需重新设计模型。

### 7. 优点
- **融合数值分析与机器学习的创新**：将有限元的局部性、Krorder delta、分区统一等强先验融入神经网络，兼顾精度、可解释性和可扩展性。
- **克服维度灾难**：一维积分的 Galerkin 形式 + 张量分解，使高维参数化 PDE 求解实际可行。
- **显式可解释结构**：网格、模式数、超参数 `s`、`p` 都有物理含义，便于工程师按精度需求设计模型。
- **收敛性与可靠性**：展示了模型复杂度增加时误差稳定下降的收敛属性，增强了工业部署的可信度。
- **开源的训练和求解代码**，提高了可复现性。

### 8. 不足与局限
- **超参数依赖**：C‑HiDeNN 的超参数 (`s`、`a`、`p`)、模式数、网格划分仍需手动设置或经验调优，缺乏自动选择策略。
- **实验场景相对理想化**：PDE 示例多为线性 Poisson/热传导，在强非线性、复杂边界、多物理场耦合问题上的泛化能力尚未验证。
- **对比方法有限**：训练任务仅比较了 MLP、SIREN、KAN，未涵盖更多现代算子网络 (如 DeepONet、FNO)；无数据求解未与 hp‑VPINN 等变分 PINN 对比。
- **反问题采用先求正向模型再优化的两步法**，若正向模型误差积累可能影响参数估计精度。
- **向量/张量场求解**仅于附录展示，主体实验均为标量场，实践中多场耦合可能增加复杂度。
- **训练数据规模**：数据驱动任务中最大仅为 100% 数据集，并未探究在小样本或高噪声下的鲁棒性。
- **硬件限制讨论不足**：虽提及使用单 GPU，但对于工业超大规模问题 (例如 10^6 自由度) 的强可伸缩性尚无证明。

（完）
