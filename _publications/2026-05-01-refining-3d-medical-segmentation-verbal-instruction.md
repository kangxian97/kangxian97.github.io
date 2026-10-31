---
title: "Refining 3D Medical Segmentation with Verbal Instruction"
collection: publications
dataseturl: "https://zenodo.org/records/20113566"
codeurl: "https://github.com/HINTLab/CowTalk"
authors: "Kangxian Xie, Jiancheng Yang, Nandor Pinter, Chao Wu, Behzad Bozorgtabar, Mingchen Gao"
venue_short: "MICCAI 2026"
project_name: "CoWTalk"
category: conferences
permalink: /publication/2026-refining-3d-medical-segmentation-verbal-instruction
link: 'https://arxiv.org/abs/2603.14496'
excerpt: "Language-guided, iterative refinement of 3D arterial segmentations with a benchmark of anatomical errors and corrective instructions."
date: 2026-05-01
venue: 'Medical Image Computing and Computer Assisted Intervention (MICCAI)'
paperurl: "https://papers.miccai.org/miccai-2026/0871-Paper0740.html"
citation: 'K. Xie, J. Yang, N. Pinter, C. Wu, B. Bozorgtabar and M. Gao, "Refining 3D Medical Segmentation with Verbal Instruction," in Proc. MICCAI, 2026. arXiv:2603.14496.'
---

Accurate 3D anatomical segmentation is essential for clinical diagnosis and surgical planning. Automated models often produce suboptimal shapes due to limited data, labeling noise, and distribution shift. We study iterative refinement from radiologists’ verbal instructions—a setting hindered by scarce paired data linking erroneous shapes to corrective language. We introduce **CoWTalk**, a benchmark with 3D arterial anatomies, controllable synthesized anatomical errors, and corresponding repairing instructions. Building on it, we propose an iterative refinement model that represents 3D shapes as vector sets and interacts with text to progressively update the segmentation. Experiments show strong gains over corrupted inputs and competitive baselines, supporting language-driven, clinician-in-the-loop refinement for 3D medical shapes.
