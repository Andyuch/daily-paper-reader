---
title: Multi-state Ensemble Refinement for Occupancy Statistics (MEROS) in Time-Resolved X-ray Crystallography
title_zh: 时间分辨X射线晶体学中的多状态系综精修占有率统计 (MEROS)
authors: "Prester, A., Spiliopoulou, M., Schulz, E. C."
date: 2026-05-07
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.04.722701v1.full.pdf"
tags: ["query:iscat"]
score: 6.5
evidence: 时间分辨晶体学中占有率统计的系综精修
tldr: 在时间分辨X射线晶体学中，准确确定状态占据率受限于占据率与原子位移参数（ADP）之间的强相关性。本文提出MEROS流程，通过蒙特卡洛采样和独立精修评估重叠状态的占据率-ADP统计分布。该方法能有效量化实验数据的确定性，并在溶菌酶和β-内酰胺酶案例中验证了其可靠性，为结构异质性分析提供了新工具。
source: biorxiv
selection_source: fresh_fetch
motivation: 针对时间分辨晶体学中状态重叠导致的占据率与原子位移参数强相关、使单点估计不可靠的问题。
method: 开发了基于蒙特卡洛采样的MEROS流程，通过从随机初始值进行多次独立精修来表征参数空间的收敛性和不确定性。
result: 在T4溶菌酶和β-内酰胺酶的案例中，该方法成功给出了占据率和ADP的统计均值与标准差，直接量化了实验数据的信息含量。
conclusion: MEROS为多状态系综精修提供了一种稳健的统计评估方案，显著提升了对复杂晶体结构异质性的解释能力。
---

## 摘要
准确确定状态占有率对于解释时间分辨晶体学中固有的结构异质性至关重要。然而，在状态之间存在高度空间重叠的情况下（这在时间分辨晶体学数据中很常见），占有率与原子位移参数 (ADPs) 之间的强相关性可能导致标准精修方案的单点估计变得不可靠。我们介绍了 MEROS（Multi-state Ensemble Refinement for Occupancy Statistics），这是一个实现系综精修方法的管线，用于评估多个重叠状态精修后的占有率-ADP 统计数据。MEROS 利用参数空间的蒙特卡罗采样，通过从随机化的起始占有率和 ADP 值进行独立精修，来经验性地表征解的收敛性和不确定性。该方法作为一个模块化的 Python 管线实现，封装了成熟的精修程序，确保了与现有工作流的兼容性。我们在两个案例研究中展示了其适用性：T4 溶菌酶 L99A 中的双状态配体结合模型，以及 β-内酰胺酶 CTX-M-14 中的四状态共价催化机制。MEROS 提供的占有率和 ADP 平均值及标准差，直接量化了实验衍射数据的信息含量。

## Abstract
Accurate determination of state occupancies is essential for interpreting the structural heterogeneity inherent in time-resolved crystallography. However, in cases of high spatial overlap between states, as commonly observed in time-resolved crystallography data, the strong correlation between occupancy and atomic displacement parameters (ADPs) can render single point estimates from standard refinement protocols unreliable. We introduce MEROS (Multi-state Ensemble Refinement for Occupancy Statistics), a pipeline that implements an ensemble refinement approach to assess the post-refinement occupancy-ADP statistics of multiple overlapping states. MEROS utilizes a Monte Carlo sampling of the parameter space, performing independent refinements from randomized starting occupancies and ADP values to empirically characterize the convergence and uncertainty of the solution. The method is implemented as a modular Python pipeline that wraps established refinement programs, ensuring compatibility with existing workflows. We demonstrate its applicability in two case studies: a two-state ligand binding model in T4 lysozyme L99A and a four-state covalent catalysis mechanism in beta-lactamase CTX-M-14. MEROS provides occupancy and ADP mean values with standard deviations that directly quantify the informational content of the experimental diffraction data.