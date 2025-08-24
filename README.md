# Amodal Mask Generation – LLNL Data Science Challenge 2025

This repository contains work from the **Lawrence Livermore National Laboratory (LLNL) Data Science Challenge 2025**, focused on enabling models to “see the unseen” through **amodal segmentation** and object permanence.

## Overview
We explore computer vision methods that predict occluded portions of objects in synthetic and real scenes. Using the **MOVi-MC-AC dataset**, the challenge tasks are:

- **Task 1.1:** (Image) Modal Mask → Amodal Mask  
- **Task 1.2:** (Image) Modal RGB → Amodal RGB  
- **Task 2.1:** (Video) Modal Mask → Amodal Mask  
- **Task 2.2:** (Video) Modal RGB → Amodal RGB  
- **Transfer Test:** Apply models to the Robotics Pick & Place dataset  
- **Bonus Tasks:** SAM2 Mask Creation, Object Re-Identification

## Models
- **SimpleConv2D baseline** – CNN predicting object masks from RGB scenes  
- **U-Net** – stronger segmentation backbone for modal→amodal mask prediction  
- **ConvLSTM** – spatiotemporal model for video-based tasks  

## Dataset
- **MOVi-MC-AC**: 3D synthetic dataset with object occlusions (RGB, depth, modal & amodal masks)  
- **Robotics Pick & Place**: Transfer test dataset for applying trained models  

Data includes:
- Scene-level RGB, depth, and segmentation masks (modal only)  
- Object-centric RGB, depth, and amodal masks  

⚠️ Note: datasets are **not stored in this repo**. Please download separately.

## Getting Started
1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
