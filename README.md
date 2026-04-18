<h1 align="center">Awsome-3D</h1>

<p align="center"><b>一个面向 3D 视觉、三维重建、3D 生成与具身感知的中文导航仓库</b></p>

<p align="center">
  <img src="https://img.shields.io/github/stars/SII-LiMing/Awsome-3D?style=flat-square" alt="GitHub stars" />
  <img src="https://img.shields.io/github/license/SII-LiMing/Awsome-3D?style=flat-square" alt="License" />
  <img src="https://img.shields.io/github/last-commit/SII-LiMing/Awsome-3D?style=flat-square" alt="Last Commit" />
</p>

> `Awsome-3D` 的目标不是堆砌链接，而是把 3D 相关的重要方向、开源工具、代表性任务与学习路线组织成一个清晰的入口，方便快速建立全局认知，并逐步沉淀成可检索、可维护的资料库。
> 现阶段主要 focus 在 3DGen

## News｜项目进展

- `2026-04-18`: 仓库创建

<!-- ## Start From Here｜从这里开始

### 仓库定位

这个仓库主要面向以下几类问题：

- 3D 视觉：点云、网格、隐式表示、三维检测、分割、定位、场景理解。
- 三维重建：SfM、MVS、NeRF、3D Gaussian Splatting、SLAM、重定位。
- 3D 生成：Text-to-3D、Image-to-3D、Mesh / Texture 生成、3D Asset Creation。
- 具身与机器人 3D 感知：面向操作、导航、仿真与场景交互的三维建模与理解。
- 工程工具链：数据处理、可视化、渲染、训练框架、Benchmark 与评测。

### 如何使用这份仓库

- 如果你是初学者，先看“研究版图”和“推荐起步工具”，建立全局地图。
- 如果你已经在做研究，直接跳到对应方向，筛选工具、项目和数据集。
- 如果你希望搭系统，优先关注工具链、数据格式、评测方式和工程实现。 -->

## 目录

- [Paper List](#paper-list)
- [Model Architecture](#model-architecture)
- [3DGen](#3dgen)
- [独立 Paper List 文件](./paperlist.md#paper-list)
- [常用算法](#common-algorithms)
- [点云](#point-cloud)
- [相机内外参](#camera-calibration-and-pose)
- [其他](#misc-algorithms)

<a id="paper-list"></a>
## Paper List

完整可维护版本见 [paperlist.md](./paperlist.md#paper-list)。

<a id="model-architecture"></a>
#### Model Architecture

以下是常用的模型架构相关文章，建议按时间顺序先把基础表征与生成范式补齐，再进入 3DGen。

- [Transformer: Attention Is All You Need](https://arxiv.org/abs/1706.03762)
- [VAE: Auto-Encoding Variational Bayes](https://arxiv.org/abs/1312.6114)
- [ViT: An Image Is Worth 16x16 Words](https://arxiv.org/abs/2010.11929)
- [DINO: Emerging Properties in Self-Supervised Vision Transformers](https://arxiv.org/abs/2104.14294)
- [DINOv2: Learning Robust Visual Features without Supervision](https://arxiv.org/abs/2304.07193) | [Code](https://github.com/facebookresearch/dinov2)
- [DINOv3](https://arxiv.org/abs/2508.10104) | [Code](https://github.com/facebookresearch/dinov3)
- [DDPM: Denoising Diffusion Probabilistic Models](https://arxiv.org/abs/2006.11239)
- [DDIM: Denoising Diffusion Implicit Models](https://arxiv.org/abs/2010.02502)
- [Stable Diffusion / LDM: High-Resolution Image Synthesis with Latent Diffusion Models](https://arxiv.org/abs/2112.10752)
- [DiT: Scalable Diffusion Models with Transformers](https://arxiv.org/abs/2212.09748)
- [Flow Matching for Generative Modeling](https://arxiv.org/abs/2210.02747)
- [3DShape2VecSet: A 3D Shape Representation for Neural Fields and Generative Diffusion Models](https://arxiv.org/abs/2301.11445) | [Project Page](https://1zb.github.io/3DShape2VecSet/) | [Code](https://github.com/1zb/3DShape2VecSet)

<a id="3dgen"></a>
#### 3DGen

从单张图像或文本出发得到三维资产的工作，这里统一归类为 3DGen。当前列表主要聚焦单物体生成。

- [CLAY: A Controllable Large-scale Generative Model for Creating High-quality 3D Assets](https://arxiv.org/abs/2406.13897)
- [TRELLIS: Structured 3D Latents for Scalable and Versatile 3D Generation](https://arxiv.org/abs/2412.01506) | [Project Page](https://microsoft.github.io/TRELLIS/) | [Code](https://github.com/microsoft/TRELLIS)
- [TRELLIS.2: Native and Compact Structured Latents for 3D Generation](https://arxiv.org/abs/2512.14692) | [Project Page](https://microsoft.github.io/TRELLIS.2) | [Code](https://github.com/microsoft/TRELLIS.2)
- [Hunyuan3D-1.0: A Unified Framework for Text-to-3D and Image-to-3D Generation](https://arxiv.org/abs/2411.02293) | [Code](https://github.com/Tencent-Hunyuan/Hunyuan3D-1)
- [Hunyuan3D 2.0: Scaling Diffusion Models for High Resolution Textured 3D Assets Generation](https://arxiv.org/abs/2501.12202) | [Code](https://github.com/Tencent-Hunyuan/Hunyuan3D-2)
- [Hunyuan3D 2.1: From Images to High-Fidelity 3D Assets with Production-Ready PBR Material](https://arxiv.org/abs/2506.15442) | [Code](https://github.com/Tencent-Hunyuan/Hunyuan3D-2.1)
- [SAM 3D: 3Dfy Anything in Images](https://arxiv.org/abs/2511.16624)
- [CUPID: Generative 3D Reconstruction via Joint Object and Pose Modeling](https://arxiv.org/abs/2510.20776) | [Project Page](https://cupid3d.github.io/) | [Code](https://github.com/cupid3d/Cupid)
- [Omni123: Exploring 3D Native Foundation Models with Limited 3D Data by Unifying Text to 2D and 3D Generation](https://arxiv.org/abs/2604.02289)

<a id="common-algorithms"></a>
## 常用算法

<a id="point-cloud"></a>
### 点云

- [FPS / Farthest Point Sampling](https://arxiv.org/abs/1706.02413)

<a id="camera-calibration-and-pose"></a>
### 相机内外参

- [PnP 算法](https://docs.opencv.org/4.x/d5/d1f/calib3d_solvePnP.html) | [本仓库 notebook](./algorithm/pnp_solver.ipynb)
- [Umeyama Method](https://zpl.fi/aligning-point-patterns-with-kabsch-umeyama-algorithm/)

<a id="misc-algorithms"></a>
### 其他

- [匈牙利匹配 / Hungarian Algorithm](https://en.wikipedia.org/wiki/Hungarian_algorithm)




## License｜许可协议

本仓库采用 [MIT License](./LICENSE)。

如果后续仓库中收录第三方内容、图片或论文摘要，其版权归原作者或原项目所有；本仓库仅负责整理与索引。
