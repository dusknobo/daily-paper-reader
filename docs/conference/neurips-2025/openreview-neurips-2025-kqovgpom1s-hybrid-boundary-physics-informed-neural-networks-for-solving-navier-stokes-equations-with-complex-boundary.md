---
title: Hybrid Boundary Physics-Informed Neural Networks for Solving Navier-Stokes Equations with Complex Boundary
title_zh: 混合边界物理信息神经网络用于求解复杂边界条件下的纳维-斯托克斯方程
authors: "Chuyu Zhou, Tianyu Li, Chenxi Lan, Rongyu Du, Guoguo Xin, Wei Li, Guoqing Wang, Xun Liu, Hangzhou Yang"
date: 2025-09-18
pdf: "https://openreview.net/pdf?id=KQoVgPOM1S"
tags: ["query:falling-film"]
score: 5.0
evidence: 求解复杂边界纳维-斯托克斯方程，可用于多相流CFD
tldr: 针对复杂边界条件下纳维-斯托克斯方程求解这一难题，本文提出混合边界物理信息神经网络(HB-PINN)，结合预训练网络进行高效初始化和边界约束机制，通过主网络处理内部点、距离度量网络增强边界预测，从而准确求解边界和内部区域。实验表明，该方法在复杂边界条件下的NS方程求解上表现优越，为多相流CFD模拟提供了新的数值方法。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1166, \"height\": 775, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1069, \"height\": 266, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1048, \"height\": 284, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1155, \"height\": 257, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1065, \"height\": 279, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1145, \"height\": 481, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1093, \"height\": 541, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1099, \"height\": 539, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1093, \"height\": 539, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1097, \"height\": 538, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1158, \"height\": 239, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 589, \"height\": 465, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1083, \"height\": 686, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 837, \"height\": 668, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 703, \"height\": 559, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-016.webp\", \"caption\": \"\", \"page\": 0, \"index\": 16, \"width\": 1063, \"height\": 344, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-017.webp\", \"caption\": \"\", \"page\": 0, \"index\": 17, \"width\": 1160, \"height\": 251, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-018.webp\", \"caption\": \"\", \"page\": 0, \"index\": 18, \"width\": 1175, \"height\": 585, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-019.webp\", \"caption\": \"\", \"page\": 0, \"index\": 19, \"width\": 1106, \"height\": 367, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-020.webp\", \"caption\": \"\", \"page\": 0, \"index\": 20, \"width\": 1098, \"height\": 545, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-021.webp\", \"caption\": \"\", \"page\": 0, \"index\": 21, \"width\": 1097, \"height\": 551, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-022.webp\", \"caption\": \"\", \"page\": 0, \"index\": 22, \"width\": 1098, \"height\": 546, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-023.webp\", \"caption\": \"\", \"page\": 0, \"index\": 23, \"width\": 1096, \"height\": 544, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-024.webp\", \"caption\": \"\", \"page\": 0, \"index\": 24, \"width\": 1102, \"height\": 549, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-025.webp\", \"caption\": \"\", \"page\": 0, \"index\": 25, \"width\": 1102, \"height\": 544, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-026.webp\", \"caption\": \"\", \"page\": 0, \"index\": 26, \"width\": 1097, \"height\": 539, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-027.webp\", \"caption\": \"\", \"page\": 0, \"index\": 27, \"width\": 1100, \"height\": 545, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-028.webp\", \"caption\": \"\", \"page\": 0, \"index\": 28, \"width\": 1165, \"height\": 248, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-029.webp\", \"caption\": \"\", \"page\": 0, \"index\": 29, \"width\": 1159, \"height\": 245, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-030.webp\", \"caption\": \"\", \"page\": 0, \"index\": 30, \"width\": 1096, \"height\": 541, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-031.webp\", \"caption\": \"\", \"page\": 0, \"index\": 31, \"width\": 1099, \"height\": 543, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-032.webp\", \"caption\": \"\", \"page\": 0, \"index\": 32, \"width\": 1097, \"height\": 544, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-033.webp\", \"caption\": \"\", \"page\": 0, \"index\": 33, \"width\": 1095, \"height\": 538, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-034.webp\", \"caption\": \"\", \"page\": 0, \"index\": 34, \"width\": 1095, \"height\": 542, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-035.webp\", \"caption\": \"\", \"page\": 0, \"index\": 35, \"width\": 1097, \"height\": 540, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-036.webp\", \"caption\": \"\", \"page\": 0, \"index\": 36, \"width\": 1134, \"height\": 676, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-037.webp\", \"caption\": \"\", \"page\": 0, \"index\": 37, \"width\": 1167, \"height\": 482, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-038.webp\", \"caption\": \"\", \"page\": 0, \"index\": 38, \"width\": 1090, \"height\": 760, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-039.webp\", \"caption\": \"\", \"page\": 0, \"index\": 39, \"width\": 542, \"height\": 556, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-040.webp\", \"caption\": \"\", \"page\": 0, \"index\": 40, \"width\": 1012, \"height\": 579, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-041.webp\", \"caption\": \"\", \"page\": 0, \"index\": 41, \"width\": 1026, \"height\": 514, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-042.webp\", \"caption\": \"\", \"page\": 0, \"index\": 42, \"width\": 1110, \"height\": 340, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-kqovgpom1s/fig-043.webp\", \"caption\": \"\", \"page\": 0, \"index\": 43, \"width\": 1078, \"height\": 487, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-neurips-2025-kqovgpom1s/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 872, \"height\": 830, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-kqovgpom1s/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1102, \"height\": 626, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-kqovgpom1s/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 897, \"height\": 253, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-kqovgpom1s/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 960, \"height\": 1599, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-kqovgpom1s/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 945, \"height\": 1022, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-kqovgpom1s/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1001, \"height\": 422, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-kqovgpom1s/table-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1136, \"height\": 429, \"label\": \"Table\"}]"
motivation: 求解复杂边界条件下的纳维-斯托克斯方程是计算流体力学中的关键难题。
method: 提出混合边界物理信息神经网络(HB-PINN)，结合预训练网络和距离度量网络以强化边界条件满足。
result: 在若干复杂边界条件的NS方程上验证了方法，边界和内部预测精度均得到提升。
conclusion: HB-PINN为复杂边界流场计算提供了有效工具，可进一步推广至多相流模拟。
---

## Abstract
Physics-informed neural networks (PINN) have achieved notable success in solving partial differential equations (PDE), yet solving the Navier-Stokes equations (NSE) with complex boundary conditions remains a challenging task. In this paper, we introduce a novel Hybrid Boundary PINN (HB-PINN) method that combines a pretrained network for efficient initialization with a boundary-constrained mechanism. The HB-PINN method features a primary network focused on inner domain points and a distance metric network that enhances predictions at the boundaries, ensuring accurate solutions for both boundary and interior regions. Comprehensive experiments have been conducted on the NSE under complex boundary conditions, including the 2D cylinder wake flow and the 2D blocked cavity flow with a segmented inlet. The proposed method achieves state-of-the-art (SOTA) performance on these benchmark scenarios, demonstrating significantly improved accuracy over existing PINN-based approaches.

---

## 论文详细总结（自动生成）

### 论文核心问题与整体含义
*   **核心问题**：针对在**复杂边界条件下**使用物理信息神经网络（PINN）求解非线性纳维-斯托克斯方程（NSE）时，因边界条件损失与偏微分方程（PDE）残差损失难以同时最小化而导致求解精度下降的难题。
*   **整体含义**：提出一种名为**混合边界物理信息神经网络（HB-PINN）** 的新方法，旨在解耦并更有效地处理复杂几何和边界条件，为复杂流场的计算流体力学（CFD）模拟提供了一种高精度的替代数值方案。

### 论文提出的方法论
*   **核心思想**：将传统PINN的单网络任务分解为三个子网络，通过“预训练+合成”的策略，将边界条件的严格约束与内部PDE的求解解耦。
*   **关键技术细节**：
    *   **三网络架构**：
        1.  **特解网络（NP）**：优先满足边界条件的弱约束预训练网络，其损失函数中边界权重远大于PDE权重（如 λ_BC=1000, λ_PDE=1），提供初始的边界合规解。
        2.  **距离度量网络（ND）**：学习域内点到边界的带符号距离函数，并应用幂函数 `f(^D_q) = 1 - (1 - ^D_q/max(^D_q))^α` 将距离映射至`[0,1]`区间，在边界处值为0，内部快速增至1，起空间调制权重作用。
        3.  **主网络（NH）**：规模最大的求解网络，接收经 `NP + ND * NH` 方式合成后的变量预测，其损失函数仅包含PDE残差，专注于提升内部域的计算精度。
    *   **训练流程**：采用两阶段训练，第一阶段分别预训练NP和ND网络；第二阶段固定NP和ND参数，仅优化主网络NH。

### 实验设计
*   **数据集/场景**：
    1.  **稳态圆柱绕流（Case 1）**：基准流体力学问题，域为5x1，圆柱直径0.2。
    2.  **稳态分段入口含障碍物方形腔流（Case 2）**：域为1x1方腔，含上下矩形障碍物及三段式入口。
    3.  **瞬态分段入口含障碍物方形腔流（Case 3）**：在Case 2基础上增加时间维度，模拟流场发展过程。
    *   *补充实验*：在更高雷诺数（Re=500, 1000, 2000）、更复杂几何（含多个交错障碍物的矩形腔流）、热传导方程及顶盖驱动流（LDC）等模型上进行了验证。
*   **基准与对比方法**：
    *   以有限元法（FEM）高分辨率计算结果作为**真值（GT）**。
    *   对比了**6种主流PINN变体**：传统软约束PINN (sPINN)，硬约束PINN (hPINN)，改进傅里叶网络PINN (MFN-PINN)，扩展PINN (XPINN)，自适应PINN (SA-PINN) 和PirateNet。

### 资源与算力
*   论文**未明确说明**所用GPU的具体型号及数量，仅提及利用PyTorch框架和“高性能GPU”进行训练。
*   **训练时间**：给出了每千轮训练时间，例如主案例中sPINN为31.1s，HB-PINN为47.8s；而一次CFD的推理时间为17s。HB‑PINN的推理时间仅为0.29s。

### 实验数量与充分性
*   **实验数量**：实验较为**充分**。
    *   **主体实验**：在3个不同复杂度的典型案例（稳态到瞬态）上进行了验证。
    *   **消融实验**：系统性地进行了3项消融研究，验证了**特解网络（NP）与距离度量网络（ND）联合使用的必要性**、**NP预训练轮次**及**ND网络中幂指数 α**对精度的影响。
    *   **鲁棒性与泛化性实验**：在不同**雷诺数（Re）**（500, 1000, 2000）、不同**物理模型**（热传导、LDC流）及更复杂的边界几何条件下进行了测试。
*   **客观与公平性**：所有对比方法均在统一的算例和基于FEM的真实值上进行量化比较，评价指标包括均方误差（MSE）、平均绝对误差（MAE）和相对L2误差，具有客观性和公平性。

### 论文的主要结论与发现
*   **精度显著提升**：在所有测试的复杂边界流动算例（稳态和瞬态）中，HB-PINN的预测精度均显著超越所有对比的基准方法，通常实现误差数量级的降低，建立了新的SOTA。
*   **架构有效性**：通过独立构造特解网络和距离度量网络来解耦边界与PDE约束，能有效解决传统PINN中的损失冲突问题，既能严格满足边界条件，又可保证内部求解精度。
*   **方法泛化性**：该框架不仅适用于不可压缩N-S方程，还可成功应用于热传导等其他物理方程，且在不同雷诺数和更复杂的几何构型下均保持鲁棒。

### 优点
*   **创新的解耦框架**：提出的“特解网络 + 距离函数网络 + 主网络”的三网络结构，巧妙地将复杂的边界处理与PDE求解分离，设计巧妙且有效。
*   **全面的实验验证**：实验设计详实，涵盖了稳态/瞬态、不同几何复杂度、不同物理模型以及详尽的消融和参数敏感性分析，论证充分。
*   **针对性强且效果显著**：直击PINN在处理复杂边界时的普遍痛点，并在标志性难题上取得了超越众多变体的大幅精度提升。

### 不足与局限
*   **关键超参数经验依赖**：距离度量网路的幂指数 α 和特解网络的预训练轮次等关键参数目前依赖经验调优，缺乏系统性的自动化确定方法。
*   **计算开销增加**：三网络架构和两阶段训练模式相比标准PINN增加了模型的复杂度和训练时间，且代码未开源。
*   **高雷诺数下性能下降**：尽管在Re=1000, Re=2000时有改善，但文中数据显示，预测误差随雷诺数增加呈上升趋势，其在高雷诺数强湍流下的绝对精度仍有提升空间。

（完）
