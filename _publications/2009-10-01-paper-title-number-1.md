---
title: "S3-TTA: Scale-Style Selection for Test-Time Augmentation in Biomedical Image Segmentation"
collection: publications
codeurl: "https://github.com/kangxian97/S3-TTA"
venue_short: "ISBI 2024"
category: conferences
permalink: /publication/2009-10-01-paper-title-number-1
excerpt: "Selecting image scale and style at test time to improve generalization in biomedical image segmentation."
date: 2024-05-30
venue: 'IEEE International Symposium on Biomedical Imaging (ISBI)'
#slidesurl: 'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://ieeexplore.ieee.org/document/10635833'
citation: 'K. Xie, S. Huang, S. C. Ordonez, H. Pfister and D. Wei, "S3-TTA: Scale-Style Selection for Test-Time Augmentation in Biomedical Image Segmentation," 2024 IEEE International Symposium on Biomedical Imaging (ISBI), Athens, Greece, 2024, pp. 1-5, doi: 10.1109/ISBI56570.2024.10635833.'
---

Deep-learning models have been successful in biomedical image segmentation. To generalize for real-world deployment, test-time augmentation (TTA) methods are often used to transform the test image into different versions that are hopefully closer to the training domain. However, due to the diversity of instance scale and styles, many augmented test images produce undesirable results, lowering the overall performance. This work proposes a new TTA framework, S3-TTA, which selects the suitable image scale and style for each test image based on a transformation consistency metric. In addition, S3-TTA constructs an end-to-end augmentation-segmentation joint-training pipeline to ensure a task-oriented augmentation. On public benchmarks for cell and lung segmentation, S3-TTA demonstrates
improvements over the prior art by 3.4% and 1.3%, respectively, by simply augmenting the input data in testing phase. Code and models are available at [GitHub](https://github.com/kangxian97/S3-TTA).
