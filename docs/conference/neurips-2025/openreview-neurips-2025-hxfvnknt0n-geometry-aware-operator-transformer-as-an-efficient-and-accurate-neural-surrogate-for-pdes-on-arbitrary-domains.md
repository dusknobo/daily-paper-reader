---
title: Geometry Aware Operator Transformer as an efficient and accurate neural surrogate for PDEs on arbitrary domains
title_zh: 几何感知算子Transformer：任意域上PDE的高效准确神经代理模型
authors: "Shizheng Wen, Arsh Kumbhat, Levi Lingsch, Sepehr Mousavi, Yizhou Zhao, Praveen Chandrashekar, Siddhartha Mishra"
date: 2025-09-18
pdf: "https://openreview.net/pdf?id=HXFvNkNt0n"
tags: ["query:falling-film"]
score: 4.0
evidence: 适用于任意域PDE求解的神经算子，可应用于多相流CFD模拟
tldr: 该文提出几何感知算子Transformer (GAOT)，用于在任意域上高效准确地学习偏微分方程的解算子。GAOT结合多尺度图神经算子和Transformer，解决了现有模型精度与效率难以兼顾的问题，在工程模拟中具有广泛应用前景，尤其可用于加速降膜蒸发等多物理场CFD仿真。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 696, \"height\": 678, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1428, \"height\": 768, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1440, \"height\": 407, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1337, \"height\": 411, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1381, \"height\": 283, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1402, \"height\": 364, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1396, \"height\": 299, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1178, \"height\": 367, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 722, \"height\": 724, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1392, \"height\": 381, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1439, \"height\": 1039, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1304, \"height\": 526, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1297, \"height\": 529, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 1389, \"height\": 763, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 841, \"height\": 837, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-016.webp\", \"caption\": \"\", \"page\": 0, \"index\": 16, \"width\": 1431, \"height\": 326, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-017.webp\", \"caption\": \"\", \"page\": 0, \"index\": 17, \"width\": 840, \"height\": 556, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-018.webp\", \"caption\": \"\", \"page\": 0, \"index\": 18, \"width\": 711, \"height\": 471, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-019.webp\", \"caption\": \"\", \"page\": 0, \"index\": 19, \"width\": 1403, \"height\": 582, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-020.webp\", \"caption\": \"\", \"page\": 0, \"index\": 20, \"width\": 1406, \"height\": 586, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-021.webp\", \"caption\": \"\", \"page\": 0, \"index\": 21, \"width\": 1406, \"height\": 583, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-022.webp\", \"caption\": \"\", \"page\": 0, \"index\": 22, \"width\": 1180, \"height\": 1256, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-023.webp\", \"caption\": \"\", \"page\": 0, \"index\": 23, \"width\": 1180, \"height\": 1255, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-024.webp\", \"caption\": \"\", \"page\": 0, \"index\": 24, \"width\": 1181, \"height\": 1255, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-025.webp\", \"caption\": \"\", \"page\": 0, \"index\": 25, \"width\": 1182, \"height\": 1242, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-026.webp\", \"caption\": \"\", \"page\": 0, \"index\": 26, \"width\": 1287, \"height\": 526, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-027.webp\", \"caption\": \"\", \"page\": 0, \"index\": 27, \"width\": 1280, \"height\": 1786, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-028.webp\", \"caption\": \"\", \"page\": 0, \"index\": 28, \"width\": 1284, \"height\": 506, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-029.webp\", \"caption\": \"\", \"page\": 0, \"index\": 29, \"width\": 1285, \"height\": 1790, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-030.webp\", \"caption\": \"\", \"page\": 0, \"index\": 30, \"width\": 1277, \"height\": 496, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-031.webp\", \"caption\": \"\", \"page\": 0, \"index\": 31, \"width\": 1280, \"height\": 1801, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-032.webp\", \"caption\": \"\", \"page\": 0, \"index\": 32, \"width\": 1409, \"height\": 1044, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-033.webp\", \"caption\": \"\", \"page\": 0, \"index\": 33, \"width\": 1410, \"height\": 1083, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-034.webp\", \"caption\": \"\", \"page\": 0, \"index\": 34, \"width\": 1398, \"height\": 1075, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-035.webp\", \"caption\": \"\", \"page\": 0, \"index\": 35, \"width\": 1407, \"height\": 1081, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-036.webp\", \"caption\": \"\", \"page\": 0, \"index\": 36, \"width\": 1405, \"height\": 2057, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-037.webp\", \"caption\": \"\", \"page\": 0, \"index\": 37, \"width\": 1404, \"height\": 2065, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-038.webp\", \"caption\": \"\", \"page\": 0, \"index\": 38, \"width\": 1389, \"height\": 1074, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-039.webp\", \"caption\": \"\", \"page\": 0, \"index\": 39, \"width\": 1405, \"height\": 597, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-040.webp\", \"caption\": \"\", \"page\": 0, \"index\": 40, \"width\": 1410, \"height\": 1046, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-041.webp\", \"caption\": \"\", \"page\": 0, \"index\": 41, \"width\": 1413, \"height\": 1087, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-042.webp\", \"caption\": \"\", \"page\": 0, \"index\": 42, \"width\": 1403, \"height\": 1088, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-043.webp\", \"caption\": \"\", \"page\": 0, \"index\": 43, \"width\": 1415, \"height\": 1082, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-044.webp\", \"caption\": \"\", \"page\": 0, \"index\": 44, \"width\": 1403, \"height\": 2054, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-045.webp\", \"caption\": \"\", \"page\": 0, \"index\": 45, \"width\": 1415, \"height\": 2079, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hxfvnknt0n/fig-046.webp\", \"caption\": \"\", \"page\": 0, \"index\": 46, \"width\": 1400, \"height\": 1073, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1383, \"height\": 824, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 597, \"height\": 211, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 698, \"height\": 283, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1444, \"height\": 220, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1404, \"height\": 806, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1455, \"height\": 1136, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1291, \"height\": 1025, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1292, \"height\": 766, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1290, \"height\": 716, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1416, \"height\": 1133, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 548, \"height\": 249, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1370, \"height\": 570, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1089, \"height\": 279, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 1439, \"height\": 212, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 1300, \"height\": 438, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-016.webp\", \"caption\": \"\", \"page\": 0, \"index\": 16, \"width\": 1331, \"height\": 582, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-017.webp\", \"caption\": \"\", \"page\": 0, \"index\": 17, \"width\": 870, \"height\": 151, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-018.webp\", \"caption\": \"\", \"page\": 0, \"index\": 18, \"width\": 1455, \"height\": 661, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-019.webp\", \"caption\": \"\", \"page\": 0, \"index\": 19, \"width\": 716, \"height\": 212, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-020.webp\", \"caption\": \"\", \"page\": 0, \"index\": 20, \"width\": 1363, \"height\": 242, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-021.webp\", \"caption\": \"\", \"page\": 0, \"index\": 21, \"width\": 746, \"height\": 232, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-022.webp\", \"caption\": \"\", \"page\": 0, \"index\": 22, \"width\": 1314, \"height\": 448, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-023.webp\", \"caption\": \"\", \"page\": 0, \"index\": 23, \"width\": 717, \"height\": 386, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-024.webp\", \"caption\": \"\", \"page\": 0, \"index\": 24, \"width\": 804, \"height\": 230, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-025.webp\", \"caption\": \"\", \"page\": 0, \"index\": 25, \"width\": 1448, \"height\": 323, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hxfvnknt0n/table-026.webp\", \"caption\": \"\", \"page\": 0, \"index\": 26, \"width\": 766, \"height\": 224, \"label\": \"Table\"}]"
motivation: 当前PDE算子学习模型在工程仿真中难以同时实现高精度与低计算成本。
method: 提出几何感知算子Transformer (GAOT)，融合多尺度注意力图神经算子编码器-解码器与Transformer处理器。
result: 在多个基准PDE问题上，GAOT实现了兼具高精度与高效率的代理建模。
conclusion: GAOT为任意域上的偏微分方程快速求解提供了新范式，有望显著加速工业仿真设计。
---

## Abstract
The very challenging task of learning solution operators of PDEs on arbitrary domains accurately and efficiently is of vital importance to engineering and industrial simulations. Despite the existence of many operator learning algorithms to approximate such PDEs, we find that accurate models are not necessarily computationally efficient and vice versa. We address this issue by proposing a geometry aware operator transformer (GAOT) for learning PDEs on arbitrary domains. GAOT combines novel multiscale attentional graph neural operator encoders and decoders, together with geometry embeddings and (vision) transformer processors to accurately map information about the domain and the inputs into a robust approximation of the PDE solution. Multiple innovations in the implementation of GAOT also ensure computational efficiency and scalability. We demonstrate this significant gain in both accuracy and efficiency of GAOT over several baselines on a large number of learning tasks from a diverse set of PDEs, including achieving state of the art performance on three large scale three-dimensional industrial CFD datasets. Our project page for accessing the source code is available at https://camlab-ethz.github.io/GAOT.

---

## 论文详细总结（自动生成）

好的，作为一名资深学术论文分析助手，我将以中文、Markdown 形式，对所提供的论文《Geometry Aware Operator Transformer As An Efficient And Accurate Neural Surrogate For PDEs On Arbitrary Domains》进行结构化、深入、客观的总结。

### **1. 研究动机与核心问题**

*   **核心问题**：在工程与工业仿真中，精确且高效地学习任意几何域上偏微分方程的解算子是一项关键但极具挑战性的任务。
*   **研究背景与动机**：
    *   **传统方法的局限**：有限元等经典数值方法对于不确定性量化、控制等“多查询”问题计算成本极高。
    *   **现有神经算子的不足**：作者通过系统对比发现，当前主流的神经算子模型普遍存在 **“精度-效率权衡”** 困境。例如，基于消息传递的模型如RIGNO虽然精度高、鲁棒性强，但计算效率低、扩展性差；而基于傅里叶算子的模型如GINO计算效率尚可，但精度不足。
    *   **根本目标**：设计一种能够在任意域上学习PDE解算子，同时具备 **高精度、高计算效率、强可扩展性** 三方面能力的新模型，以胜任真实世界的工业级仿真。

### **2. 方法论：几何感知算子Transformer (GAOT)**

GAOT 遵循经典的“编码-处理-解码”范式，其核心架构与关键技术细节如下：

*   **整体架构流程**：
    1.  **输入与编码**：将定义在任意点云上的PDE输入（如初始条件、边界条件、系数、几何形状）映射到**潜在规则网格**上的“几何感知令牌”。
    2.  **处理**：在潜在空间中使用视觉Transformer对令牌进行全局信息交互与特征提取。
    3.  **解码**：将处理后的令牌解码回原始的物理空间，可输出在**任意查询点**上的PDE解。
*   **关键技术细节**：
    *   **多尺度注意力图神经算子 (MAGNO) 编/解码器**：
        *   **多尺度聚合**：在编码和解码阶段，围绕潜在令牌或查询点，构建多个不同半径（尺度）的局部邻域。这取代了传统的单尺度GNO，能捕捉多尺度物理特征。
        *   **注意力权重**：在每个尺度内，通过注意力机制动态计算邻域点对中心点贡献的权重 αₘₖ，而非均匀或固定权重。
            `αₘₖ = softmax(⟨Wₘq y, Wₘκ xₖ⟩ / √d)`
        *   **跨尺度融合**：通过可学习的注意力权重 βₘ，对不同尺度的编码特征进行加权融合，得到最终令牌特征。
            `βₘ(y) = softmax(ψₘ(y))`
            `wₑ(y) = Σ βₘ(y) · ŵₘ(y)`
    *   **几何嵌入 (Geometry Embeddings)**：
        *   **动机**：仅有坐标信息不足以描述复杂几何域对解的影响。
        *   **方法**：为每个尺度的邻域计算**统计描述符**（如邻居点数、平均距离、方差、质心偏移、PCA特征等），将其作为额外的几何信息输入MLP，生成几何嵌入向量，并与MAGNO编码特征融合。这使模型能感知局部形状的各向异性和密度变化。
    *   **Transformer 处理器**：
        *   **选择**：由于编码器输出位于规则网格上，GAOT采用高效的**视觉Transformer (ViT)** 作为处理器，通过**补丁化 (Patching)** 技术合并相邻令牌，大幅降低自注意力的计算复杂度。
        *   **结构**：使用RMS标准化、旋转位置编码和跨层残差连接，以稳定训练和促进信息流动。
    *   **高效实现策略**：
        *   **图预计算**：预处理并缓存计算图中的边连接关系，避免运行时重复构建。
        *   **混合批处理**：编/解码器因图结构各异而逐样本处理，但ViT处理器对令牌进行批处理，兼顾内存效率与计算吞吐量。
        *   **双向图构建**：在3D大规模网格上，结合半径图和K近邻图，确保域覆盖率的同时控制边的数量，避免内存溢出。

### **3. 实验设计**

*   **数据集/场景**：实验覆盖了极为广泛的PDE问题，包括：
    *   **二维时间无关问题**：泊松方程（新版多尺度数据集）、超弹性力学、可压缩流（跨声速/超声速、多种翼型和钝体）。
    *   **二维时间相关问题**：不可压纳维-斯托克斯方程、可压缩欧拉方程、波动方程。以上数据包含规则网格、随机点云和非结构化自适应网格。
    *   **三维工业级CFD数据集**：汽车空气动力学（DrivAerNet++、DrivAerML）和飞机空气动力学（NASA-CRM），任务为预测表面压力场和壁面剪切应力等。
*   **基线模型 (Benchmarks)**：广泛对比了三大类代表性模型，包括：
    *   **基于图/消息传递**：RIGNO。
    *   **基于傅里叶层/算子**：GINO, GeoFNO, FNO DSE。
    *   **基于Transformer**：Transolver, UPT, GNOT。
*   **评估指标**：相对L1误差（精度）、训练吞吐量（效率）、推理延迟（效率），以及在不同输入/模型规模下的可扩展性。对于3D数据集，使用均方误差和平均绝对误差。

### **4. 资源与算力**

*   **主要算力配置**：对于二维数据集，使用**单个NVIDIA GeForce RTX 4090** GPU进行训练和评估。
*   **大规模3D数据集**：
    *   **DrivAerNet++**: 使用**4块 NVIDIA A100** GPU，数据并行，训练**50个epochs**，每块GPU批处理大小为1。
    *   **DrivAerML 和 NASA-CRM**: 使用**1块 NVIDIA A100** GPU训练**200个epochs**。
*   **对比基准**：论文明确指出所有模型（除特殊说明外）均在相同硬件上进行公平比较，并记录了详细的计算效率指标，确保了对比的公正性。

### **5. 实验数量与充分性**

*   **实验数量**：实验规模非常庞大和系统。
    *   **主要基准**：至少包含 **28个** 不同的PDE学习任务。
    *   **对比方法**：与 **超过8种** 主流模型进行了详细比较。
    *   **消融研究**：设计了大量消融实验来分析模型各组件的贡献，包括：MAGNO编码器、几何嵌入、Transformer处理器、多尺度特征、潜在网格选择、时间步进策略等。
    *   **扩展性分析**：系统研究了模型在模型尺寸、数据规模、测试分辨率泛化、迁移学习等方面的性能。
*   **充分性与公平性**：实验设计非常充分且客观。对比在统一的硬件平台、数据划分和训练轮次下进行，明确排除了因训练设置不同导致性能差异的可能性。消融实验详实，有力地支撑了模型设计的合理性。

### **6. 主要结论与发现**

*   **打破精度-效率权衡**：GAOT是首个在PDE代理建模中，同时实现**最高精度**和**最高计算效率**的模型。其雷达图中精度和效率指标均接近满分，显著优于GINO（高效率/低精度）和RIGNO（高精度/低效率）。
*   **SOTA性能**：在二维PDE基准上，GAOT在绝大多数数据集上取得了最佳或次佳的精度，平均精度比第二名提升近50%。在DrivAerNet++等3D工业仿真基准上，GAOT也达到了最优性能。
*   **鲁棒性**：GAOT在各种PDE类型、几何形状和网格类型上表现极其稳定，而其他基线模型在某些复杂任务上会出现性能崩溃。
*   **强大的可扩展性**：随着输入规模和模型参数量的增加，GAOT的吞吐量下降平缓，展现出优秀的模型和输入可扩展性。
*   **泛化能力**：GAOT具备“神经场”特性，可进行零样本超分辨率泛化、跨几何域的少样本迁移学习，且效果显著。

### **7. 优点与亮点**

*   **方法论创新**：**MAGNO**将多尺度局部聚合、注意力机制和几何统计嵌入巧妙地融为一体，这是模型高精度的核心。
*   **系统性工程优化**：**图预计算**和**混合批处理**策略是GAOT实现高效率和高扩展性的关键，为大规模稀疏图计算提供了优秀范本。
*   **实验设计极其严谨**：采用**多维雷达图**综合评估精度、效率、鲁棒性，全面揭示了模型间的权衡关系，对比清晰、说服力强。
*   **工业应用潜力巨大**：在3D工业CFD数据集上取得的SOTA成果和几个数量级的推理加速效果，直接证明了其取代传统数值求解器的巨大潜力。

### **8. 不足与局限**

*   **缺乏严格理论分析**：论文主要依靠大量实验证明模型的有效性，缺少对MAGNO的算子逼近能力、Transformer处理器的泛化误差等理论层面的分析。
*   **3D解码器过拟合风险**：论文在消融实验中指出，在解码器中加入几何嵌入会导致DrivAerML数据集的性能下降，作者推测这增加了过拟合风险，但这个现象的通用性有待进一步验证。
*   **下游任务验证缺失**：论文未评估GAOT在除前向模拟之外的典型下游任务（如不确定性量化、逆向设计、PDE约束优化）中的表现。
*   **超参数敏感性**：模型引入了多个新组件（多尺度半径、补丁大小等），其超参数设定对性能的敏感性虽然通过消融有所体现，但未系统探讨。

（完）
