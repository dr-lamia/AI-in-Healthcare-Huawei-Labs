# AI in Healthcare — Huawei-Inspired Lab Series

A healthcare-focused, simplified laboratory series adapted from the **Huawei HCIA-AI V4.0 Lab Guide** and expanded with additional medical-AI labs for healthcare providers, educators, and students.

> **Educational use only.** These notebooks are teaching demonstrations. They are not clinical decision-support systems and must not be used for diagnosis, prognosis, treatment, triage, or patient management.

## Course structure

| Lab | Medical problem / focus | AI model | Dataset / data type | Open in Colab |
|---|---|---|---|---|
| 01 | Predict a continuous healthcare outcome | Linear Regression | Healthcare tabular data | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_01_Linear_Regression.ipynb) |
| 02 | Understand how a model learns | Gradient Descent + Linear Regression | Healthcare numeric data | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_02_Gradient_Descent.ipynb) |
| 03 | Binary disease classification | Logistic Regression | Binary healthcare data | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_03_Logistic_Regression.ipynb) |
| 04 | Transparent rule-based classification | Decision Tree | Healthcare classification data | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_04_Decision_Tree.ipynb) |
| 05 | Discover patient groups without labels | K-Means | Unlabelled healthcare data | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_05_KMeans_Clustering.ipynb) |
| 06 | Learn deep-learning foundations | PyTorch Basics | Healthcare tensors/tabular data | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_06_PyTorch_Basics.ipynb) |
| 07 | Pneumonia image classification | LeNet CNN | PneumoniaMNIST | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_07_LeNet_PneumoniaMNIST.ipynb) |
| 08 | Skin-lesion image classification | ResNet-50 Transfer Learning | DermaMNIST | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_08_ResNet50_DermaMNIST.ipynb) |
| 09 | Healthcare text classification | TextCNN | Drug reviews / healthcare text | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_09_TextCNN_Drug_Reviews.ipynb) |
| 10 | Build a neural network from scratch | Fully Connected Network | Healthcare tabular data | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_10_Fully_Connected_Network.ipynb) |
| 11 | Run a compact LLM online with low RAM | llama.cpp + quantised LLM | Prompt-based workflow | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_11_RAM_Safe_Online_LLM_CLI.ipynb) |
| 12 | Build a web/API LLM demo | LLM API + Gradio | Prompt-based workflow | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_12_Online_LLM_API_Gradio.ipynb) |
| 13 | Understand 3D medical AI tasks | 3D CNN + Detector + 3D U-Net | Synthetic 3D medical volumes | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_13_3D_Classification_Detection_Segmentation.ipynb) |
| 14 | Compare model depth and efficiency | ResNet-18/34/50 | PneumoniaMNIST | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_14_ResNet18_34_50_Comparison.ipynb) |
| 15 | Study training design choices | ReLU/Sigmoid + He/Xavier + L2 | Breast Cancer Wisconsin | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_15_Activation_Initialisation_L2.ipynb) |
| 16 | Understand what is inside ResNet | Custom BasicBlock + BottleNeck ResNet | PathMNIST | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_16_ResNet_From_Scratch.ipynb) |
| 17 | Compare, explain, select, and deploy models | Logistic + Tree + MLP | Breast Cancer Wisconsin | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_17_Integrated_Capstone.ipynb) |
| 18 | Validate probabilities and thresholds responsibly | Calibrated Logistic Regression | Breast Cancer Wisconsin | [Open](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_18_Responsible_Model_Validation.ipynb) |

## Learning pathway

1. **Labs 1–5:** Core machine learning for healthcare data.
2. **Lab 6:** PyTorch foundations.
3. **Labs 7–10:** Healthcare deep learning for image, text, and tabular data.
4. **Labs 11–12:** LLM inference and web deployment.
5. **Labs 13–16:** 3D medical imaging and deeper architecture understanding.
6. **Labs 17–18:** Capstone integration and responsible validation.

## Huawei source coverage and extensions

The sequence preserves the principal ideas from the Huawei HCIA-AI V4.0 laboratory material while replacing or adapting examples for healthcare education. **Lab 13, Lab 17, and Lab 18 are original healthcare extensions**. Labs 14–16 expand architectural and training concepts introduced by the Huawei material.

This repository is an independent educational adaptation and does not imply Huawei endorsement.

## Ready-to-run backup on Google Drive

All 18 notebooks are also available in the course Google Drive folder:

https://drive.google.com/drive/folders/1CJgBd9inFLvnVzGmxpkIJfGkh0O2I-e7

## How to run a lab

1. Click the **Open in Colab** link in the table.
2. Choose a GPU runtime when the lab recommends one.
3. Run cells from top to bottom.
4. Read the medical problem and model explanation before running the code.
5. Record results and interpret them as an educational exercise.
6. Do not upload identifiable patient information.

## Clinical safety

These notebooks are not validated medical devices. Real clinical AI requires representative patient-level data, leakage prevention, external validation, calibration, subgroup assessment, privacy protection, security, governance, professional oversight, ethics approval where applicable, and appropriate regulatory evaluation.
