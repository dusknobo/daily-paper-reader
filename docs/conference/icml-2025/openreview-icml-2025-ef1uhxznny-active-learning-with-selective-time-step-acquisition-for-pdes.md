---
title: Active Learning with Selective Time-Step Acquisition for PDEs
title_zh: 面向偏微分方程的选择性时间步主动学习
authors: "Yegon Kim, Hyunsu Kim, Gyeonghoon Ko, Juho Lee"
date: 2025-05-01
pdf: "https://openreview.net/pdf?id=ef1UHxznNy"
tags: ["query:falling-film"]
score: 6.0
evidence: 针对PDE代理模型的主动学习可降低降膜换热CFD模拟的成本
tldr: 针对PDE代理模型训练数据生成成本高昂的问题，论文提出一种选择性时间步主动学习框架，仅用数值求解器生成最关键时间步，其余由代理模型近似。实验表明该方法大大降低了数据获取成本，为垂直管降膜换热CFD模拟的加速提供了可行路径。
source: ICML-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-icml-2025-ef1uhxznny/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 849, \"height\": 416, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-ef1uhxznny/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 831, \"height\": 496, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-ef1uhxznny/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1777, \"height\": 518, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-ef1uhxznny/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1700, \"height\": 460, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-ef1uhxznny/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1760, \"height\": 342, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-ef1uhxznny/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 800, \"height\": 527, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-ef1uhxznny/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1609, \"height\": 454, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-ef1uhxznny/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 853, \"height\": 425, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-ef1uhxznny/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 882, \"height\": 427, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-ef1uhxznny/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1741, \"height\": 1314, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-ef1uhxznny/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1705, \"height\": 2291, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-ef1uhxznny/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1779, \"height\": 444, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-ef1uhxznny/fig-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1780, \"height\": 498, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-ef1uhxznny/fig-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 723, \"height\": 2006, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-ef1uhxznny/fig-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 542, \"height\": 477, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-icml-2025-ef1uhxznny/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 865, \"height\": 945, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-ef1uhxznny/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 864, \"height\": 224, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-ef1uhxznny/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 857, \"height\": 258, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-ef1uhxznny/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 808, \"height\": 300, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-ef1uhxznny/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 854, \"height\": 273, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-ef1uhxznny/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 853, \"height\": 352, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-ef1uhxznny/table-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 866, \"height\": 326, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-ef1uhxznny/table-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1339, \"height\": 174, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-ef1uhxznny/table-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1634, \"height\": 388, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-ef1uhxznny/table-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1582, \"height\": 390, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-ef1uhxznny/table-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1585, \"height\": 388, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-ef1uhxznny/table-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1611, \"height\": 388, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-ef1uhxznny/table-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1526, \"height\": 389, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-ef1uhxznny/table-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 1351, \"height\": 995, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-ef1uhxznny/table-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 1172, \"height\": 1144, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-ef1uhxznny/table-016.webp\", \"caption\": \"\", \"page\": 0, \"index\": 16, \"width\": 635, \"height\": 325, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-ef1uhxznny/table-017.webp\", \"caption\": \"\", \"page\": 0, \"index\": 17, \"width\": 679, \"height\": 324, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-ef1uhxznny/table-018.webp\", \"caption\": \"\", \"page\": 0, \"index\": 18, \"width\": 872, \"height\": 324, \"label\": \"Table\"}]"
motivation: 解决训练PDE代理模型时全轨迹数据获取成本高的问题。
method: 提出仅获取关键时间步的主动学习策略，其余用代理模型补全。
result: 在多个PDE基准上大幅减少所需数值模拟次数。
conclusion: 该主动学习框架可显著降低PDE代理建模成本，适用于降膜CFD等工程模拟。
---

## Abstract
Accurately solving partial differential equations (PDEs) is critical to understanding complex scientific and engineering phenomena, yet traditional numerical solvers are computationally expensive. Surrogate models offer a more efficient alternative, but their development is hindered by the cost of generating sufficient training data from numerical solvers. In this paper, we present a novel framework for active learning (AL) in PDE surrogate modeling that reduces this cost. Unlike the existing AL methods for PDEs that always acquire entire PDE trajectories, our approach strategically generates only the most important time steps with the numerical solver, while employing the surrogate model to approximate the remaining steps. This dramatically reduces the cost incurred by each trajectory and thus allows the active learning algorithm to try out a more diverse set of trajectories given the same budget. To accommodate this novel framework, we develop an acquisition function that estimates the utility of a set of time steps by approximating its resulting variance reduction. We demonstrate the effectiveness of our method on several benchmark PDEs, including the Burgers' equation, Korteweg–De Vries equation, Kuramoto–Sivashinsky equation, the incompressible Navier-Stokes equation, and the compressible Navier-Stokes equation.
Experiments show that our approach improves performance by large margins over the best existing method. Our method not only reduces average error but also the 99\%, 95\%, and 50\% quantiles of error, which is rare for an AL algorithm. All in all, our approach offers a data-efficient solution to surrogate modeling for PDEs.

---

## 论文详细总结（自动生成）

好的，作为一名资深学术论文分析助手，我将以中文、Markdown形式，对该论文进行结构化、深入、客观的总结。

### 1. 论文的核心问题与整体含义

*   **核心问题**: 在为偏微分方程构建高效的代理模型时，主要的瓶颈在于使用传统数值求解器生成训练数据的过程成本极高。现有的主动学习方法虽然旨在减少所需数据量，但每次都获取完整的PDE轨迹，这并非最优策略，因为轨迹内部的时间步往往高度相关，信息冗余。
*   **整体含义**: 该论文提出了一种新的数据获取框架，它打破了“必须获取完整轨迹”的限制，允许在单个轨迹内部进行选择性采样。通过仅用昂贵的数值求解器计算最关键的时间步，并用廉价的代理模型近似其余部分，可以在给定的计算预算下探索更多样化的初始条件，从而以更低的成本训练出更高精度的代理模型。

### 2. 论文提出的方法论

*   **核心思想**: 论文提出了一个名为**STAP** 的框架。其核心思想是，对于给定初始条件的一条轨迹，不生成全部时间步，而是选择一个**采样模式**，只对标记为 `true` 的时间步使用昂贵的数值求解器 `G`，而对标记为 `false` 的时间步，则使用当前廉价的代理模型 `\hat{G}` 进行预测。这大大降低了一条轨迹的获取成本。
*   **关键技术细节**:
    *   **轨迹生成**: 采用迭代方式生成轨迹 `\hat{u}_i`。如果采样模式为 `true`，则 `\hat{u}_i = G[\hat{u}_{i-1}]`；如果为 `false`，则 `\hat{u}_i = \hat{G}[\hat{u}_{i-1}]`。只有使用求解器的配对 `(\hat{u}_{i-1}, \hat{u}_i)` 会被加入训练数据集。
    *   **采集函数**: 设计了一个新的采集函数 `a(u_0, S)`，用于评估特定初始条件 `u_0` 和采样模式 `S` 的效用。该函数基于委员会成员间的**方差减少**来估计信息量。具体地，它计算委员会中任意两个模型 `(\hat{G}^a, \hat{G}^b)` 的预测轨迹差异，以及在假设从`\hat{G}^a`处为`\hat{G}^b`获取了`S`所指定的时间步数据后，`\hat{G}^b`预测轨迹的差异变化。该函数是“按委员会查询”方法在选择性时间步采样下的推广。
    *   **批采集算法**: 为了解决计算复杂度和数据多样性的问题，STAP被设计为一个附加模块，与现有的全轨迹主动学习方法配合使用。每轮采集时，先由基础方法选择一个初始条件 `u_0`，然后通过一个贪心搜索算法，最大化代价加权采集函数 `a^*(u_0, S) = a(u_0, S) / \|S\|`，为选定的 `u_0` 优化出最佳的采样模式 `S`。重复此过程直到达到一轮的预算上限。

### 3. 实验设计

*   **数据集/场景**: 在五个具有代表性的PDE基准上进行验证，涵盖从一维到二维、从平滑到混沌和湍流等多种复杂行为：
    *   Burgers'方程（冲击波现象）
    *   Korteweg–De Vries方程（孤立波）
    *   Kuramoto–Sivashinsky方程（混沌动力学）
    *   不可压缩Navier-Stokes方程（湍流）
    *   可压缩Navier-Stokes方程（强非线性、湍流）
*   **Benchmark方法**: 对比了多种全轨迹采样的主动学习方法：
    *   **Random**: 随机选择初始条件。
    *   **QbC**: 按委员会查询，基于模型预测的方差来选择初始条件。
    *   **LCMD**: 一种基于特征空间距离的批量主动学习方法。
    *   **SBAL**: 随机批量主动学习，以特定概率分布随机采样数据点。
*   **代理模型**: 所有方法均采用**傅里叶神经算子** 作为代理模型 `\hat{G}`，并训练其预测相邻时间步的状态差。委员会规模设为2。

### 4. 资源与算力

*   **计算资源**: 所有实验均在 **8 块 NVIDIA GeForce RTX 2080 Ti GPU** 上运行。
*   **其他耗时**: 论文详细分析了STAP自身的计算开销（主要集中在批采集阶段的优化搜索上），并提供了与基线方法的壁钟时间对比，以及加速变体 `+STAP_{10}` 的性能和耗时对比。

### 5. 实验数量与充分性

*   **实验数量**: 实验设计充分且多样，主要包括：
    1.  **主实验**: 在5个PDE上对比4种基线方法及其与STAP的结合版本，每项实验用5个随机种子取平均，进行10轮采集。
    2.  **消融实验**:
        *   对比了随机Bernoulli采样模式，以证明STAP自适应选择时间步位置的优势。
        *   测试了在仅用1条轨迹作为初始数据（极端数据匮乏）下STAP的鲁棒性。
        *   探索了与多步FNO模型的兼容性。
    3.  **分析与可视化**: 对模型隐藏层激活进行PCA分析，直观展示了局部轨迹采样与多样化随机采样的数据分布差异，解释了STAP有效的原因。
*   **充分性与公平性**: 实验对比全面，涵盖了主流基线，并在多个性质的PDE上验证，结论具有普遍性。消融实验有效支撑了核心论点。比较是在相同预算（每轮获取相同数量的求解器查询次数）下进行的，保证了公平性。

### 6. 论文的主要结论与发现

*   **性能显著提升**: 在所有测试PDE上，**SBAL+STAP** 的组合均大幅优于所有基线方法（包括SBAL本身），不仅降低了平均RMSE，还罕见地同时降低了99%、95%和50%分位数的误差。
*   **采样策略的有效性**: 单纯随机稀疏采样时间步（Bernoulli采样）本身可能优于全轨迹采样，而STAP通过自适应地选择采样的频率和具体位置，超越了任何固定概率的随机稀疏采样。
*   **鲁棒性**: STAP即使在初始代理模型非常不准确（例如仅用1条轨迹训练）的情况下，多数场景下依然能保持对基线的优势，显示出对模型误差的一定鲁棒性。

### 7. 优点

*   **新颖的框架**: 首次在PDE轨迹预测的主动学习中引入“局部轨迹采样”的框架，是对领域内“全轨迹采样”范式的一次重要突破。
*   **严格的理论泛化**: 将经典的QbC采集函数自然地推广到了可以评估时间步子集的场景，理论基础扎实。
*   **即插即用**: STAP被设计为一个可与现有全轨迹主动学习方法轻松集成的附加模块，实用性强。
*   **全面的性能提升**: 不仅提升平均性能，还能提升各个误差分位数的性能，表明该方法在不同复杂度的轨迹上均有效。

### 8. 不足与局限

*   **计算开销**: STAP的批采集算法引入了额外的计算开销，尤其是在优化采样模式时。虽然论文提出了近似和加速变体，但相对于简单的基线方法仍有额外的时间成本。
*   **对特定动力学不稳定性的处理**: 在KdV方程实验中，模型合成的输入偶尔会导致数值求解器崩溃。论文通过简单地跳过这些时间步来处理，这种方法略显被动，可能浪费一部分预算。
*   **超参数敏感性**: 贪心搜索算法的迭代次数 `T` 和变异概率 `ϵ` 可能需要根据具体任务进行调整，论文对此的讨论较少。
*   **代理模型依赖性**: 轨迹生成依赖于代理模型的预测来填充“未采样”的时间步，如果初始代理模型质量极差，可能会严重影响轨迹的质量，尽管实验证明其具有一定鲁棒性，但在极端情况下仍是潜在风险点。

（完）
