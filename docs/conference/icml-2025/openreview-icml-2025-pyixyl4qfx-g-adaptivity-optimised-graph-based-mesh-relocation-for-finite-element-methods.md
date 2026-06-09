---
title: "G-Adaptivity: optimised graph-based mesh relocation for finite element methods"
title_zh: "G-Adaptivity: 优化的基于图的有限元网格重定位"
authors: "James Rowbottom, Georg Maierhofer, Teo Deveney, Eike Hermann Müller, Alberto Paganini, Katharina Schratz, Pietro Lio, Carola-Bibiane Schönlieb, Chris Budd"
date: 2025-05-01
pdf: "https://openreview.net/pdf?id=pyIXyl4qFx"
tags: ["query:falling-film"]
score: 4.0
evidence: 基于图的有限元网格重定位可提高CFD模拟效率
tldr: 针对传统r-自适应网格重定位需要求解非线性网格偏微分方程、计算成本高的问题，该论文提出用图神经网络直接优化网格点位置，绕过传统方法。实验表明其在有限元分析中能提升精度和效率，有望加速降膜流动的CFD模拟网格生成。
source: ICML-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-icml-2025-pyixyl4qfx/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 798, \"height\": 870, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pyixyl4qfx/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 826, \"height\": 621, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pyixyl4qfx/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 747, \"height\": 277, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pyixyl4qfx/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 822, \"height\": 400, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pyixyl4qfx/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 799, \"height\": 1308, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pyixyl4qfx/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 863, \"height\": 678, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pyixyl4qfx/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 822, \"height\": 464, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pyixyl4qfx/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 832, \"height\": 632, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pyixyl4qfx/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1632, \"height\": 1636, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pyixyl4qfx/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1599, \"height\": 796, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pyixyl4qfx/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1107, \"height\": 1196, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-pyixyl4qfx/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1560, \"height\": 2010, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-icml-2025-pyixyl4qfx/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 904, \"height\": 594, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pyixyl4qfx/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 886, \"height\": 516, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pyixyl4qfx/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 884, \"height\": 306, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pyixyl4qfx/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1397, \"height\": 337, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pyixyl4qfx/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1252, \"height\": 285, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pyixyl4qfx/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1089, \"height\": 323, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pyixyl4qfx/table-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 877, \"height\": 325, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pyixyl4qfx/table-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1315, \"height\": 175, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-pyixyl4qfx/table-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 870, \"height\": 357, \"label\": \"Table\"}]"
motivation: 降低有限元方法中网格重定位的计算开销。
method: 训练图神经网络直接优化网格点位置，替代传统网格偏微分方程求解。
result: 在基准测试上获得更优的精度-成本权衡。
conclusion: 为有限元模拟提供了一种高效网格优化工具，可间接辅助CFD计算。
---

## Abstract
We present a novel, and effective, approach to achieve optimal mesh relocation in finite element methods (FEMs). The cost and accuracy of FEMs is critically dependent on the choice of mesh points. Mesh relocation (r-adaptivity) seeks to optimise the mesh geometry to obtain the best solution accuracy at given computational budget. Classical r-adaptivity relies on the solution of a separate nonlinear ``meshing'' PDE to determine mesh point locations. This incurs significant cost at remeshing, and relies on estimates that relate interpolation- and FEM-error. Recent machine learning approaches have focused on the construction of fast surrogates for such classical methods. Instead, our new approach trains a graph neural network (GNN) to determine mesh point locations by directly minimising the FE solution error from the PDE system Firedrake to achieve higher solution accuracy. Our GNN architecture closely aligns the mesh solution space to that of classical meshing methodologies, thus replacing classical estimates for optimality with a learnable strategy. This allows for rapid and robust training and results in an extremely efficient and effective GNN approach to online r-adaptivity. Our method outperforms both classical, and prior ML, approaches to r-adaptive meshing. In particular, it achieves lower FE solution error, whilst retaining the significant speed-up over classical methods observed in prior ML work.

---

## 论文详细总结（自动生成）

# 论文总结：G-Adaptivity: 优化的基于图的有限元网格重定位

## 1. 论文的核心问题与整体含义
- **研究背景**：有限元方法 (FEM) 是科学计算的核心工具，其计算成本与精度高度依赖于网格点的分布。传统 r‑自适应网格重定位通过求解额外的非线性“网格生成”偏微分方程 (如 Monge‑Ampère 方程) 来调整网格点位置，但这会带来显著的计算开销，且依赖插值误差与 FEM 误差之间的间接估计。
- **核心问题**：如何以更低的计算成本获得比传统方法更优的网格，从而直接降低 FEM 解的误差。
- **整体含义**：本文提出一种全新的、基于图神经网络 (GNN) 的 r‑自适应框架 (G‑adaptivity)，通过直接最小化 FEM 解的误差来学习网格点位移，绕过了传统方法的低效代理方程，在保持快速推理的同时实现了超越经典方法和先前 ML 方法的精度。

## 2. 论文提出的方法论
- **核心思想**：将网格重定位视为一个可学习的变形过程，训练一个 GNN 直接预测新的网格点坐标，使得在该网格上求解的 FEM 结果与解析解（或细网格参考解）之间的 \(L^2\) 误差最小。
- **关键技术细节**：
  - **扩散变形器 (Diffformer)**：使用基于扩散过程的 GNN 块，其节点更新形式为 \(\dot{Z}(\tau) = (A_\theta(X^k) - I) Z(\tau)\)，其中 \(A_\theta\) 是行随机注意力矩阵。该架构模拟各向异性扩散，可将节点拉向邻居凸包内部，从而**理论上保证网格不会缠绕** (定理4.2)。
  - **输入特征**：输入包含当前网格坐标以及由 FEM 解的 Hessian 矩阵恢复的曲率信息，通过特征提取器编码后馈入 GNN。
  - **可微 FEM 与伴随梯度**：利用 `Firedrake` 可微框架及其自动伴随 (`pyadjoint`) 高效计算 FEM 误差关于网格坐标的梯度，避免了手工推导伴随方程的巨大工作量。
  - **损失函数**：\( \mathcal{L}_\theta = E(\mathcal{M}_\theta) + \mathcal{L}_{\text{equi}}(\mathcal{M}_\theta) \)，其中 \(E\) 为 FEM 解的 \(L^2\) 误差，\(\mathcal{L}_{\text{equi}}\) 为基于监视函数（如解的梯度大小）的等分布正则化项，鼓励网格向解变化剧烈区域集中。
- **算法流程**：给定初始均匀网格和 PDE 源项/边界条件，先用粗网格求得 FEM 解并提取 Hessian；将其输入 GNN（多个 Diffformer 块）得到变形后网格坐标；在该变形网格上再次求解 FEM 并计算与参考解的误差；通过 Firedrake 伴随计算网格坐标梯度，反向传播更新 GNN 参数。推理时只需一次前向传播，无需重复求解伴随方程。

## 3. 实验设计
- **数据集与场景**：
  - 泊松方程：正方形域 (100 训练 /100 测试高斯源项)；凸多边形域 (同样高斯源项)；五个非凸几何形状。
  - Burgers 方程：二维方形域上的粘性 Burgers 方程，训练使用随机高斯初值，评估使用 rollout（每2步重网格）以及长时步（10步）重网格场景。
  - Navier‑Stokes 方程：圆柱绕流经典问题 (多连通域)，训练/测试取自 \(t\in[1,4]\) 的随机快照。
  - 3D 泊松方程：\(10\times10\times10\) 单位立方体，高斯解。
  - 可扩展性：在 15×15 网格上训练，直接推理至 60×60 和 150×150 网格。
- **基准与对比方法**：
  - 经典 Monge‑Ampère (MA) 方法（由 `Movement` 包实现）。
  - ML 代理方法 UM2N（原始训练）。
  - UM2N‑G：用本文提出的正则化 FEM 损失重新训练的 UM2N。
  - 直接优化 (DirectOpt)：对网格坐标直接做梯度优化（仅用于展示理论上界，非实用方法）。
- **评价指标**：相对 \(L^2\) 误差减少百分比 (ER)、网格重定位时间 (ms)、网格质量 (纵横比)。

## 4. 资源与算力
- 论文并未明确提及所用 GPU 型号、数量或具体训练时长。仅说明 G‑Adapt 和 UM2N‑G 使用 Adam 优化器、学习率 0.001，训练 300 个 epoch（UM2N 原始训练 1000 个 epoch）。因此，无法从文中直接获知算力需求。

## 5. 实验数量与充分性
- 实验覆盖了**二维静态（泊松）、二维瞬态（Burgers）、二维不可压流动（Navier‑Stokes）、三维静态（泊松）**四种 PDE 场景，并在**凸域、多边形域、非凸域、多连通域**等多种几何上进行测试。
- 进行了**超分辨率**（训练在低分辨率，测试在高分辨率）和**可扩展性**实验（最大 150×150，22,500 节点），验证了 GNN 的归纳能力。
- 包含了**消融/敏感性分析**：扩散时间步长与滚动步数对误差和推理时间的影响、等分布正则化权重的敏感性。
- 所有实验均**重复 5 次**，提供均值和标准差，具备统计意义。
- 对比了**经典方法、先前 ML 方法、本文方法、以及理论最优直接优化**，比较维度全面。
- 总体而言，实验设计充分、客观，覆盖了主流 PDE 与几何类型，且与当前最优方法进行了公平对比（除 MA 在多连通域无法收敛外）。

## 6. 论文的主要结论与发现
- G‑adaptivity 是**首个在误差减少上超越经典 Monge‑Ampère 方法**的 ML 网格重定位方法，同时保留了 ML 方法在推理速度上的巨大优势（例如在泊松方程上误差减少 21.01% vs. MA 的 12.69%，推理时间 88 ms vs. 3780 ms）。
- 直接优化 FEM 误差（而非代理误差估计）能有效提升网格质量；扩散变形器架构确保了**无网格缠绕**，并结合等分布正则化使生成的网格更规整。
- 方法具有**广泛的适用性**：可处理瞬态、非线性、多连通域以及三维问题，且在未见过的更高分辨率网格上仍能有效工作。
- 与先前 ML 方法（UM2N）相比，无论在原始训练还是同一损失下训练，G‑adaptivity 均表现出更优或相当的误差减少和更好的鲁棒性（尤其在分布外数据上）。

## 7. 优点
- **方法论创新**：首次将可微 FEM 与 GNN 结合，直接以 FEM 误差为优化目标，突破了传统基于代理方程或监督学习的思路。
- **架构优势**：扩散变形器从理论上保证非交错网格，同时行随机注意力矩阵与经典 MA 方法的理论对齐，赋予模型良好的归纳偏置。
- **高效低成本**：推理时仅需 GNN 前向传播，无需再次求解伴随方程或网格 PDE，网格重定位速度远快于传统方法。
- **可扩展与通用**：证明了在二维/三维、凸/非凸/多连通域、静态/瞬态问题上的有效性，且可通过低分辨率训练即插即用于高分辨率。
- **工程贡献**：代码开源，与 Firedrake 深度集成，为学术与工程应用提供了完整工具链。

## 8. 不足与局限
- **泛化能力受限**：论文明确指出 ML 类方法在分布外数据（如 PDE 解的特征尺度与训练集显著不同）上性能可能下降，这是目前 ML 自适应网格的共同挑战。
- **依赖参考解**：虽然推理时不需要参考解，但训练时仍需通过细网格 FEM 计算获得“真实”误差用于监督，这可能限制其在完全无参考解的场景中的应用。
- **高阶元支持未深入**：文中主要使用线性元（泊松、Burgers）或 Taylor‑Hood 元（Navier‑Stokes），对于高阶元的 Hessian 恢复及梯度计算虽提及但未系统评估。
- **三维及大规模案例有限**：虽然初步展示了 3D 效果，但仅在 10³ 网格的小规模问题上验证，缺乏更大规模或更复杂三维流动的评估。
- **计算资源与训练成本未报告**：训练所需的 GPU 资源、训练时长等信息缺失，使得难以评估方法在实际部署中的总体成本。
- **对比方法有限**：除了 UM2N 外，未与其他最新的深度学习网格自适应方法进行对比。
- **等分布正则化器依赖手工设计的监视函数**，虽然有效，但可能不如学习得到的先验灵活。

（完）
