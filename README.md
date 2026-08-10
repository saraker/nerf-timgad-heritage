# nerf-timgad-heritage
# NeRF-Based 3D Reconstruction of Timgad Archaeological Heritage (Algeria)

This repository documents the application of Neural Radiance Fields (NeRF), via the Nerfstudio framework, to the digital reconstruction of Roman archaeological monuments at Timgad, Algeria — specifically the Arch of Trajan.

---

## 📦 Dataset Structure

The dataset was processed using **COLMAP** and includes camera poses, sparse point clouds, and NeRF-compatible transformations:

```text
Dataset/
├── colmap/          # COLMAP sparse reconstruction & camera poses
├── images/          # High-resolution input images
└── transforms.json  # Camera intrinsics & extrinsics (NeRF format)
```

## 📦 Large Files (Google Drive)

Due to file size constraints, the following are hosted externally:

| Name | Description |
|---|---|
| Input Dataset | Video-extracted frames (377 images, Arch of Trajan) |
| Rendered Outputs | NeRF-synthesized novel views and flythrough videos |
| Timgad Scene | [Timgad](https://drive.google.com/file/d/1r2gY4bcNHx7W10uolMZHeWXb6xhhs19C/view?usp=sharing) |

## 🔧 Methodology

- **Framework:** Nerfstudio (nerfacto model)
- **Pose Estimation:** COLMAP (Structure-from-Motion)
- **Hardware:** NVIDIA RTX 3060 (12GB VRAM)
- **Training:** 30,000 iterations, Adam optimizer


