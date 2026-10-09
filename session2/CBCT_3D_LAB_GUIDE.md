# Session 2 Advanced Lab — 3D CBCT for Dental AI

## Purpose

A compact original training module that extends the Session 2 2D computer-vision lab into **3D dental CBCT segmentation**.

This module was designed independently for the Dental AI workshop. It does **not** copy code, notebooks, slides, or datasets from the KnightsLab EMRA Workshop. The external repository was used only as a high-level example of how a medical-imaging workshop can progress from data understanding to model training.

## Recommended placement in the 2-hour Session 2

Keep the existing implant-recognition / Landing AI lab as the core activity.

Use this as a **25–30 minute advanced CBCT track**:

| Time | Activity |
|---|---|
| 0–5 min | 2D image vs 3D volume, voxels, spacing, planes |
| 5–12 min | 3D Slicer: import CBCT, Segment Editor, create one segment |
| 12–20 min | Colab: inspect synthetic 3D volume, geometry, patient-level split |
| 20–27 min | Tiny MONAI 3D U-Net training + Dice + visual QC |
| 27–30 min | Leakage, external validation, 2D vs 3D comparison |

For a longer workshop, expand to 45–60 minutes.

## Learning outcomes

Participants will be able to:

- distinguish 2D dental images from 3D CBCT volumes;
- explain voxel spacing and volume geometry;
- annotate a structure in 3D Slicer;
- export image + label volumes while preserving geometry;
- explain patient-level splitting;
- understand patch-based 3D training;
- run a small 3D U-Net demonstration;
- interpret Dice and inspect segmentation errors;
- explain why internal performance does not equal clinical validation.

## Hands-on architecture

### Track A — Annotation in 3D Slicer

1. Load a de-identified CBCT DICOM series.
2. Open **Segment Editor**.
3. Create named segments.
4. Use Paint / Threshold / Grow from Seeds / Fill Between Slices as appropriate.
5. Review axial, coronal, sagittal, and 3D views.
6. Perform expert QC.
7. Export volume + segmentation in NIfTI or NRRD.

### Track B — Colab

Open:

https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Dental_Workshop_Session_2_CBCT_RealDrive_Simple.ipynb

The notebook runs without patient data by generating a small synthetic CBCT-like dataset. It teaches the mechanics of:

**volume → metadata → masks → patient split → 3D patches → 3D U-Net → Dice → visual QC**

### Track C — Optional real dataset

For research after the workshop, participants may explore a properly licensed dental CBCT dataset such as optional external 3D dental dataset from the official source:



The official dataset requires registration/download. Do not redistribute it inside the workshop repository.

## Core safety messages

- A CBCT is not a collection of independent 2D images.
- Never split slices from the same patient across train/test.
- Image and segmentation masks must remain spatially aligned.
- CBCT intensities are scanner-dependent and are not universally equivalent to standard CT HU values.
- Synthetic data are useful for teaching pipelines, not for clinical validation.
- High Dice on an internal dataset does not establish clinical usefulness.
- Real deployment requires external validation, expert review, bias/generalizability assessment, and governance.

## Optional advanced extension

Introduce MONAI Label only as an AI-assisted annotation concept:

**CBCT → AI suggestion → expert correction → improved label**

Avoid installing/configuring a full server during the 2-hour core workshop unless the environment is prepared in advance.

## Tools

- 3D Slicer: https://www.slicer.org/
- MONAI: https://monai.io/
- MONAI Label: https://github.com/Project-MONAI/MONAILabel
- optional external 3D dental dataset: 


## Course dataset copy

The workshop notebook uses the isolated course dataset folder:

https://drive.google.com/drive/folders/1uZuAxSDNOgDEVt3NFVWhfw9ISwlQudup

This folder contains only de-identified teaching case pairs named `Case_001` through `Case_009`, each with `image.nii.gz` and `label.nii.gz`. It is separate from the original research project folder.
