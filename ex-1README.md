# 😎 Awesome Aerial-Ground Person Re-Identification

[![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](#-contributing)
[![License](https://img.shields.io/badge/License-CC0--1.0-lightgrey.svg)](LICENSE)

A curated list of **Aerial-Ground Person Re-Identification (AG-ReID)** papers, datasets, codebases and challenges.  
AG-ReID aims to match pedestrians across **UAV-captured aerial views** and **ground camera views**, facing major challenges such as extreme viewpoint discrepancy, scale/resolution variation, illumination changes and background clutter.

> 🔄 **Last updated:** 2026-01-12 (America/Los_Angeles)

---

## 📖 Table of Contents
- [😎 Awesome Aerial-Ground Person Re-Identification](#-awesome-aerial-ground-person-re-identification)
  - [📖 Table of Contents](#-table-of-contents)
  - [🌟 Spotlight: Our Contributions](#-spotlight-our-contributions)
  - [🧭 Task Overview](#-task-overview)
  - [📝 Papers \& Methods](#-papers--methods)
    - [Image-based AG-ReID](#image-based-ag-reid)
    - [Video-based AG-ReID](#video-based-ag-reid)
    - [Text/Multimodal \& Related Retrieval](#textmultimodal--related-retrieval)
    - [Challenges \& Workshops](#challenges--workshops)
  - [📦 Datasets \& Benchmarks](#-datasets--benchmarks)
  - [🤝 Contributing](#-contributing)
  - [📌 Citation](#-citation)

---

## 🌟 Spotlight: Our Contributions

Selected works from our research group on **cross-view alignment** and **robust representation learning**:

- **[WACVW 2026]** SAS-VPReID: A Scale-Adaptive Framework with Shape Priors for Video-based Person Re-Identification at Extreme Far Distances  [Paper](https://arxiv.org/pdf/2601.05535) · [Code](https://github.com/YangQiWei3/SAS-VPReID)

- **[arXiv 2025]** SD-ReID: View-aware Stable Diffusion for Aerial-Ground Person Re-Identification  [Paper](https://arxiv.org/abs/2504.09549)

- **[arXiv 2025]** LATex: Leveraging Attribute-based Text Knowledge for Aerial-Ground Person Re-Identification  [Paper](https://arxiv.org/abs/2503.23722)

> More coming soon.  
> 📩 Feel free to open an issue / PR to add papers, code or datasets.

---

## 🧭 Task Overview

**Goal:** match the same person across **aerial (drone)** and **ground** cameras.  
**Key difficulties:**
- **Viewpoint gap:** top-down vs horizontal viewpoints
- **Scale gap:** far-distance tiny pedestrians in aerial views
- **Domain gap:** different sensors, backgrounds, lighting
- **Occlusion & clutter:** complex scenes + moving cameras

Typical solution directions:
- Cross-view **feature alignment** (geometry/semantic/part-based)
- **Transformer**-based representation learning
- **CLIP / multimodal** supervision
- **Diffusion / generative priors** for view adaptation
- **Self-/unsupervised** domain adaptation

---

## 📝 Papers & Methods

### Image-based AG-ReID

| Venue          | Year  | Title                                                                                                                | Resources                                                                                                                                                                                                                                                                                                   |
| :------------- | :---: | :------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **AAAI**       | 2026  | Semantic-Driven Progressive Refinement for Aerial-Ground Person ReID: A Challenging Large-Scale                      | [Paper](TBA)                                                                                                                                                                                                                                                                                                |
| **NeurIPS**    | 2025  | GSAlign: Geometric and Semantic Alignment Network for Aerial-Ground Person Re-Identification                         | [Paper](https://openreview.net/attachment?id=bxELEjg3VE&name=pdf) · [Code](https://github.com/stone96123/GSAlign?tab=readme-ov-file)                                                                                                                                                                        |
| **ICCV**       | 2025  | VIF: Bridging the Sky and Ground: Towards View-Invariant Feature Learning for Aerial-Ground Person Re-Identification | [Paper](https://openaccess.thecvf.com/content/ICCV2025/html/Khalid_Bridging_the_Sky_and_Ground_Towards_View-Invariant_Feature_Learning_for_ICCV_2025_paper.html)                                                                                                                                            |
| **arXiv**      | 2025  | SD-ReID: View-aware Stable Diffusion for Aerial-Ground Person Re-Identification                                      | [Paper](https://arxiv.org/abs/2504.09549)                                                                                                                                                                                                                                                                   |
| **arXiv**      | 2025  | LATex: Leveraging Attribute-based Text Knowledge for Aerial-Ground Person Re-Identification                          | [Paper](https://arxiv.org/abs/2503.23722)                                                                                                                                                                                                                                                                   |
| **ICME**       | 2025  | DTST: Dynamic Token Selective Transformer for Aerial-Ground Person Re-Identification                                 | [Paper](https://yuhaiw.github.io/DTS-AGPReID/ICMEYuhai.pdf) · [Code](https://github.com/YuhaiW/reidselecttoken)                                                                                                                                                                                             |
| **CVPR**       | 2025  | SeCap: Self-Calibrating and Adaptive Prompts for Cross-view Person Re-Identification in Aerial-Ground Networks       | [Paper](https://arxiv.org/abs/2503.06965) · [Code](https://github.com/wangshining681/SeCap-AGPReID) · [Dataset](https://pan.baidu.com/share/init?surl=MRrhqoQzwxw7qOx4Lqdl2g) |
| **TOMM**       | 2025  | CVAF: A CLIP-Based View-Consistent Alignment Framework for Aerial-Ground Person Re-Identification                    | [Paper](https://dl.acm.org/doi/pdf/10.1145/3785482)                                                                                                                                                                                                                                                         |
| **ICIG**       | 2025  | Perspective Driven Prototype Alignment for Aerial-Ground Person Re-Identification                                    | [Paper](https://link.springer.com/chapter/10.1007/978-981-95-3393-0_42)                                                                                                                                                                                                                                     |
| **自动化学报** | 2025  | Implicit Decoder Alignment for Aerial-ground Person Re-identification                                                | [Paper](https://www.aas.net.cn/cn/article/doi/10.16383/j.aas.c240705)                                                                                                                                                                                                                                       |
| **CVPR**       | 2024  | VDT: View-decoupled Transformer for Person Re-identification under Aerial-ground Camera Network                      | [Paper](https://arxiv.org/abs/2403.14513) · [Code](https://github.com/LinlyAC/VDT-AGPReID?tab=readme-ov-file) · [Dataset](https://drive.google.com/file/d/1yDjyH0VtW7efxP3vgQjIqTx2oafCB67t/view)                                                                                                           |
| **TITS**       | 2024  | AG-ReID.v2: Bridging Aerial and Ground Views for Person Re-identification                                            | [Paper](https://arxiv.org/abs/2401.02634) · [Code](https://github.com/huynguyen792/AG-ReID.v2) · [Dataset](https://drive.google.com/drive/folders/16r7G_CuUqfWG6_UCT7goIGRMqJird6vK)                                                                                                                        |
| **ICME**       | 2023  | Explain: Aerial-Ground Person Re-ID                                                                                  | [Paper](https://arxiv.org/abs/2303.08597) · [Dataset](https://drive.google.com/file/d/1hzieEPlXfjkN3V3XWqI5rAwpF_sCF1K9/view)                                                                                                                                                                               |
| **ATR**        | 2017  | Person Re-Identification Across Aerial and Ground-Based Cameras by Deep Feature Fusion                               | [Paper](https://publica.fraunhofer.de/bitstreams/ef904224-f31f-484d-b8d2-56695e46779c/download)                                                                                                                                                                                                             |

### Video-based AG-ReID

| Venue     | Year  | Title                                                                                                                         | Resources                                                                                                                                                                  |
| :-------- | :---: | :---------------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **WACVW** | 2026  | SAS-VPReID: A Scale-Adaptive Framework with Shape Priors for Video-based Person Re-Identification at Extreme Far Distances    | [Paper](https://arxiv.org/pdf/2601.05535) · [Code](https://github.com/YangQiWei3/SAS-VPReID)                                                                               |
| **CVPR**  | 2025  | AG-VPReID: A Challenging Large-Scale Benchmark for Aerial-Ground Video-based Person Re-Identification                         | [Paper](https://arxiv.org/abs/2503.08121) · [Dataset](https://drive.google.com/drive/folders/1wtdhKzK9Fbj7xkGAM84KNJ1uYCxSMHdj)                                            |
| **IJCB**  | 2025  | VM-TAPS: View-specific Memory with Temporal and Scale Awareness Framework for Video-based Cross-View Person Re-Identification | [Paper](https://www.di.ubi.pt/%7Ehugomcp/doc/rashid_ijcb2025.pdf) · [Code](https://github.com/MdRashidunnabi/VM-TAPS)                                                      |
| **TBIOM** | 2025  | DetReIDX: A Stress-Test Dataset for Real-World UAV-Based Person Recognition                                                   | [Paper](https://arxiv.org/pdf/2505.04793) · [Dataset](https://github.com/kailashhambarde/DetReIDX/tree/main)                                                               |
| **TBIOM** | 2025  | Seeing Across Time and Views: Multi-Temporal Cross-View Learning for Robust Video Person Re-Identification                    | [Paper](https://arxiv.org/pdf/2511.02564) · [Code](https://github.com/MdRashidunnabi/MTF-CVReID)                                                                           |
| **ECCV**  | 2024  | Cross-Platform Video Person ReID: A New Benchmark Dataset and Adaptation Approach                                             | [Paper](https://arxiv.org/abs/2408.07500) · [Code](https://github.com/FHR-L/VSLA-CLIP) · [Dataset](https://drive.google.com/file/d/1vPS-Xc1gBNc8Q40QZ0FaUWeYRkKsndeL/view) |

---

### Text/Multimodal & Related Retrieval

| Venue      | Year  | Title                                                                                                                   | Resources                                                                                                                                                                                     |
| :--------- | :---: | :---------------------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **AAAI**   | 2026  | Text-based Aerial-Ground Person Retrieval                                                                               | [Paper](https://arxiv.org/pdf/2511.08369) · [Code](https://github.com/Flame-Chasers/TAG-PR) · [Dataset](https://pan.quark.cn/s/dcddfa17cb7f?pwd=8pE6#/list/share)                             |
| **arXiv**  | 2025  | Multi-modal Multi-platform Person Re-Identification: Benchmark and Method                                               | [Paper](https://arxiv.org/pdf/2503.17096) · [Code](https://github.com/MP-ReID/mp-reid) · [Dataset](https://drive.google.com/file/d/1hImLEMcsBB2kNV4McGyksVAumLjZQoUU/view)                    |
| **TCSVT**  | 2025  | AEA-FIRM: Adaptive Elastic Alignment with Fine-Grained Representation Mining for Text-based Aerial Pedestrian Retrieval | [Paper](https://ieeexplore.ieee.org/document/11072214) · [Code](https://github.com/xbdxwyh/AEA-FIRM-main) · [Dataset](https://drive.google.com/file/d/1YYIpBDoJzTIwYRlpWUqEHmpo5GK05S_W/view) |
| **SPL**    | 2025  | Omni-Directional View Person Re-Identification Through 3D Human Reconstruction                                          | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10839551)                                                                                                                    |
| **IJCB**   | 2025  | AG-VPReID.VIR: Bridging Aerial and Ground Platforms for Video-based Visible-Infrared Person Re-ID                       | [Paper](https://arxiv.org/abs/2507.17995) · [Dataset](https://drive.google.com/drive/folders/1Iy814PqWjwIZcv6CZpieFju-Dop9Y2G7)                                                               |
| **ACM MM** | 2024  | AerialGait: Bridging Aerial and Ground Views for Gait Recognition                                                       | [Paper](https://dl.acm.org/doi/pdf/10.1145/3664647.3681002)                                                                                                                                   |

> If you also want **Vehicle cross-view ReID** in this repo, consider adding a dedicated section.  
> Currently found in the earlier list:
> - **SENSORS 2025** CVNet (Vehicle ReID) — [Paper](https://www.mdpi.com/1424-8220/25/9/2809)  
> - **RS 2025** AGID (Vehicle ReID dataset) — [Paper](https://www.mdpi.com/2072-4292/17/15/2653)

---

### Challenges & Workshops

| Venue    | Year  | Title                                                                                     | Resources                                                                            |
| :------- | :---: | :---------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------- |
| **WACV** | 2026  | VReID-XFD: Video-based Person Re-identification at Extreme Far Distance Challenge Results | [Paper](https://arxiv.org/pdf/2601.01312v1)                                          |
| **IJCB** | 2025  | AG-VPReID 2025: Aerial-Ground Video-based Person Re-identification Challenge Results      | [Paper](https://arxiv.org/pdf/2506.22843)                                            |
| **IJCB** | 2023  | AG-ReID 2023: Aerial-Ground Person Re-identification Challenge Results                    | [Paper](https://cvlab.cse.msu.edu/pdfs/IJCB_AG_ReID2023_Challenge_Summary_Paper.pdf) |

---

## 📦 Datasets & Benchmarks

A quick entry point for datasets mentioned above:

- **AG-ReID (ICME 2023)** — [Dataset](https://drive.google.com/file/d/1hzieEPlXfjkN3V3XWqI5rAwpF_sCF1K9/view)
- **AG-ReID.v2 (TITS 2024)** — [Dataset](https://drive.google.com/drive/folders/16r7G_CuUqfWG6_UCT7goIGRMqJird6vK)
- **CARGO (CVPR 2024)** — [Dataset](https://drive.google.com/file/d/1yDjyH0VtW7efxP3vgQjIqTx2oafCB67t/view)
- **LAGPeR / G2APS-ReID(CVPR 2025)** — [Dataset](https://pan.baidu.com/share/init?surl=MRrhqoQzwxw7qOx4Lqdl2g) · [Usage Restriction](https://wangshining681.github.io/laper-page/Restrictions%20for%20The%20Use%20of%20LAGPeR%20Dataset.pdf)
- **AG-VPReID (CVPR 2025)** — [Dataset](https://drive.google.com/drive/folders/1wtdhKzK9Fbj7xkGAM84KNJ1uYCxSMHdj)
- **DetReIDX (TBIOM 2025)** — [Dataset](https://github.com/kailashhambarde/DetReIDX/tree/main)

> Suggestion: later you can add **stats** (IDs / images / cameras / splits) and an **evaluation protocol** column (mAP, Rank-1, etc.).

---

## 🤝 Contributing

PRs are welcome! Please follow the format below:

1. Add your paper in the correct section (Image / Video / Text / Challenge / Dataset).
2. Keep the table sorted by **Year (desc)**, then **Venue**.
3. Use consistent formatting:
   - Venue in **bold**
   - Year as a number
   - Resources order: `Paper · Code · Dataset · Project Page` (if available)

**Template**
- **[VENUE YEAR]** Paper Title  
  [Paper](link) · [Code](link) · [Dataset](link) · [Project](link)

---

## 📌 Citation

If you find this repository helpful, please consider citing / starring it ⭐

```bibtex
@misc{awesome_agpreid,
  title        = {Awesome Aerial-Ground Person Re-Identification},
  author       = {Yang, Qiwei, Zhang, Pingping and Gong, Zijing},
  howpublished = {\url{https://github.com/<your_repo>/awesome-aerial-ground-person-reid}},
  year         = {2026},
  note         = {A curated list of papers, datasets, and resources for AGPReID.}
}