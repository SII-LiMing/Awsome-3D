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
- [常用算法](#common-algorithms)

<a id="paper-list"></a>
## Paper List

为避免 `XXX: ...` 这种原始论文标题和简称混在一起，下面统一采用 `[简称] 标题` 的排版方式。

<a id="model-architecture"></a>
#### Model Architecture

以下是常用的模型架构相关文章，建议按时间顺序先把基础表征与生成范式补齐，再进入 3DGen。

- **[Transformer]** [Attention Is All You Need](https://arxiv.org/abs/1706.03762)
- **[VAE]** [Auto-Encoding Variational Bayes](https://arxiv.org/abs/1312.6114)
- **[ViT]** [An Image Is Worth 16x16 Words](https://arxiv.org/abs/2010.11929)
- **[DINO]** [Emerging Properties in Self-Supervised Vision Transformers](https://arxiv.org/abs/2104.14294)
- **[DINOv2]** [Learning Robust Visual Features without Supervision](https://arxiv.org/abs/2304.07193) | [Code](https://github.com/facebookresearch/dinov2)
- **[DINOv3]** [Paper](https://arxiv.org/abs/2508.10104) | [Code](https://github.com/facebookresearch/dinov3)
- **[DDPM]** [Denoising Diffusion Probabilistic Models](https://arxiv.org/abs/2006.11239)
- **[DDIM]** [Denoising Diffusion Implicit Models](https://arxiv.org/abs/2010.02502)
- **[Stable Diffusion / LDM]** [High-Resolution Image Synthesis with Latent Diffusion Models](https://arxiv.org/abs/2112.10752)
- **[DiT]** [Scalable Diffusion Models with Transformers](https://arxiv.org/abs/2212.09748)
- **[Flow Matching]** [Flow Matching for Generative Modeling](https://arxiv.org/abs/2210.02747)
- **[3DShape2VecSet]** [A 3D Shape Representation for Neural Fields and Generative Diffusion Models](https://arxiv.org/abs/2301.11445) | [Project Page](https://1zb.github.io/3DShape2VecSet/) | [Code](https://github.com/1zb/3DShape2VecSet)

<a id="3dgen"></a>
#### 3DGen

从单张图像或文本出发得到三维资产的工作，这里统一归类为 3DGen。当前列表主要聚焦单物体生成。

- **[CLAY]** [A Controllable Large-scale Generative Model for Creating High-quality 3D Assets](https://arxiv.org/abs/2406.13897)
- **[TRELLIS]** [Structured 3D Latents for Scalable and Versatile 3D Generation](https://arxiv.org/abs/2412.01506) | [Project Page](https://microsoft.github.io/TRELLIS/) | [Code](https://github.com/microsoft/TRELLIS)
- **[TRELLIS.2]** [Native and Compact Structured Latents for 3D Generation](https://arxiv.org/abs/2512.14692) | [Project Page](https://microsoft.github.io/TRELLIS.2) | [Code](https://github.com/microsoft/TRELLIS.2)
- **[Hunyuan3D-1.0]** [A Unified Framework for Text-to-3D and Image-to-3D Generation](https://arxiv.org/abs/2411.02293) | [Code](https://github.com/Tencent-Hunyuan/Hunyuan3D-1)
- **[Hunyuan3D 2.0]** [Scaling Diffusion Models for High Resolution Textured 3D Assets Generation](https://arxiv.org/abs/2501.12202) | [Code](https://github.com/Tencent-Hunyuan/Hunyuan3D-2)
- **[Hunyuan3D 2.1]** [From Images to High-Fidelity 3D Assets with Production-Ready PBR Material](https://arxiv.org/abs/2506.15442) | [Code](https://github.com/Tencent-Hunyuan/Hunyuan3D-2.1)
- **[SAM 3D]** [3Dfy Anything in Images](https://arxiv.org/abs/2511.16624)
- **[CUPID]** [Generative 3D Reconstruction via Joint Object and Pose Modeling](https://arxiv.org/abs/2510.20776) | [Project Page](https://cupid3d.github.io/) | [Code](https://github.com/cupid3d/Cupid)
- **[Omni123]** [Exploring 3D Native Foundation Models with Limited 3D Data by Unifying Text to 2D and 3D Generation](https://arxiv.org/abs/2604.02289)

#### Conferences

> CCF 等级参考 [CCF 第七版（2026-03）在线检索](https://ccf.atom.im/)。下面的“分类”是为了方便快速筛选，不等同于 CCF 原始学科分类；这里只列常见且适合 3D 方向投稿的 venue。

| Venue | 分类 | CCF | 适合的 3D 方向 | 简介 |
| --- | --- | --- | --- | --- |
| [CVPR](https://cvpr.thecvf.com/) | CV | A | 3D detection, reconstruction, generation | 年会，CV 旗舰会，3D 论文量很大。 |
| [ICCV](https://iccv.thecvf.com/) | CV | A | 3D perception, geometry, generative 3D | 仅奇数年举办，与 CVPR 并列顶会。 |
| [ECCV](https://eccv.ecva.net/) | CV | B | multi-view geometry, 3D understanding | 仅偶数年举办，欧洲 CV 旗舰会。 |
| [3DV](https://3dvconf.github.io/2026/) | 3D Vision | C | reconstruction, pose, geometry, SLAM | 纯 3D 视觉会议，对口度很高。 |
| [NeurIPS](https://neurips.cc/) | AI/ML | A | 3D foundation models, world models, generative 3D | 年会，偏方法创新与学习范式。 |
| [ICLR](https://iclr.cc/) | AI/ML | A | representation learning, diffusion, 3D generation | 年会，偏表示学习与生成建模。 |
| [ICML](https://icml.cc/) | AI/ML | A | large-scale learning, 3D generative modeling | 年会，偏机器学习方法本身。 |
| [SIGGRAPH](https://www.siggraph.org/) | 图形学 | A | rendering, geometry, animation, asset creation | 年会，图形学旗舰，3D 资产与渲染工作集中。 |
| [Eurographics](https://conferences.eg.org/) | 图形学 | B | geometry processing, rendering, animation | 年会，欧洲图形学旗舰，对 3D 几何较友好。 |
| [IEEE VR](https://ieeevr.org/) | XR/3D交互 | A | 3D interaction, rendering, VR/AR systems | 年会，偏虚拟现实与 3D 用户交互。 |
| [IEEE VIS](https://ieeevis.org/) | 可视化 | A | volume rendering, scientific visualization, geometry vis | 年会，偏可视化而非通用 CV。 |
| [ISMAR](https://www.ismar.net/) | XR/AR | B | tracking, 3D reconstruction, scene understanding | 年会，偏 AR/MR 场景理解与交互。 |
| [ICRA](https://www.ieee-ras.org/conferences-workshops/fully-sponsored/icra) | 机器人 | B | 3D perception, SLAM, manipulation | 年会，机器人旗舰会，感知和控制并重。 |
| [IROS](https://www.ieee-ras.org/conferences-workshops/financially-co-sponsored/iros) | 机器人 | C | navigation, 3D perception, embodied systems | 年会，机器人范围更广，系统 work 较多。 |

#### Journals

| Venue | 分类 | CCF | 适合的 3D 方向 | 简介 |
| --- | --- | --- | --- | --- |
| [TPAMI](https://www.computer.org/csdl/journal/tp) | CV | A | 3D vision, recognition, learning | 视觉/模式识别顶刊，适合更完整的方法论文。 |
| [IJCV](https://link.springer.com/journal/11263) | CV | A | multi-view geometry, 3D understanding, reconstruction | CV 顶刊，通常更强调完整故事和系统实验。 |
| [TOG](https://dl.acm.org/journal/tog) | 图形学 | A | graphics, geometry, rendering, 3D generation | 图形学顶刊；SIGGRAPH/SIGGRAPH Asia 论文常与 TOG 发表体系相关。 |
| [TVCG](https://www.computer.org/csdl/journal/tg) | 图形学/可视化/XR | A | visualization, XR, rendering, 3D interaction | 与 IEEE VIS / VR 社区联系紧密。 |
| [CVIU](https://www.sciencedirect.com/journal/computer-vision-and-image-understanding) | CV | B | 3D vision, scene understanding, geometry | CV 老牌期刊，适合实验较完整的 3D 工作。 |
| [TR](https://www.ieee-ras.org/publications/t-ro) | 机器人 | B | SLAM, 3D perception, manipulation, robot learning | 机器人代表期刊，偏系统与方法结合。 |

<a id="common-algorithms"></a>
## 常用算法

<a id="point-cloud"></a>
### 点云

- [FPS / Farthest Point Sampling](https://arxiv.org/abs/1706.02413)

<a id="camera-calibration-and-pose"></a>
### 相机内外参

- [PnP 算法](./algorithm/pnp_solver.ipynb) 
- [Umeyama Method](https://zpl.fi/aligning-point-patterns-with-kabsch-umeyama-algorithm/)

<a id="misc-algorithms"></a>
### 其他

- [匈牙利匹配 / Hungarian Algorithm](https://en.wikipedia.org/wiki/Hungarian_algorithm)

## License｜许可协议

本仓库采用 [MIT License](./LICENSE)。

如果后续仓库中收录第三方内容、图片或论文摘要，其版权归原作者或原项目所有；本仓库仅负责整理与索引。
