

<div align="center">
<h1> M4V: Multi-Modal Mamba for Text-to-Video Generation</h1>
<h3></h3>

Jiancheng Huang<sup>1</sup>, Gengwei Zhang<sup>2</sup>, ZEQUN JIE<sup>1</sup>,Siyu Jiao<sup>3</sup>, Yinlong Qian<sup>1</sup>, Ling Chen<sup>2</sup>,  
Yunchao Wei<sup>3</sup>, Lin Ma<sup>1</sup>

<sup>1</sup> Meituan BJTU, <sup>2</sup> UTS, <sup>3</sup> BJTU


[![arXiv](https://img.shields.io/badge/arXiv%20paper-2506.10915-b31b1b.svg)](https://arxiv.org/abs/2506.10915)&nbsp;
[![Project&Videos](https://img.shields.io/badge/%F0%9F%8E%AC%20Project&Videos-MV4/project-yellow)](https://huangjch526.github.io/M4V_project/)&nbsp;



</div>

<div align="center">
<img src="resources/abs.png" width="958%">
</div>

## Introduction

Text-to-video generation has significantly enriched content creation and holds the potential to evolve into powerful world simulators. However, modeling the vast spatiotemporal space remains computationally demanding, particularly when employing Diffusion Transformers (DiTs), which incur quadratic complexity in sequence processing, thereby limiting its practical applications. Recent advancements in linear-time sequence modeling, particularly the Mamba architecture, offer a more efficient alternative to Transformers. Nevertheless, its plain design constrains its direct application to multi-modal and spatiotemporal video generation tasks. To address these challenges, we introduce M4V, a Multi-Modal Mamba framework for text-to-video generation. Specifically, we introduce a multi-modal diffusion Mamba (MM-DiM) block that enables seamless multi-modal integration and spatiotemporal modeling within an autoregressive generation pipeline. Additionally, to mitigate error accumulation in long-context autoregressive processes, we introduce a reward learning strategy to enhance per-frame consistency and quality. As a result, the Mamba blocks in M4V reduce the FLOPs by 45\% compared to the attention alternative when generating 121-frame videos at 768×1280 resolution. Extensive experiments on text-to-video benchmarks demonstrate M4V's ability to produce high-quality videos while significantly lowering computational costs. Code and models will be publicly available.





### Acknowledgement
[PyramidFlow](https://openaccess.thecvf.com/content/CVPR2023/html/Lei_PyramidFlow_High-Resolution_Defect_Contrastive_Localization_Using_Pyramid_Normalizing_Flow_CVPR_2023_paper.html?ref=https://githubhelp.com)

[Mamba](https://minjiazhang.github.io/courses/fall24-resource/Mamba.pdf)

[Zigma](https://link.springer.com/chapter/10.1007/978-3-031-72664-4_9)
