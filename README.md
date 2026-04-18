<h1 align="center">Awsome-3D</h1>

<p align="center"><b>一个面向 3D 视觉、三维重建、3D 生成与具身感知的中文导航仓库</b></p>

<p align="center">
  <img src="https://img.shields.io/github/stars/SII-LiMing/Awsome-3D?style=flat-square" alt="GitHub stars" />
  <img src="https://img.shields.io/github/license/SII-LiMing/Awsome-3D?style=flat-square" alt="License" />
  <img src="https://img.shields.io/github/last-commit/SII-LiMing/Awsome-3D?style=flat-square" alt="Last Commit" />
</p>

> `Awsome-3D` 的目标不是堆砌链接，而是把 3D 相关的重要方向、开源工具、代表性任务与学习路线组织成一个清晰的入口，方便快速建立全局认知，并逐步沉淀成可检索、可维护的资料库。

## News｜项目进展

- `2026-04-18`: 初始化仓库，补充首页 README 与 LICENSE。
- `2026-04-18`: 明确仓库定位为 3D 方向的中文资料导航与开源项目索引。

## (1) Start From Here｜从这里开始

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
- 如果你希望搭系统，优先关注工具链、数据格式、评测方式和工程实现。

## (2) Research Map｜3D 研究版图

### 2.1 3D Foundations｜基础能力

- 多视图几何、相机模型、位姿估计、PnP、Bundle Adjustment。
- 点云、体素、网格、SDF、NeRF、3DGS 等三维表示。
- 渲染基础：Rasterization、Ray Marching、Differentiable Rendering。

### 2.2 3D Reconstruction｜三维重建

- 传统重建：SfM、MVS、TSDF、Poisson Surface Reconstruction。
- 神经重建：NeRF 系列、Dynamic NeRF、Feed-forward Reconstruction。
- 实时与工程化重建：SLAM、RGB-D Mapping、3DGS Real-time Rendering。

### 2.3 3D Generation｜三维生成

- Text-to-3D：从文本生成形状、外观或场景。
- Image-to-3D：单图 / 多图三维重建与资产生成。
- 3D Asset Generation：Mesh、Texture、Material、Avatar、Scene Layout。

### 2.4 3D Understanding｜三维理解

- 3D Detection、3D Segmentation、Pose Estimation、Tracking。
- Scene Understanding：室内外场景解析、语义地图、开放词汇 3D 理解。
- Vision-Language-3D：把语言和三维表示对齐，用于检索、问答和规划。

### 2.5 Embodied 3D｜具身与机器人

- 面向机器人操作的三维感知、抓取、场景建模与几何推理。
- 面向导航的 3D occupancy、语义地图、场景图与世界模型。
- 面向仿真的 3D 场景构建、传感器建模与数据合成。

### 2.6 Datasets & Benchmarks｜数据集与评测

- 室内外重建数据集。
- 3D detection / segmentation 基准。
- 具身操作与导航中的 3D 感知基准。
- 大规模 3D 生成与资产评测基准。

## (3) Recommended Starting Points｜推荐起步工具

下面这些项目适合作为 3D 工程与研究的起点：

- [Open3D](https://github.com/isl-org/Open3D): 点云、配准、重建、可视化的通用工具库。
- [PyTorch3D](https://github.com/facebookresearch/pytorch3d): 适合做可微渲染、几何学习和 3D 深度学习实验。
- [COLMAP](https://github.com/colmap/colmap): 经典 SfM / MVS 基础设施，重建方向必备。
- [nerfstudio](https://github.com/nerfstudio-project/nerfstudio): NeRF 研究与实验的高质量工程框架。
- [gaussian-splatting](https://github.com/graphdeco-inria/gaussian-splatting): 3D Gaussian Splatting 官方实现。
- [MMDetection3D](https://github.com/open-mmlab/mmdetection3d): 3D 检测与感知任务的成熟训练框架。
- [Kaolin](https://github.com/NVIDIAGameWorks/kaolin): NVIDIA 的 3D 深度学习工具库，适合生成与几何方向。

## (4) Scope Planning｜后续整理计划

- [x] 初始化仓库首页。
- [x] 补充开源许可证。
- [ ] 增加 3D Vision / Reconstruction / Generation 专题条目。
- [ ] 增加 Datasets / Benchmarks / Surveys 整理。
- [ ] 增加面向 Python 用户的最小实践路线。
- [ ] 整理 `paperlist.md`，形成可持续维护的论文索引。

## (5) Contribution｜贡献方式

欢迎通过以下方式一起维护这个仓库：

- 提交 PR，补充高质量项目、教程、课程、数据集和综述。
- 提交 issue，指出失效链接、分类问题或内容遗漏。
- 如果你维护相关项目，也欢迎把仓库信息补充进来。

建议补充内容时尽量包含：

- 项目链接
- 任务类型
- 关键特点
- 适用场景
- 论文或主页

## (6) License｜许可协议

本仓库采用 [MIT License](./LICENSE)。

如果后续仓库中收录第三方内容、图片或论文摘要，其版权归原作者或原项目所有；本仓库仅负责整理与索引。
