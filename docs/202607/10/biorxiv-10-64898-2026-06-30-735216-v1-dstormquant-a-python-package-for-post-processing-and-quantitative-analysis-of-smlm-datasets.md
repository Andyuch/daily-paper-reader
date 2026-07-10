---
title: "dSTORMQuant: A Python Package for Post-Processing and Quantitative Analysis of SMLM datasets"
title_zh: dSTORMQuant：用于 SMLM 数据集后处理与定量分析的 Python 软件包
authors: "Karki, S., Nemeita, B., Hammann, A. S., Thoms, S."
date: 2026-07-03
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.30.735216v1.full.pdf"
tags: ["query:iscat"]
score: 6.0
evidence: 随机光学重建显微镜 (dSTORM) 分析
tldr: 单分子定位显微技术（SMLM）如dSTORM和PALM虽能突破衍射极限，但其数据处理过程复杂且耗时，限制了大规模生物学研究。本文推出了dSTORMQuant，这是一个基于Python的开源软件包，旨在实现SMLM定位数据的自动化、高通量后处理与定量分析。该工具显著降低了人工干预需求，提高了处理效率，为大规模SMLM数据集的统计分析提供了有力支持。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-30-735216-v1/fig-001.webp\", \"caption\": \"Fig. 1: Overview of the dSTORMQuant analysis workflow. A Schematic illustration of the dSTORMQuant processing and analysis pipeline. Arrows indicate the sequential progression from input through processing to analysis. Individual modules are listed beneath each stage. The dashed border of the cell detection module denotes its optional use, depending on experimental requirements. B-E Example results of processing and analysis of a U2OS WT cell stained for mitochondria and peroxisomes as two different organelle markers: B Localization map of Voronoi- and grid-based cell detection. C Localization map by Coordinate-Based Co-localization (CBC) and Relative Enrichment (RE) methods. D DBSCAN (Density-based spatial clustering of applications with noise) result. Scale bar: 10 µm. E Reconstructed dSTORM image using the initial localization list in comparison with the post-processed localization list. The number of localizations per channel is noted on the upper left. Scale bar: 10 µm.\", \"page\": 3, \"index\": 1, \"width\": 902, \"height\": 964}]"
motivation: 针对SMLM数据后处理计算挑战大、耗时长且难以进行大规模统计分析的问题，开发高效的自动化工具。
method: 开发了一个基于Python的开源软件包，集成了自动化、高通量的定位数据后处理与定量分析功能。
result: 实现了对大规模SMLM数据集的高效处理，显著减少了人工干预并提升了数据分析的吞吐量。
conclusion: dSTORMQuant为SMLM研究提供了一个便捷、可靠的定量分析平台，增强了超分辨率成像研究的统计效力。
---

## 摘要
摘要：单分子定位显微技术（SMLM），如（直接）随机光学重建显微术（(d)STORM）和光激活定位显微术（PALM），能够实现超越传统光学显微镜衍射极限的亚细胞分子组织可视化。不仅数据采集过程较为缓慢，定位数据集的下游分析在计算上也往往具有挑战性且耗时。因此，数据处理的复杂性和时长通常限制了实验仅能采集和分析少量的细胞或感兴趣区域，从而制约了 SMLM 研究的统计效力和生物学可靠性。为了解决这一局限性，我们开发了一个基于 Python 的开源软件包，用于 SMLM 定位数据的自动化、高通量后处理和定量分析，能够以极少的人工干预高效且直接地处理大规模数据集。可用性与实现：dSTORMQuant（源代码和文档）可在 GitHub（https://github.com/BCMM-Bielefeld-University/dSTORMQuant）上根据 GPL v3 许可免费获取。

## Abstract
SummarySingle-molecule localization microscopy techniques, such as (direct) stochastic optical reconstruction microscopy ((d)STORM) and photo-activated localization microscopy (PALM) enable the visualization of subcellular molecular organization beyond the diffraction limit of conventional light microscopy. Not only is data acquisition rather slow, but the downstream analysis of localization datasets often remains computationally challenging and time-consuming. Consequently, the complexity and duration of data processing often limit experiments to the acquisition and analysis of only small numbers of cells or regions of interest, thereby restricting the statistical power and biological reliability of SMLM studies. To address this limitation, we developed an open-source Python-based package for automated, high-throughput post-processing and quantitative analysis of SMLM localization data, enabling efficient and straightforward handling of extensive datasets with minimal manual intervention.

Availability and implementationdSTORMQuant (source code and documentation) are freely available on GitHub at https://github.com/BCMM-Bielefeld-University/dSTORMQuant under GPL v3 license.