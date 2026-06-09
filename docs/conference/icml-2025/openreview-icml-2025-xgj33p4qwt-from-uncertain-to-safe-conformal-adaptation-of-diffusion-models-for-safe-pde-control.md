---
title: "From Uncertain to Safe: Conformal Adaptation of Diffusion Models for Safe PDE Control"
title_zh: "从不确定到安全: 面向安全PDE控制的扩散模型共形适应"
authors: "Peiyan Hu, Xiaowei Qian, Wenhao Deng, Rui Wang, Haodong Feng, Ruiqi Feng, Tao Zhang, Long Wei, Yue Wang, Zhi-Ming Ma, Tailin Wu"
date: 2025-05-01
pdf: "https://openreview.net/pdf?id=XGJ33p4qwt"
tags: ["query:falling-film"]
score: 4.0
evidence: 用于安全PDE控制的扩散模型可潜在地应用于降膜系统
tldr: 针对现有PDE控制方法忽略安全约束的问题，论文提出SafeDiffCon，在扩散模型中引入不确定性分位数以生成满足安全约束的控制序列。实验验证了其在多种PDE控制任务中的安全性和性能，为降膜换热过程的鲁棒控制提供了理论参考。
source: ICML-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-icml-2025-xgj33p4qwt/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1153, \"height\": 505, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-xgj33p4qwt/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 856, \"height\": 471, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-xgj33p4qwt/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1314, \"height\": 282, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-xgj33p4qwt/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 955, \"height\": 1550, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-xgj33p4qwt/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1633, \"height\": 1704, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-icml-2025-xgj33p4qwt/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 838, \"height\": 467, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xgj33p4qwt/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 647, \"height\": 337, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xgj33p4qwt/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 687, \"height\": 424, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xgj33p4qwt/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 703, \"height\": 278, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xgj33p4qwt/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1496, \"height\": 151, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xgj33p4qwt/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 740, \"height\": 278, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xgj33p4qwt/table-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 895, \"height\": 279, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xgj33p4qwt/table-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 670, \"height\": 277, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xgj33p4qwt/table-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 576, \"height\": 232, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xgj33p4qwt/table-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 499, \"height\": 233, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xgj33p4qwt/table-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1766, \"height\": 360, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xgj33p4qwt/table-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 950, \"height\": 195, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xgj33p4qwt/table-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 642, \"height\": 461, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xgj33p4qwt/table-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 712, \"height\": 720, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xgj33p4qwt/table-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 1232, \"height\": 848, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xgj33p4qwt/table-016.webp\", \"caption\": \"\", \"page\": 0, \"index\": 16, \"width\": 1122, \"height\": 848, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xgj33p4qwt/table-017.webp\", \"caption\": \"\", \"page\": 0, \"index\": 17, \"width\": 914, \"height\": 419, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xgj33p4qwt/table-018.webp\", \"caption\": \"\", \"page\": 0, \"index\": 18, \"width\": 915, \"height\": 419, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xgj33p4qwt/table-019.webp\", \"caption\": \"\", \"page\": 0, \"index\": 19, \"width\": 704, \"height\": 631, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xgj33p4qwt/table-020.webp\", \"caption\": \"\", \"page\": 0, \"index\": 20, \"width\": 748, \"height\": 630, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-xgj33p4qwt/table-021.webp\", \"caption\": \"\", \"page\": 0, \"index\": 21, \"width\": 556, \"height\": 416, \"label\": \"Table\"}]"
motivation: 解决PDE控制中深度学习方法缺乏安全保障的问题。
method: 通过重新加权扩散损失和不确定性分位数后训练，实现安全控制序列生成。
result: 在一系列PDE基准上取得满足安全约束的优化控制。
conclusion: 为安全关键型PDE控制提供了新范式，可能拓展至降膜蒸发器等工业应用。
---

## Abstract
The application of deep learning for partial differential equation (PDE)-constrained control is gaining increasing attention. However, existing methods rarely consider safety requirements crucial in real-world applications. To address this limitation, we propose Safe Diffusion Models for PDE Control (SafeDiffCon), which introduce the uncertainty quantile as model uncertainty quantification to achieve optimal control under safety constraints through both post-training and inference phases. Firstly, our approach post-trains a pre-trained diffusion model to generate control sequences that better satisfy safety constraints while achieving improved control objectives via a reweighted diffusion loss, which incorporates the uncertainty quantile estimated using conformal prediction. Secondly, during inference, the diffusion model dynamically adjusts both its generation process and parameters through iterative guidance and fine-tuning, conditioned on control targets while simultaneously integrating the estimated uncertainty quantile. We evaluate SafeDiffCon on three control tasks: 1D Burgers' equation, 2D incompressible fluid, and controlled nuclear fusion problem. Results demonstrate that SafeDiffCon is the only method that satisfies all safety constraints, whereas other classical and deep learning baselines fail. Furthermore, while adhering to safety constraints, SafeDiffCon achieves the best control performance. The code can be found at https://github.com/AI4Science-WestlakeU/safediffcon.

---

## 论文详细总结（自动生成）

## 一、研究动机与核心问题

在偏微分方程（PDE）控制的深度学习应用中，现有方法普遍忽略了**安全约束**要求，而这对流体控制、核聚变等高风险场景至关重要。传统扩散模型控制的预测安全得分与真实安全得分之间存在显著**分布偏移**，导致模型在追求控制性能时容易越过安全界限。

* 论文整体目标：**在离线、数据驱动条件下，使扩散模型能够在满足安全约束的前提下生成接近最优的控制序列**。
* 核心含义：通过**共形预测**量化安全不确定性，将“不确定”的安全预测转化为“安全”的控制行为。

## 二、方法论

SafeDiffCon 的核心是在扩散模型的**后训练与推理阶段**植入**不确定性分位数**（uncertainty quantile），以引导模型输出避开潜在风险区域。

### 2.1 不确定性量化：基于共形预测的不确定性分位数
* **校准集与分数集**：将一部分数据作为校准集 \(D_{cal}\)，计算模型预测的安全得分 \(s(u_\theta(w))\) 与实际安全得分 \(s(u)\) 的绝对差值集合 \(S\)。
* **分布偏移下的加权分数集**：考虑到推理时模型生成数据的分布 \(\tilde p\) 与校准集分布 \(p\) 不同，引入权重 \(\omega(u_i,w_i)=\tilde p(u_i,w_i)/p(u_i,w_i)\)，得到**移位分数集** \(\tilde S\)。实际中利用后训练过程中的 \(e^{-W}\) 近似计算权重。
* **不确定性分位数**：从 \(\tilde S\) 中取 \((1-\alpha)(1+1/|D_{cal}|)\) 分位数 \(Q(1-\alpha;\tilde S)\)。
* **共形区间**：\(CI_\theta = [s(u_\theta(w)) - Q,\; s(u_\theta(w)) + Q]\)，理论保证真实安全得分落在该区间内的概率 ≥ \(1-\alpha\)。

### 2.2 后训练：重加权损失
为将模型分布从 \(p\) 推向 \(p^* \propto p\,e^{-W}\)，定义：
\[
W(u,w) = \max[\,s(u)+Q(1-\alpha;\tilde S)-s_0,\,0\,] + \gamma J(u,w)
\]
后训练损失为：
\[
L_{\text{post‑train}} = \mathbb{E}_{k,(u,w),\epsilon}\left[ e^{-W(u,w)} \| \epsilon - \epsilon_\theta(\sqrt{\bar\alpha_k}[u,w]+\sqrt{1-\bar\alpha_k}\epsilon, k) \|_2^2 \right]
\]
利用 \(e^{-W}\) 对样本重加权，使模型偏好更安全且目标更优的区域。

### 2.3 推理时微调
* **引导 \(G\)**：与 \(W\) 同形，在扩散去噪过程中以梯度引导采样（式4），融入不确定性分位数。
* **微调损失**：基于当前采样结果 \(D_{\text{sampled}}\)，微调模型参数 \(\theta\)：
\[
L_{\text{fine‑tune}} = \sum_{(u_\theta,w_\theta)\in D_{\text{sampled}}} W(u_\theta,w_\theta)
\]
仅保留最后一个去噪步的计算图以节省显存。迭代式引导采样与参数微调，使最终控制序列更精确满足安全约束与控制目标。

## 三、实验设计

### 3.1 任务与数据集
* **1D Burgers 方程**
  * 目标：最终状态 \(u_T\) 逼近目标状态 \(u_d\)，\(J = \int |u_T - u_d|^2 dx\)
  * 安全得分：\(s = \sup u^2\)，界限 \(s_0 = 0.64\)（训练集中89.7%轨迹不安全）
* **2D 不可压缩流体**（Navier‑Stokes）
  * 目标：最大化通过目标桶的烟量，\(J\) 为负比率
  * 安全得分：进入危险区域的烟量比例，界值 \(s_0 = 0.1\)（53.1%训练样本不安全）
* **托卡马克核聚变模型**（KSTAR 数据驱动仿真器）
  * 目标：使 \(\beta_p, l_i\) 跟踪目标值，\(J\) 为累积偏差
  * 安全得分：\(s = -\inf q_{95}\)，界值 \(s_0 = -4.98\)（71.18%训练样本不安全）

### 3.2 对比方法
* **BC/BC‑Safe**：行为克隆/仅使用安全轨迹的行为克隆
* **PID**、**SL‑Lag**（监督学习+Lagrange）、**MPC‑Lag**（模型预测控制+Lagrange）
* **CDT**（Constrained Decision Transformer）
* **TREBI**（基于扩散模型的离线安全 RL 规划）

### 3.3 安全评估指标
* \(R_{\text{sample}}\)：不安全轨迹比例（最严格）
* \(R_{\text{time}}\)：不安全时间步比例
* \(R_{\text{point}}\)：不安全空间点比例
* 2D 实验额外引入 \(SVM = \max[s-s_0, 0]\)（违规幅度）

## 四、资源与算力

* 推理耗时对比在 A800 (8 CPUs) 上进行，SafeDiffCon 在 Burgers 方程上用时约 **2.36 分钟**（较 TREBI 的 13.55 分钟快）。
* 文中**没有明确说明训练阶段的 GPU 数量、显存消耗和总训练时长**，仅给出了训练步数（如 200k）和架构参数。算力消耗信息不够透明。

## 五、实验数量与充分性

* **三个物理场景**，每个场景至少 7 种方法对比，包含 1–3 项安全指标和目标函数。
* **消融实验**（2D 流体与 Burgers、Tokamak）：分别去除后训练、推理时微调、不确定性分位数 \(Q\)，展示每个组件的必要性。
* **参数敏感性分析**：在 Tokamak 上变化覆盖概率 \(\alpha\)、训练/校准集分割比；在 2D 流体上变化目标权重 \(\gamma\)。结果稳健。
* 实验覆盖了不同类型的 PDE 控制，与主流离线安全 RL/IL 方法对比，**整体充分且公平**。

## 六、主要结论

* SafeDiffCon 是**唯一在所有三个任务中均完全满足安全约束**的方法，其他基线（含 CDT、TREBI）均出现违规。
* 在满足安全约束的条件下，SafeDiffCon 取得**最优控制性能**（J 最低）。
* 后训练、推理微调和不确定性分位数三个组件缺一不可，共同保障安全性与控制精度。

## 七、优点

* **首次将安全约束引入扩散模型 PDE 控制**，且提供了形式化的不确定性保障。
* 利用**共形预测处理分布偏移**，无需对模型和数据分布做额外假设，具有理论保证。
* **端到端框架**：预训练、后训练、推理微调三个阶段清晰，可灵活植入不同物理场景。
* 实验设计**纳入了高维、强非线性任务**（2D 流体、聚变），验证了方法的可扩展性。

## 八、不足与局限

* **场景局限**：仅在三个特定 PDE 环境上验证，缺乏更广泛真实工业系统（如降膜蒸发器、飞行器）的测试。
* **离线设定**：假设无法与环境交互，完全依赖离线数据；未探索在线安全自适应控制。
* **计算资源描述不足**：未报告训练所需 GPU 数量、训练时长、显存，不利于复现和资源评估。
* **安全保证依赖假设**：共形覆盖要求校准集与测试集满足加权可交换性，实际应用中可能出现更剧烈分布变化，影响安全区间有效性。
* **推理微调虽加速，但依然需数分钟**，可能无法满足高频实时控制需求。

（完）
