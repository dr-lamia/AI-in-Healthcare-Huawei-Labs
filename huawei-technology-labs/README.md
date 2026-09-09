# Huawei Technology Labs — Healthcare AI

This folder contains the **actual Huawei-technology implementation layer** for the AI Explorer Hub / HCIA-AI Academy competition project.

It is intentionally separated from the older 18-lab **Huawei-Inspired healthcare adaptation**, which is mainly PyTorch/Colab.

## Six-lab pathway

| Lab | Technology | Main learning goal | Notebook | Colab |
|---|---|---|---|---|
| 1 | MindSpore | Tensors, datasets, model, loss, optimiser, training | [View](./Huawei_Tech_Lab_01_MindSpore_Fundamentals.ipynb) | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/huawei-technology-labs/Huawei_Tech_Lab_01_MindSpore_Fundamentals.ipynb) |
| 2 | MindSpore | Medical-image classification and healthcare metrics | [View](./Huawei_Tech_Lab_02_MindSpore_Medical_Image_Classification.ipynb) | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/huawei-technology-labs/Huawei_Tech_Lab_02_MindSpore_Medical_Image_Classification.ipynb) |
| 3 | MindSpore | 2D segmentation and Dice evaluation | [View](./Huawei_Tech_Lab_03_MindSpore_2D_Segmentation.ipynb) | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/huawei-technology-labs/Huawei_Tech_Lab_03_MindSpore_2D_Segmentation.ipynb) |
| 4 | Huawei Cloud ModelArts + MindSpore | Reproducible cloud notebook workflow | [View](./Huawei_Tech_Lab_04_ModelArts_Cloud_Workflow.ipynb) | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/huawei-technology-labs/Huawei_Tech_Lab_04_ModelArts_Cloud_Workflow.ipynb) |
| 5 | MindSpore + CANN + Ascend | Understand and verify acceleration environment | [View](./Huawei_Tech_Lab_05_Ascend_CANN_Acceleration.ipynb) | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/huawei-technology-labs/Huawei_Tech_Lab_05_Ascend_CANN_Acceleration.ipynb) |
| 6 | MindSpore + ModelArts concept | Responsible deployment, model card and prohibited use | [View](./Huawei_Tech_Lab_06_Responsible_Deployment_Model_Card.ipynb) | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/huawei-technology-labs/Huawei_Tech_Lab_06_Responsible_Deployment_Model_Card.ipynb) |

> Colab is provided as a convenient notebook viewer/runtime. MindSpore installation and hardware support depend on the runtime. ModelArts and Ascend-specific evidence must be produced in the corresponding Huawei environment.

## Evidence status

- **Labs 1–3:** contain genuine MindSpore implementation code.
- **Lab 4:** is **ModelArts-ready/guided** until actual ModelArts execution is documented.
- **Lab 5:** is **hardware/cloud Ascend dependent**. Do not claim actual Ascend execution until a configured Ascend + CANN environment successfully runs the model.
- **Lab 6:** creates responsible deployment documentation and deliberately does not claim clinical or ModelArts deployment.

## Huawei technology pathway

**MindSpore Foundations → Medical Classification → Segmentation → ModelArts Cloud → Ascend/CANN → Responsible Deployment**

## Relationship to the 18 Huawei-Inspired labs

The repository therefore contains two clearly separated teaching layers:

1. **18 Huawei-Inspired healthcare labs** — broad healthcare AI pedagogy and Colab-based practice, largely using PyTorch and common open-source tools.
2. **6 Huawei Technology Labs** — the competition-focused implementation layer using MindSpore, with guided ModelArts and Ascend/CANN activities.

This distinction is deliberate and should be preserved in competition materials.

## Safety and academic integrity

**Educational prototype — not for clinical diagnosis or treatment.**

Do not upload identifiable patient information. Benchmark or synthetic performance does not establish clinical validity. Do not state that ModelArts, CANN, or Ascend were executed by learners until actual run evidence exists.
