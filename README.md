# LiDGS: An Efficient 3D Reconstruction Framework Integrating LiDAR Point Clouds and Multi-view Images for Enhanced Geometric Fidelity
This repository represents the official implementation of the paper titled "**LiDGS: An efficient 3D reconstruction framework integrating lidar point clouds and multi-view images for enhanced geometric fidelity**".

[![Project](https://img.shields.io/badge/Project-Website-blue)](https://github.com/SongJiang-WHU/LiDGS)
[![Paper](https://img.shields.io/badge/Paper-PDF-red)](https://www.sciencedirect.com/science/article/pii/S1569843225003772)
[![License](https://img.shields.io/badge/License-Apache--2.0-green)](LICENSE)

[**Li Yan**]()*<sup>1,2</sup> · [**Jiang Song**]()<sup>1,*</sup> · [**Hong Xie**]()<sup>1,2</sup> · [**Pengcheng Wei**]()<sup>1</sup> · [**Gang Li**]()<sup>1</sup> · [**Longze Zhu**]()<sup>1</sup> · [**Zhongli Fan**]()<sup>3</sup> · [**Shucheng Gong**]()<sup>1</sup>

<sup>1</sup>School of Geodesy and Geomatics, Wuhan University, 129 Luoyu Rd, Wuhan, 430079, China  
<sup>2</sup>Hubei Luojia Laboratory, 129 Luoyu Rd, Wuhan, 430079, China  
<sup>3</sup>State Key Laboratory of Information Engineering in Surveying, Mapping and Remote Sensing, Wuhan University, Wuhan 430079, China

*Corresponding author

---

We present **LiDGS**, a novel 3D reconstruction approach within the 3D Gaussian Splatting (3DGS) framework that integrates LiDAR point clouds and multi-view images. Our method achieves high-fidelity 3D scene reconstruction by introducing high-precision geometric a priori information and multiple geometric constraints from LiDAR point clouds, while guaranteeing efficient and accurate scene rendering.

Our key contributions include:
- **Adaptive Checkerboard Sampling Strategy**: Multi-hypothesis joint view selection (ACMP) for whole-image depth propagation, generating high-precision dense depth maps
- **Adaptive Gaussian Densification**: Effective guidance of geometric structure through geometric anchors with adaptive adjustment of Gaussian parameters
- **Depth Regularization**: Correction of depth estimation for each Gaussian to ensure consistency across different viewpoints

## 🔥 News
- **2024.12**: LiDGS paper accepted by *International Journal of Applied Earth Observation and Geoinformation*
- **2024.11**: Code repository created and initial implementation released

## 🚀 Method Overview

![LiDGS Method Overview](https://github.com/user-attachments/assets/a3380384-cd1d-4bfb-b02a-6ac219204b66)

LiDGS addresses the limitation of existing NeRF and 3DGS methods regarding geometric structure fidelity by:

1. **High-precision Depth Prior**: Leveraging LiDAR point clouds to provide continuous and accurate depth constraints
2. **Geometric Anchors**: Guiding 3D scene geometric structure through adaptive densification
3. **Multi-view Consistency**: Ensuring depth information consistency across different viewpoints

## 📊 Results

[![demo](https://github.com/user-attachments/assets/video_thumbnail.png)](https://github.com/user-attachments/assets/5db2cd1c-e193-4003-854b-58cb3f192a2c)

Our method achieves superior performance in both novel view synthesis and 3D reconstruction tasks:

| Method | PSNR ↑ | SSIM ↑ | LPIPS ↓ | Depth RMSE ↓ |
|--------|--------|--------|---------|---------------|
| DSNeRF | 21.62  | 0.571  | 0.645   | 0.529        |
| LiDeNeRF | 22.28  | 0.674  | 0.346   | 0.627        |
| 3DGS   | 21.83  | 0.797  | 0.255   | 0.305        |
| **Ours (LiDGS)** | **23.42** | **0.834** | **0.217** | **0.272** |

## 📄 Citation

If you find our work useful, please cite:

```bibtex
@article{yan2025lidgs,
  title={LiDGS: An efficient 3D reconstruction framework integrating lidar point clouds and multi-view images for enhanced geometric fidelity},
  author={Yan, Li and Song, Jiang and Xie, Hong and Wei, Pengcheng and Li, Gang and Zhu, Longze and Fan, Zhongli and Gong, Shucheng},
  journal={International Journal of Applied Earth Observation and Geoinformation},
  volume={142},
  pages={104730},
  year={2025},
  publisher={Elsevier}
}
```

## 🤝 Contributing

We welcome contributions! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## 📞 Contact

For questions and discussions:
- **Jiang Song**: [songjiang@whu.edu.cn](mailto:songjiang@whu.edu.cn)
- **Li Yan**: [liyan@whu.edu.cn](mailto:liyan@whu.edu.cn)

## 📜 License

This project is licensed under the Apache-2.0 License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgements

We thank the following projects that made this work possible:
- [3D Gaussian Splatting](https://github.com/graphdeco-inria/gaussian-splatting)
- [NeRF](https://github.com/bmild/nerf)
- [COLMAP](https://github.com/colmap/colmap)

---

**Keywords**: 3D Reconstruction · 3D Gaussian Splatting · Novel View Synthesis · Depth Prior · Geometric Anchors · Depth Regularization

## 🙏 Acknowledgements

We thank the following projects that made this work possible:
- [3D Gaussian Splatting](https://github.com/graphdeco-inria/gaussian-splatting)
- [NeRF](https://github.com/bmild/nerf)
- [COLMAP](https://github.com/colmap/colmap)

---

**Keywords**: 3D Reconstruction · 3D Gaussian Splatting · Novel View Synthesis · Depth Prior · Geometric Anchors · Depth Regularization
