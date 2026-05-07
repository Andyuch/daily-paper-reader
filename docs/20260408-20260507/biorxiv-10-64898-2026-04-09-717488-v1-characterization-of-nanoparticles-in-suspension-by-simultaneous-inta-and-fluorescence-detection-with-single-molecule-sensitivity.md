---
title: Characterization of Nanoparticles in Suspension by Simultaneous iNTA and Fluorescence Detection with Single-Molecule Sensitivity
title_zh: 通过具有单分子灵敏度的同步 iNTA 和荧光检测对悬浮液中的纳米颗粒进行表征
authors: "Jiang, S., Kashkanova, A. D., Lee, H., Miller, M. E. C., Utikal, T., Shkarin, A., Qazvini, H., Sandoghdar, V."
date: 2026-04-13
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.09.717488v1.full.pdf"
tags: ["query:iscat"]
score: 9.0
evidence: 用于纳米颗粒性质的干涉纳米颗粒追踪分析 (iNTA)
tldr: 纳米颗粒特性的定量表征在科研中至关重要，但高精度测量极具挑战。本文在干涉纳米颗粒追踪分析（iNTA）基础上，融合了单分子灵敏度的多色荧光检测，开发出iNTA-F技术。该方法在保留iNTA测定粒径、浓度和折射率优势的同时，增加了生化特异性。通过对脂质囊泡和细胞外囊泡的实验，证明了其在区分复杂混合物亚群方面的卓越性能，为纳米材料表征提供了新工具。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在克服现有纳米颗粒表征技术在同时获取物理属性与生化特异性信息方面的不足。
method: 开发了iNTA-F技术，将无标记干涉成像与高灵敏度多色荧光检测相结合进行同步测量。
result: 成功实现了对不同材质、尺寸及荧光强度的纳米颗粒以及生物细胞外囊泡的精确区分与表征。
conclusion: iNTA-F技术为复杂生物样本中纳米颗粒的多参数、高灵敏度分析提供了一种强有力的非侵入式手段。
---

## 摘要
对纳米颗粒性质的定量了解在大量科学和技术应用中都是非常理想的，但高精度的测量通常极具挑战性。在各种现有方法中，具有单颗粒灵敏度的光学技术特别引人注目，因为它们能以快速、非侵入性的方式揭示内在的异质性。最近，我们提出了干涉纳米颗粒跟踪分析（iNTA），这是一种高灵敏度的无标记技术，能够确定悬浮混合物中不同亚群的尺寸、浓度和折射率。在此，我们通过单分子灵敏度极限下的多色荧光检测，增强了该方法的生化特异性。我们通过区分不同材料、尺寸和荧光强度的荧光与非荧光纳米颗粒群体，对这种命名为 iNTA-F 的组合技术性能进行了基准测试，并重点表征了脂质囊泡和生物细胞外囊泡（EVs）。

## Abstract
Quantitative knowledge of nanoparticle properties is desirable in a large number of scientific and technological applications, but measurements with a high degree of precision usually prove to be challenging. Among a range of available methodologies, optical techniques with single particle sensitivity are especially interesting because they can reveal intrinsic hetero-geneities in a fast non-invasive manner. Recently, we presented interferometric nanoparticle tracking analysis (iNTA) as a highly sensitive label-free technique that is capable of determining the size, concentration and index of refraction of different subpopulations in a suspension mixture. Here, we enhance this method with biochemical specificity through multicolor fluorescence detection at the single-molecule sensitivity limit. We benchmark the performance of the combined technique, which we name iNTA-F, by distinguishing populations of fluorescent and non-fluorescent nanoparticles of different material, size, and fluorescence intensity, with an emphasis on the characterization of lipid vesicles and biological extracellular vesicles (EVs).

---

## 论文详细总结（自动生成）

这篇论文介绍了一种名为 **iNTA-F** 的新型纳米颗粒表征技术，以下是对该研究的结构化总结：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心问题**：如何在保持高通量、非侵入性的前提下，同时实现对悬浮液中单个纳米颗粒（如细胞外囊泡 EVs、脂质体等）的**物理属性**（尺寸、折射率）和**生化特异性**（表面标记物）的精确表征。
*   **研究背景**：传统的电子显微镜（EM）分辨率高但通量低且需真空环境；现有的光学无标记技术（如 iSCAT/iNTA）虽能测量尺寸和折射率，但缺乏区分特定生物分子的能力。因此，开发一种结合干涉成像与单分子荧光检测的同步测量系统具有重要的生物医学价值。

### 2. 论文提出的方法论：iNTA-F
*   **核心思想**：将**干涉纳米颗粒追踪分析（iNTA）**与**多色荧光检测**集成在同一光学平台上，实现对单个扩散颗粒的同步多参数测量。
*   **关键技术细节**：
    *   **iNTA 部分**：利用 638nm 激光进行干涉散射成像（iSCAT），以极高帧率（5000 fps）记录颗粒的布朗运动轨迹，通过扩散系数计算粒径，并通过散射对比度推算折射率。
    *   **荧光部分**：集成 488nm 和 561nm 激发光源，通过交错（Interlaced）激发模式避免光谱串扰，实现单分子级别的荧光灵敏度。
    *   **同步与流控**：使用 Arduino 微控制器同步高频 iSCAT 相机与低频荧光相机；引入微流控系统持续刷新样本，以减轻荧光漂白的影响。
    *   **算法流程**：采用中值背景校正、径向方差变换（RVT）进行颗粒定位，利用 `trackpy` 进行轨迹追踪，并将荧光信号与 iNTA 轨迹在时空上进行匹配。

### 3. 实验设计
*   **基准测试（Benchmark）**：
    *   **单分子灵敏度验证**：在玻璃表面旋涂 Alexa Fluor 488 和 DyLight 550 染料，通过分步光漂白（Stepwise Photobleaching）确认单分子检测能力。
    *   **定量荧光分析**：使用不同染料浓度的 MemBright 488 标记脂质体，建立荧光强度与分子数量的对应关系。
*   **混合样本区分**：测试了由 30nm 金纳米颗粒、40nm 红色荧光球和 100nm 绿色荧光球组成的复杂混合物。
*   **生物应用场景**：对 HEK293 细胞来源的细胞外囊泡（EVs）进行免疫荧光标记（抗 CD9 和抗 CD81），分析其亚群分布。

### 4. 资源与算力
*   **硬件设备**：论文详细描述了定制的宽场显微镜系统，包括高灵敏度 CMOS 和 sCMOS 相机。
*   **算力说明**：文中**未明确提及**具体的 GPU 型号或大规模计算集群的使用。由于该研究侧重于实验物理和生物分析，其数据处理主要依赖于 Python 环境下的图像处理库（如 `trackpy`），计算需求主要集中在单颗粒轨迹追踪和信号提取上，而非深度学习训练。

### 5. 实验数量与充分性
*   **实验规模**：
    *   对脂质体进行了 5 种不同染料浓度的对比实验。
    *   对 EVs 进行了单标记（CD9 或 CD81）和双标记（CD9+CD81）的多组实验。
    *   每组实验通常追踪并分析了数百个（如 163 个或更多）有效颗粒轨迹。
*   **充分性与客观性**：实验设计包含了严格的对照组（如未标记样本）和“帧错位分析”（Frame-mismatched analysis）来评估假阳性率。通过分步光漂白进行定量校准，确保了荧光分子计数的客观性。

### 6. 论文的主要结论与发现
*   **技术可行性**：iNTA-F 能够成功关联单个颗粒的物理尺寸、折射率与生化标记物信息。
*   **生物学发现**：在 HEK293 EVs 的研究中，发现 CD81 阳性比例（48%）高于 CD9 阳性比例（32%），且双阳性亚群占 28%。实验还观察到 EV 的荧光强度随尺寸增加而增加，表明较大囊泡携带更多表面蛋白。
*   **性能指标**：该系统在检测 50nm 以下小颗粒方面具有显著优势，且能区分折射率极近的亚群。

### 7. 优点
*   **多维度表征**：在单颗粒水平上同时提供尺寸、折射率、浓度和分子拷贝数。
*   **极高灵敏度**：达到了单分子荧光检测极限，能够识别仅携带 1-2 个荧光分子的微弱信号。
*   **非侵入性与高通量**：相比电镜，该方法在水溶液原位测量，且数据采集速度快。
*   **消除串扰**：创新的交错激发方案有效解决了多色荧光检测中的光谱重叠问题。

### 8. 不足与局限
*   **光漂白挑战**：尽管使用了流控系统，但扩散颗粒在进入视野前可能已发生部分光漂白，影响定量准确性。
*   **粒径限制**：受限于布朗运动追踪，对于极大或极小的颗粒（超出 iSCAT 检测范围或扩散过快）可能存在测量偏差。
*   **系统复杂性**：定制化的光学系统和多相机同步对实验操作和维护要求较高。
*   **背景干扰**：在处理高背景荧光的样本（如游离染料过多）时，假阳性风险依然存在。

（完）
