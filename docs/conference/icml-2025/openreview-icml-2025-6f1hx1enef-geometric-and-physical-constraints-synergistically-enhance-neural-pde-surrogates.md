---
title: Geometric and Physical Constraints Synergistically Enhance Neural PDE Surrogates
title_zh: 几何与物理约束协同增强神经偏微分方程代理模型
authors: "Yunfei Huang, David S. Greenberg"
date: 2025-05-01
pdf: "https://openreview.net/pdf?id=6f1Hx1eneF"
tags: ["query:falling-film"]
score: 6.0
evidence: 基于交错网格的物理对称约束神经代理模型用于CFD，可迁移至降膜换热模拟
tldr: 该论文提出在交错网格上引入几何与物理约束的神经偏微分方程代理模型，系统研究了这些先验对于计算流体力学问题精度的影响。以浅水波方程为对象，验证了约束协同提升泛化性与长期预测能力。该方法可直接迁移至垂直降膜换热的CFD建模，为传热与多相流模拟提供物理一致的加速手段。
source: ICML-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1763, \"height\": 398, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1777, \"height\": 332, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 859, \"height\": 980, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1776, \"height\": 729, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 854, \"height\": 465, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 860, \"height\": 641, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1738, \"height\": 853, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1766, \"height\": 1420, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1777, \"height\": 1883, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1764, \"height\": 1017, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1595, \"height\": 1042, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1771, \"height\": 718, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1430, \"height\": 264, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 1708, \"height\": 2085, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 1780, \"height\": 367, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-016.webp\", \"caption\": \"\", \"page\": 0, \"index\": 16, \"width\": 1777, \"height\": 366, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-017.webp\", \"caption\": \"\", \"page\": 0, \"index\": 17, \"width\": 1754, \"height\": 2049, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-018.webp\", \"caption\": \"\", \"page\": 0, \"index\": 18, \"width\": 1754, \"height\": 2046, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-019.webp\", \"caption\": \"\", \"page\": 0, \"index\": 19, \"width\": 1760, \"height\": 1048, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-020.webp\", \"caption\": \"\", \"page\": 0, \"index\": 20, \"width\": 1776, \"height\": 773, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-021.webp\", \"caption\": \"\", \"page\": 0, \"index\": 21, \"width\": 1780, \"height\": 349, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-022.webp\", \"caption\": \"\", \"page\": 0, \"index\": 22, \"width\": 1760, \"height\": 1481, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-023.webp\", \"caption\": \"\", \"page\": 0, \"index\": 23, \"width\": 1760, \"height\": 1481, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-024.webp\", \"caption\": \"\", \"page\": 0, \"index\": 24, \"width\": 1776, \"height\": 297, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-025.webp\", \"caption\": \"\", \"page\": 0, \"index\": 25, \"width\": 1780, \"height\": 757, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-026.webp\", \"caption\": \"\", \"page\": 0, \"index\": 26, \"width\": 1777, \"height\": 327, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-027.webp\", \"caption\": \"\", \"page\": 0, \"index\": 27, \"width\": 1776, \"height\": 328, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-028.webp\", \"caption\": \"\", \"page\": 0, \"index\": 28, \"width\": 1785, \"height\": 1781, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-029.webp\", \"caption\": \"\", \"page\": 0, \"index\": 29, \"width\": 1777, \"height\": 1797, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-030.webp\", \"caption\": \"\", \"page\": 0, \"index\": 30, \"width\": 1775, \"height\": 1795, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-031.webp\", \"caption\": \"\", \"page\": 0, \"index\": 31, \"width\": 1752, \"height\": 1766, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-032.webp\", \"caption\": \"\", \"page\": 0, \"index\": 32, \"width\": 1753, \"height\": 1775, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-033.webp\", \"caption\": \"\", \"page\": 0, \"index\": 33, \"width\": 1779, \"height\": 768, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-6f1hx1enef/fig-034.webp\", \"caption\": \"\", \"page\": 0, \"index\": 34, \"width\": 1765, \"height\": 1721, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-icml-2025-6f1hx1enef/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 857, \"height\": 196, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-6f1hx1enef/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 856, \"height\": 235, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-6f1hx1enef/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1765, \"height\": 1016, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-6f1hx1enef/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1772, \"height\": 550, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-6f1hx1enef/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1708, \"height\": 290, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-6f1hx1enef/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 978, \"height\": 374, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-6f1hx1enef/table-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 951, \"height\": 501, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-6f1hx1enef/table-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1732, \"height\": 588, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-6f1hx1enef/table-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1554, \"height\": 292, \"label\": \"Table\"}]"
motivation: 神经PDE代理模型在CFD中泛化差且误差累积，现有物理约束不兼容交错网格。
method: 设计尊重物理定律和对称性的输入输出层，系统组合约束嵌入交错网格代理模型。
result: 在浅水波方程中，几何与物理约束协同提升精度和泛化能力。
conclusion: 物理感知的神经代理模型为复杂流体仿真提供了可靠且高效的计算方案。
---

## Abstract
Neural PDE surrogates can improve the cost-accuracy tradeoff of classical solvers, but often generalize poorly to new initial conditions and accumulate errors over time. Physical and symmetry constraints have shown promise in closing this performance gap, but existing techniques for imposing these inductive biases are incompatible with the staggered grids commonly used in computational fluid dynamics. Here we introduce novel input and output layers that respect physical laws and symmetries on the staggered grids, and for the first time systematically investigate how these constraints, individually and in combination, affect the accuracy of PDE surrogates. We focus on two challenging problems: shallow water equations with closed boundaries and decaying incompressible turbulence. Compared to strong baselines, symmetries and physical constraints consistently improve performance across tasks, architectures, autoregressive prediction steps, accuracy measures, and network sizes. Symmetries are more effective than physical constraints, but surrogates with both performed best, even compared to baselines with data augmentation or pushforward training, while themselves benefiting from the pushforward trick. Doubly-constrained surrogates also generalize better to initial conditions and durations beyond the range of the training data, and more accurately predict real-world ocean currents.

---

## 论文详细总结（自动生成）

### 1. 论文的核心问题与整体含义（研究动机和背景）
- **核心问题：** 神经网络偏微分方程（PDE）代理模型在长期自回归预测中普遍存在**泛化能力差**和**误差随时间累积**的问题。
- **研究动机：** 物理约束（守恒定律）和几何约束（对称等变性）虽能改善上述问题，但现有技术**不兼容**计算流体力学中广泛使用的**交错网格**（如Arakawa C-grid）。
- **整体含义：** 论文旨在系统性地研究物理与几何约束对PDE代理模型精度的影响，并首次将这两种约束协同嵌入交错网格架构中，以提升模型的长期稳定性和泛化能力。

### 2. 论文提出的方法论：核心思想、关键技术细节
- **核心思想：** 设计新颖的**输入层**和**输出层**，使神经网络能够直接在交错网格上保持物理守恒律和几何对称性，并探索其联合效用。
- **关键技术细节：**
    - **输入层（等变输入层）：** 针对交错网格上不同位置定义的变量（如网格中心的热力学量、界面上的速度分量），构建了一组特殊的滤波器。这些滤波器在空间变换（旋转、翻转）时，不仅进行重采样，还会进行通道置换和符号翻转，最终将输入数据映射为**群正则表示**，确保输入层的等变性。
    - **输出层（等变守恒输出层）：** 从内部隐藏层的正则表示中，通过线性组合和差分运算，在网格界面上重构速度场。通过在正则表示中引入类似差分的形式（如 `u_{i+0.5,j} = p_{i+1,j,1} - p_{i,j,3}`），在保持等变性的同时，输出符合交错网格排布的速度场。
    - **物理硬约束（守恒律）：**
        - **质量守恒：** 通过减去全局质量扰动均值实现，或在不可压缩流中学习势函数 \(a\)，并通过旋度运算（\(u = \nabla \times a\)）产生无散度速度场。
        - **动量守恒：** 通过减去各速度分量的全局均值实现。
    - **网络架构：** 以改进的“Modern U-Net”为基础架构，内部层使用等变卷积（如 `escnn` 库中的实现）替换标准卷积，并匹配参数量。

### 3. 实验设计：数据集、场景、对比方法
- **数据集与场景：**
    - **封闭边界浅水方程（SWE）：** 模拟波动，预测水面高度 \(\zeta\) 与速度场。训练数据包含50个仿真，网格为 \(100 \times 100\)，采用混合推理策略。
    - **衰减不可压缩湍流（INS）：** 模拟湍流衰减过程，预测速度场。训练数据包含100个随机初始条件，在 \(48 \times 48\) 网格上进行粗化处理。
    - **真实海洋洋流观测数据：** 测试模型对真实地球物理数据的预测能力。
- **对比的基准方法与环境：**
    - **几何对称性（Group）：** p1（仅平移）、p4（平移+旋转）、p4m（平移+旋转+翻转）。
    - **物理约束（Phys）：** 无约束（\( \emptyset \)）、质量守恒（M）、动量守恒（\( \rho\vec{u} \)）、质量+动量守恒（M+\( \rho\vec{u} \)）。
    - **基准架构：** 标准Modern U-Net、Dilated ResNet、Fourier Neural Operator (FNO)、Wang et al. 的等变旋转U-Net。
    - **训练技巧：** 标准训练、输入噪声注入、数据增强（Data Augmentation）和推演前移技巧（Pushforward Trick）。

### 4. 资源与算力
- **硬件：** 使用 2 块 Nvidia **A100 GPU**。
- **训练时长：**
    - **SWE：** 无等变网络训练需 0.5 小时，等变网络需 2 小时。
    - **INS：** 无等变网络训练需 0.4 小时，等变网络需 1.4 小时。
- **求解器与CPU推理：** 数据生成阶段应用了48核CPU节点（67秒/条件）以及显式求解器。在CPU和GPU上的推理速度对比显示，小级别等变网络推理在GPU上的开销受限于算子启动和数据传输，而非网络尺寸。

### 5. 实验数量与充分性
- **实验组数：** 进行了超百余组的系统性实验。
- **充分性与客观性：**
    - **消融实验充分：** 分别测试了2种对称约束等级、3种物理约束等级、多种组合、2种完全不同类型的PDE任务、3种输出时间跨度。
    - **架构与规模测试：** 在 U-Net 和 Dilated ResNet 上验证，并测试了数据量（100/400/760 ICs）和模型参数量（0.1M/2M/8.5M）的缩放效应。
    - **泛化性测试：** 测试了完全超出训练分布的全新初始条件（如L形隆起、改变波数峰值），以及真实海洋数据。
    - **对比公平性：** 维持了不同几何约束组之间的参数总量一致，考虑了数据增强、时间展开训练等先进技巧作为额外的强竞品。

### 6. 论文的主要结论与发现
- **约束有效性：** 几何对称约束与物理守恒约束均能持续提升PDE代理模型的精度与稳定性。
- **协同效应（Synergy）：** 几何约束的贡献大于物理约束，但**两者组合（“双重约束”）性能最佳**。例如，在SWE任务中，只有 `p4m/M` 模型在50小时长程预测中仍保持极高相关性；在INS任务中，只有 `p4m/M+ρu` 模型精确捕获了湍流动量守恒及能量频谱。
- **超越高级技巧：** 双重约束的模型性能超越了仅使用数据增强或推演前移技巧的无约束模型，且双重约束模型能进一步从“推演前移训练”中获益。
- **泛化能力：** 双重约束的代理模型在面对**新的初始条件**、**更长的预测时长**及**真实数据**时，表现出更强的物理一致性和更高的预测精度。

### 7. 优点：方法或实验设计上的亮点
- **系统性工程贡献：** 首次提出了适用于交错网格的等变卷积输入/输出层和守恒硬约束，填补了现有工具库（如escnn）不能处理交错网格的空白。
- **全面的量化分析：** 对几何与物理约束进行了极其彻底的剥离与组合分析，得出了“协同增强”的确定结论。
- **多维度客观评估：** 不仅依靠单点均方根误差，还综合应用了长程相关性、物理守恒量偏差、能量频谱分析和统计分布图，使得评估非常立体。
- **代码开源：** 提供了完整代码，保证了可复现性。

### 8. 不足与局限
- **应用范围限制：** 研究主要局限于规则的2维、方形网格及离散对称群（p4/p4m）。对于不规则网格、球形网格、连续性对称群及真实复杂几何体的推广仍需进一步验证。
- **硬约束的实施方式：** 物理硬约束采用了“全局平均值矫正”或“标量势函数求旋度”的方式。全局矫正可能会在某些非封闭边界或高度非齐次统计场景下不适用；基于势函数的无散策略可能损失一部分速度场的直接可解释性（如边界力）。
- **特定场景假设：** 模型在个别任务（如SWE）中使用了混合推理策略，需要结合部分传统数值求解步骤完成长程推演。

（完）
