# 3D Spleen CT Segmentation using MONAI & PyTorch

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-2.0%2B-ee4c2c)
![MONAI](https://img.shields.io/badge/MONAI-Medical%20AI-brightgreen)
![License](https://img.shields.io/badge/License-MIT-green)

An end-to-end Deep Learning pipeline for 3D volumetric spleen segmentation from abdominal CT scans using **MONAI** and **PyTorch**, engineered with a focus on **memory optimization** and **Edge/Embedded AI deployment**.

Project Overview
Volumetric medical data (3D NIfTI scans) typically require substantial computational resources and high RAM overhead, leading to runtime crashes in memory-constrained environments.

This repository demonstrates a hardware-aware software design approach:

Memory-Efficient Data Handling: Streamlined 3D volume loading to prevent RAM bottlenecks.

3D Volumetric Processing: Precise extraction and slice-wise visualization along the depth axis.

Edge AI Preparedness: Pipeline structured for seamless model quantization and ONNX export for real-time inference on embedded devices.

##Tech Stack & Tools
Framework: PyTorch & MONAI (Medical Open Network for AI)

Medical Data Handling: Nibabel, NIfTI (.nii, .nii.gz)

Dataset: MSD (Medical Segmentation Decathlon) - Task09 Spleen

Visualization: Matplotlib

Target Platforms: Edge AI Hardware / Embedded Systems

Repository Structure
Plaintext
├── 3D_Spleen_Segmentation_MONAI.ipynb   # Main Jupyter Notebook
├── README.md                             # Project Documentation
└── data/                                 # Dataset Directory (Auto-downloaded)
 Getting Started
Prerequisites
Install the required medical imaging and deep learning packages:

Bash
pip install monai gradio torch nibabel matplotlib tqdm
Running the Notebook
Open 3D_Spleen_Segmentation_MONAI.ipynb in Google Colab or local Jupyter environment.

Execute the setup cells to auto-download the Decathlon Task09 Spleen dataset.

Run the slice extraction module to visualize 3D CT slices alongside segmentation masks.

 Engineering & Optimization Highlights
Streaming Data Loaders: Avoids loading full 3D scans simultaneously into RAM.

Format Flexibility: Native support for compressed NIfTI files (.nii.gz) without manual extraction.

Hardware Co-Design Focus: Built with future deployment on embedded AI accelerators (e.g., Jetson, Microcontrollers) in mind.

## License
Distributed under the MIT License. See LICENSE for more information.
## Sample Visualisation

<img width="836" height="418" alt="image" src="https://github.com/user-attachments/assets/2a742700-1cc0-42f4-ba8b-9fe62923ae5c" />
<img width="404" height="427" alt="image" src="https://github.com/user-attachments/assets/f3bb55a2-a987-4416-9199-d7ce4de688ce" />
