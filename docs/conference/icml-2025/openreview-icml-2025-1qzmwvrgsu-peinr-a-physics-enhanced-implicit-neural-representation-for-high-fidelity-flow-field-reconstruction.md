---
title: "PEINR: A Physics-enhanced Implicit Neural Representation for High-Fidelity Flow Field Reconstruction"
title_zh: "PEINR: 面向高保真流场重建的物理增强隐式神经表示"
authors: "Liming Shen, Liang Deng, Chongke Bi, Yu Wang, Xinhai Chen, Yueqing Wang, Jie Liu"
date: 2025-05-01
pdf: "https://openreview.net/pdf?id=1QZMWVrgsU"
tags: ["query:falling-film"]
score: 7.0
evidence: 物理增强的隐式神经表示用于从CFD数据重建高保真流场，可应用于降膜模拟
tldr: 针对隐式神经表示在流场重建中缺乏标准数据集和忽略物理规律的问题，论文发布5.4TB的HFR-Beach CFD数据集，并提出物理增强的INR框架PEINR。实验表明该方法能精细捕捉流场细节和时空动态，为降膜蒸发等两相流CFD模拟提供了高保真代理模型基础。
source: ICML-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-icml-2025-1qzmwvrgsu/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 850, \"height\": 573, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-1qzmwvrgsu/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1777, \"height\": 484, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-1qzmwvrgsu/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1770, \"height\": 404, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-1qzmwvrgsu/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1780, \"height\": 890, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-1qzmwvrgsu/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1773, \"height\": 362, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-1qzmwvrgsu/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 869, \"height\": 329, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-1qzmwvrgsu/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 862, \"height\": 751, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-1qzmwvrgsu/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1764, \"height\": 1141, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-1qzmwvrgsu/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1772, \"height\": 720, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-1qzmwvrgsu/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1777, \"height\": 485, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-icml-2025-1qzmwvrgsu/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1744, \"height\": 431, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-1qzmwvrgsu/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1746, \"height\": 852, \"label\": \"Table\"}]"
motivation: 解决INR在流场重建中标准数据集缺失和物理约束不足的问题。
method: 构建大规模CFD数据集，并提出融入物理先验的隐式神经表示。
result: 在重建精度和细节捕捉上超越现有INR方法。
conclusion: 为基于数据的流场重建提供基准和强基线，有望促进降膜流动CFD的代理模型研究。
---

## Abstract
Implicit neural representation (INR) has now been thrust into the limelight with its flexibility in high-fidelity flow field reconstruction tasks. However, the lack of standard benchmarking datasets and the grid independence assumption for INR-based methods hinder progress and adoption in real-world simulation scenarios. Moreover, naive adoptions of existing INR frameworks suffer from limited accuracy in capturing fine-scale structures and spatiotemporal dynamics. Tacking these issues, we first introduce HFR-Beach, a 5.4 TB public large-scale CFD dataset with 33,600 unsteady 2D and 3D vector fields for reconstructing high-fidelity flow fields. We further present PEINR, a physics-enhanced INR framework, to enrich the flow fields by concurrently enhancing numerical-precision and grid-resolution. Specifically, PEINR is mainly composed of physical encoding and transformer-based spatiotemporal fuser (TransSTF). Physical encoding decouples temporal and spatial components, employing Gaussian coordinate encoding and localized encoding techniques to capture the nonlinear characteristics of spatiotemporal dynamics and the stencil discretization of spatial dimensions, respectively. TransSTF fuses both spatial and temporal information via transformer for capturing long-range temporal dependencies. Qualitative and quantitative experiments and demonstrate that PEINR outperforms state-of-the-art INR-based methods in reconstruction quality.

---

## 论文详细总结（自动生成）

```markdown
# PEINR: 面向高保真流场重建的物理增强隐式神经表示

## 1. 论文的核心问题与整体含义

- **研究背景与动机**  
  高保真流场在理解流体行为中至关重要，传统计算流体力学（CFD）通过提高网格分辨率和数值精度获取精细结构，但计算成本极高。  
  隐式神经表示（INR）能以连续函数形式学习流场，支持任意网格类型，避免了卷积神经网络（CNN）局限于笛卡尔网格和图神经网络（GNN）信息传播困难的问题。

- **核心问题**  
  1. **标准数据集缺失**：现有 INR 方法缺乏公开基准，且隐含假设“网格独立性”（即不同网格分辨率下同一位置的物理量不变），但在真实模拟中该假设不成立。  
  2. **时空不平衡**：实际仿真因 I/O 瓶颈仅保存部分时间步，时空复杂度严重失衡，现有方法简单耦合时空坐标，难以模拟复杂时空动力学。  
  3. **频谱偏差**：INR 倾向学习低频信息，难以捕捉高保真流场中丰富的高频精细结构。

- **整体含义**  
  本文旨在构建大规模流场重建基准数据集（HFR‑Bench），并提出物理增强的 INR 框架（PEINR），同时提升数值精度和网格分辨率，突破现有方法在真实 CFD 场景下的局限性。

## 2. 论文提出的方法论

PEINR 的整体框架包括四个组成部分：逆问题输入编码、物理编码、TransSTF模块和逆问题求解。

- **逆问题建模与误差场学习**  
  不再直接映射从低精度到高精度流场，而是学习低精度与高精度流场之间的**误差场** \(\delta F = F_H - F_B\)（其中 \(F_B\) 为低精度场上采样后的结果）。PEINR 的目标是建立映射：
  \[
  \delta F(x,y,z,t) \approx \mathcal{N}(\Phi(t),\Psi(\vec{C}),\theta)
  \]
  最终高保真解由误差场与低精度上采样场相加得到。

- **物理编码（Physical Encoding）**  
  解耦时间与空间维度，注入物理先验。

  - **空间局部化编码（Localized Spatial Encoding）**  
    仿照 CFD 模板（stencil）离散方式，在输入空间坐标时不仅包含自身坐标 \(\vec{C}\)，还拼接其邻近点坐标（2D 取 4 邻域，3D 取 9 邻域），即 \(\Psi(\vec{C}) = [\vec{C}, \vec{C}_{\text{neighbors}}]\)。这显式编码了求解离散 Navier-Stokes 方程所需的局部空间相关性。

  - **高斯时间编码（Gaussian Temporal Encoding）**  
    通过两步处理一维时间坐标：
    1. 利用高斯径向基函数（RBF）核 \(K(t_i, t_j) = \exp(-|t_i - t_j|^2/(2\sigma^2))\) 将时间映射到高维特征空间，并赋予平移不变性，使 NTK 具有对角结构，提升泛化能力；
    2. 对核矩阵进行核主成分分析（Kernel PCA），提取前 \(m\) 个主成分得到低维时间特征 \(\Phi(t)\)。  
    这一过程增强了时间信息的高维特征和非线性动态捕捉能力。

- **Transformer 时空融合器（TransSTF）**  
  负责融合时间和空间特征，捕获长程时间依赖。
  - **多头注意力（MHA）**：采用自注意力机制增强时空特征交互。
  - **ResuMLP**：带有残差连接和正弦激活函数（SIREN）的 MLP 块，提升深层梯度传播和非线性表达能力。
  - **频域模块（Spectral Block）**：通过快速傅里叶变换（FFT）将特征转换到频域，用门控网络加权不同频率成分，再通过逆 FFT 回到物理空间，缓解频谱偏差，增强高频结构重建能力。

## 3. 实验设计

- **数据集与 Benchmark**  
  构建了公开的大规模数据集 **HFR‑Bench**（5.4 TB），涵盖 2D 和 3D 非定常流场，共计 33,600 个矢量场。具体包括：
  - 均匀笛卡尔网格：Riemann（RM）、Rayleigh‑Taylor 不稳定性（RT）、前向台阶（FFS）2D 案例，以及冲击‑纵向涡干扰（SV）3D 案例。
  - 非均匀结构网格：圆柱绕流（Cylinder）案例。
  每个案例配置 4 种网格分辨率和 4 种数值精度（WENO 格式，精度从 3 阶到 7 或 9 阶），最大网格分辨率差距达 64 倍，数值精度最高为 7 阶。低、高保真数据具有相同初始条件和物理参数，仅分辨率和精度不同。

- **对比方法**  
  - 传统双三次插值（BI）
  - NIF（Neural Implicit Flow, JMLR 2023）
  - CoordNet（TVCG 2023）
  - 消融版本：PEINR1（无谱块和无物理编码）和 PEINR2（仅无物理编码）

- **评价指标**  
  - PSNR（峰值信噪比）
  - SSIM（结构相似性指数）
  - CORR（相关系数）
  - DD（耗散差异，评估流场梯度捕捉能力）

- **训练与测试划分**  
  均匀网格案例：时间步 460~480 用于训练，后 20 步测试；非均匀网格：步长 5 采样训练，其余测试。测试结果分别展示特定步（如 step 500 或 494）。

## 4. 资源与算力

- **硬件配置**  
  全部实验在 **单个 NVIDIA A100 80GB GPU** 上完成。
- **训练设置**  
  - 损失函数：MSE
  - 训练轮次：2000 epoch（所有方法 1000 轮内均收敛）
  - 优化器：AdamW，学习率 \(1\!\times\!10^{-5}\)，20 轮不下降时衰减
  - 每个实验的批量大小、GPU 内存占用和单轮时间在论文 Table 1 中列出（如 3D SV 案例为 BS=36000，内存 75.31 GB，时间 68.45 s/epoch）

- **算力未明确部分**  
  未给出整体训练总时长，但提供了每个案例单轮时间和总轮数，可粗略估算总计算量。

## 5. 实验数量与充分性

- **实验规模**  
  - 5 组不同流场案例（RM、RT、FFS、SV、Cylinder），分别包含不同分辨率提升因子 \(\alpha\) 和数值精度提升因子 \(\beta\) 的组合（如表 2 共展示 9 种配置）。
  - 每组配置下对比 5 种方法（BI、NIF、CoordNet、PEINR1、PEINR2、PEINR），共计 **≥ 45 组测试配置**。
  - 定性展示：流线绘制、等值线图、3D 视角对比。
  - 消融实验：逐步剥离谱块和物理编码，验证各组件贡献。
  - 泛化性实验：评估在超出训练时间步上的表现。

- **充分性与公平性**  
  实验覆盖多种网格类型、维度、物理场景和分辨率提升因子，对比时使用原作者代码（仅修改输入长度），超参数在±10% 范围内微调至最优。多指标定量评估和详细定性结果保证了实验的充分性和公平性。

## 6. 主要结论与发现

- PEINR 在绝大多数定量指标（PSNR、SSIM、CORR、DD）上优于现有 INR 方法（NIF、CoordNet），尤其在物理一致性指标 DD 上优势显著。
- 物理编码能有效缓解时空复杂度不匹配，同时保留流场的物理奇性（如激波、涡结构）。
- 频域模块有效对抗频谱偏差，提升高频细节重建。
- 在超出训练时间步的泛化测试中，PEINR 表现出一致的优势，说明其具备更强的外推能力。
- 消融实验证实：仅加入物理编码或谱块均对重建质量有显著增益，两者组合效果最佳。

## 7. 优点

- **创新性**  
  - 首次发布面向高保真流场重建的大规模公开基准数据集 HFR‑Bench，填补领域空白。
  - 首次在 INR 框架中同时处理网格分辨率和数值精度增强，摒弃网格独立性假设。
  - 独特的时间 RBF 核编码 + Kernel PCA，从 NTK 角度设计时序特征，具有理论支撑。

- **方法设计**  
  - 物理编码融入 CFD 模板逻辑，显式利用局部邻域信息，契合偏微分方程求解本质。
  - 频谱块与 Transformer 结合，有效提升高频捕捉能力。
  - 误差场学习范式，将 INR 的重点放在修正低精度场的残差上，降低建模难度。

- **实验严谨性**  
  - 多指标、多场景、多方法全面对比，包含消融与泛化实验，证据充分。

## 8. 不足与局限

- **场景局限性**  
  论文聚焦于 5 种典型压缩/不可压缩流（Euler 方程、N‑S 方程），尚未在更广泛的流动类型（如多相流、化学反应流、高马赫数非稳态复杂边界）上验证。
- **效率未充分讨论**  
  虽然在单个 A100 上完成，但对比推理时间、参数量、对超大规模 3D 网格的可扩展性未作深入分析。
- **时域超参数敏感性**  
  RBF 核宽度 \(\sigma\) 需手动设定（实验中设为 10），不同流动特征可能影响最优取值，缺乏系统性分析。
- **网格类型限制**  
  虽支持非均匀结构网格，但未展示在完全非结构网格（如 DG 方法产生的三角形/四面体网格）上的表现，尚不能断言完全网格无关性。
- **误差分析与物理一致性**  
  尽管 DD 指标显示物理一致性提升，但并未深入讨论在极强间断（如 RM 问题）附近 PEINR 的 PSNR 略逊于 CoordNet 的根本物理原因，或可能的改进策略。

（完）
```
