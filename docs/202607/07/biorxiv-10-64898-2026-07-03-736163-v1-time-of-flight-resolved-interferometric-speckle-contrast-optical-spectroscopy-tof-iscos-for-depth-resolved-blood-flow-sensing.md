---
title: Time-of-flight-resolved interferometric speckle-contrast optical spectroscopy (TOF-iSCOS) for depth-resolved blood-flow sensing
title_zh: 飞行时间分辨干涉散斑对比光学光谱法 (TOF-iSCOS) 用于深度分辨血流传感
authors: "Nowacka-Pieszak, K., Borycki, D., Mogharari, N., Marzejon, M."
date: 2026-07-03
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.03.736163v1.full.pdf"
tags: ["query:iscat"]
score: 7.5
evidence: 用于深度分辨传感的干涉斑点对比光学光谱 (iSCOS)
tldr: 本研究提出了一种飞行时间解析干涉斑点对比光学光谱技术（TOF-iSCOS），旨在解决传统连续波光学血流监测缺乏深度选择性的问题。通过结合扫频光源干涉近红外光谱（iNIRS）与斑点对比分析，该方法利用光子飞行时间区分浅层与深层组织动态。实验证明，该技术能有效抑制加性噪声，并在仿体及人体实验中成功实现了深度解析的血流监测，为可扩展的皮层血流动力学监测提供了新途径。
source: biorxiv
selection_source: fresh_fetch
motivation: 传统的连续波斑点对比光学光谱技术缺乏深度选择性，难以区分皮肤与深层组织（如大脑皮层）的血流动态。
method: 利用扫频光源iNIRS系统获取干涉信号，通过傅里叶变换恢复飞行时间解析的复斑点场，并基于场自相关函数g1间接估计斑点对比度。
result: 该方法在仿体实验中符合理论预期且抗噪性强，在人体实验中成功捕捉到前臂袖带压迫反应及苏独任务期间随深度增加的血流指数变化。
conclusion: TOF-iSCOS结合了干涉测量与飞行时间解析的优势，是一种能够抑制噪声并实现深度解析血流感测的有效平台。
---

## 摘要
意义：对血流相关的组织动力学进行连续、无创且具有深度分辨能力的监测仍是一项重要且尚未满足的需求。散斑对比光学光谱法 (SCOS)，包括如 iSCOS 等干涉实现方式，为血流传感提供了一种可扩展的光学途径，但传统的连续波方法缺乏内在的深度选择性。飞行时间 (TOF) 门控通过分辨光子路径长度，提供了一种分离分层组织（如皮肤-肌肉或头皮-大脑皮层）中浅层和深层动态贡献的方法。目的：我们引入了一种基于扫频光源、单通道实现的干涉散斑对比光学光谱法 (iSCOS)，旨在从测量的电场自相关函数 g1 中获取 TOF 分辨的时间散斑对比度 κ²，并评估其在深度分辨血流传感中的可行性。方法：采用工作在 780 nm 的扫频光源 iNIRS 系统获取干涉信号，沿光频率轴进行傅里叶变换以恢复复数 TOF 分辨散斑场。随后利用散斑可见度关系，从 g1 间接估计每个 TOF 门的时间散斑对比度。首先通过基于扩散理论的数值模拟，在不同的减速散射系数、扩散系数、加性噪声水平和双层几何结构下，比较了直接基于方差的估计器和间接基于 g1 的估计器。模拟结果显示，基于 g1 推导的 κ² 估计器对加性噪声的敏感度显著低于直接估计器，因此该估计器被用于主要的仿体和活体分析，而直接估计器仅作为模拟对照。随后，将基于 g1 的估计器应用于液体和双层仿体，并进行了人体前臂袖带压迫实验和额头数独任务期间的活体概念验证测量。结果：使用基于 g1 的估计器恢复的 TOF 分辨 κ² 曲线在不同散射系数、光子路径长度和曝光时间下均符合 DWS 理论。在加性噪声幅度高达电场幅度 50% 的情况下，该估计器仍能保持理论准确性，而直接方差估计器则表现出显著的噪声诱导偏差并需要校正。双层模拟和仿体实验重现了分层介质中预测的随 TOF 变化的去相关速率趋势的方向和起始点。在活体实验中，恢复的血流指数追踪到了前臂预期的随 TOF 变化的袖带压迫和反应性充血响应。在单受试者数独任务期间，左额头记录显示血流指数随 TOF 增加而相对增加：在 TOF = 400 ps 时为 +0.8 ± 1.9%，在 600 ps 时为 +9.8 ± 2.2%，在 800 ps 时为 +15.2 ± 5.6%。这一模式与长光子路径长度对深层组织敏感度增加的特性一致，但在将其定量解释为认知激活之前，仍需进行群体水平的验证。结论：将时间散斑对比分析与扫频光源 iNIRS 相结合，产生了一个用于血流传感的深度分辨概念验证平台。通过基于 g1 推导 κ² 的路径来估计 TOF 分辨散斑对比度，TOF-iSCOS 在抑制加性噪声偏差的同时，保持了对深层动态组织层的敏感性。目前的单通道结果桥接了连续波 iSCOS、干涉 NIRS 和时域弥散相关光谱法 (TD-DCS)，并为未来用于可扩展皮层血流动力学监测的多通道和群体研究提供了动力。

## Abstract
SignificanceContinuous, noninvasive, and depth-resolved monitoring of blood-flow-related tissue dynamics remains an important unmet need. Speckle-contrast optical spectroscopy (SCOS), including interferometric implementations such as iSCOS, provides a scalable optical route to blood-flow sensing, but conventional continuous-wave approaches lack intrinsic depth selectivity. Time-of-flight (TOF) gating offers a way to separate superficial and deeper dynamic contributions in layered tissues, such as skin- muscle or scalp-cortex, by resolving photon path lengths.

AimWe introduce a swept-source, single-channel implementation of interferometric speckle-contrast optical spectroscopy (iSCOS) to obtain TOF-resolved temporal speckle contrast,{kappa} 2, from the measured field autocorrelation g1, and evaluate its feasibility for depth-resolved blood-flow sensing.

ApproachA swept-source iNIRS system operating at 780 nm acquired interferometric signals, which were Fourier-transformed along the optical-frequency axis to recover complex TOF-resolved speckle fields. Temporal speckle contrast was then estimated at each TOF gate indirectly from g1 using the speckle-visibility relation. Diffusion-based numerical simulations were first used to compare the direct variance-based estimator and the indirect g1-based estimator under varying reduced scattering coefficient, diffusion coefficient, additive noise level, and bi-layer geometry. Because the simulations showed that the g1-derived{kappa} 2 estimator was substantially less sensitive to additive noise than the direct estimator, this estimator was used for the main phantom and in vivo analyses, while the direct estimator served as a simulation comparator. The g1-derived estimator was then applied to liquid and bi-layer phantoms, followed by proof-of-concept in vivo measurements on the human forearm during cuff occlusion and on the forehead during a Sudoku task.

ResultsTOF-resolved{kappa} 2 curves recovered with the g1-derived estimator matched DWS theory across scattering coefficients, photon path lengths, and exposure times. The estimator preserved theoretical accuracy for additive noise amplitudes up to 50% of the field amplitude, whereas the direct variance estimator showed substantial noise-induced bias and required correction. Bi-layer simulations and phantom experiments reproduced the predicted direction and onset of TOF-dependent decorrelation-rate trends in layered media. In vivo, the recovered blood-flow index tracked the expected TOF-dependent cuff-occlusion and reactive-hyperemia response in the forearm. During the single-subject Sudoku task, the left-forehead recording showed a TOF-dependent relative blood-flow-index increase of +0.8 {+/-} 1.9% at TOF = 400 ps, +9.8 {+/-} 2.2% at TOF = 600 ps, and +15.2 {+/-} 5.6% at TOF = 800 ps. This pattern is consistent with increased sensitivity to deeper tissue at longer photon path lengths, but requires cohort-level validation before quantitative interpretation as cognitive activation.

ConclusionsCoupling temporal speckle-contrast analysis with swept-source iNIRS yields a proof-of-concept, depth-resolved platform for blood-flow sensing. By estimating TOF-resolved speckle contrast through the g1-derived{kappa} 2 route, TOF-iSCOS suppresses additive-noise bias while preserving sensitivity to deeper dynamic tissue layers. The present single-channel results bridge continuous-wave iSCOS, interferometric NIRS and time-domain diffuse correlation spectroscopy (TD-DCS), and motivate future multi-channel and cohort studies for scalable cortical hemodynamic monitoring.