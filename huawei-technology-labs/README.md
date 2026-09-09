# Huawei Technology Labs — Healthcare AI

This folder contains the **actual Huawei-technology implementation layer**
for the AI Explorer Hub / HCIA-AI Academy competition project.

It is intentionally separated from the older 18-lab
**Huawei-Inspired healthcare adaptation**, which is mainly PyTorch/Colab.

## Six-lab pathway

| Lab | Technology | Main learning goal |
|---|---|---|
| 1 | MindSpore | Tensors, datasets, model, loss, optimiser, training |
| 2 | MindSpore | Medical-image classification and healthcare metrics |
| 3 | MindSpore | 2D segmentation and Dice evaluation |
| 4 | Huawei Cloud ModelArts + MindSpore | Reproducible cloud notebook workflow |
| 5 | MindSpore + CANN + Ascend | Understand and verify acceleration environment |
| 6 | MindSpore + ModelArts concept | Responsible deployment, model card and prohibited use |

## Evidence status

- Labs 1–3 contain genuine MindSpore implementation code.
- Lab 4 is **ModelArts-ready/guided** until actual ModelArts execution is documented.
- Lab 5 is **hardware/cloud Ascend dependent**. Do not claim actual Ascend execution
  until a configured Ascend+CANN environment successfully runs the model.
- Lab 6 creates responsible deployment documentation and deliberately does not
  claim clinical or ModelArts deployment.

## Safety

**Educational prototype — not for clinical diagnosis or treatment.**

Do not upload identifiable patient information. Benchmark or synthetic
performance does not establish clinical validity.

## Competition pathway

**MindSpore Foundations → Medical Classification → Segmentation → ModelArts Cloud
→ Ascend/CANN → Responsible Deployment**
