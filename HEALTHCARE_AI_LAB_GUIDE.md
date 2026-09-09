# AI in Healthcare — Huawei-Inspired Laboratory Guide

**Prepared for Dr. Lamiaa ElFadaly**  
**18 hands-on healthcare AI laboratories | Beginner-friendly | Educational use only**

> **Educational use only — not for clinical diagnosis, treatment, triage, prognosis, or patient management.** The labs are teaching demonstrations and do not represent validated medical devices.

## Teaching principle

**Healthcare problem first. AI model second.**

The learning journey is designed for healthcare providers, educators, medical and dental students, and other health-science learners who may have limited programming experience. Each lab connects a healthcare problem to the data type, AI model, evaluation metrics, interpretation, and responsible-use limitations.

## Learning journey

**Understand → Build → Evaluate → Validate → Apply Responsibly**

### Foundation — Labs 1–5

| Lab | Healthcare problem / focus | Model | Run |
|---|---|---|---|
| 1 | Predict a continuous healthcare outcome | Linear Regression | [Open in Colab](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_01_Linear_Regression.ipynb) |
| 2 | Understand how a model learns step by step | Gradient Descent + Linear Regression | [Open in Colab](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_02_Gradient_Descent.ipynb) |
| 3 | Binary disease classification | Logistic Regression | [Open in Colab](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_03_Logistic_Regression.ipynb) |
| 4 | Transparent rule-based clinical decisions | Decision Tree | [Open in Colab](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_04_Decision_Tree.ipynb) |
| 5 | Discover patient groups without labels | K-Means Clustering | [Open in Colab](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_05_KMeans_Clustering.ipynb) |

### Deep Learning — Labs 6–10

| Lab | Healthcare problem / focus | Model | Run |
|---|---|---|---|
| 6 | Learn deep-learning foundations | PyTorch Basics | [Open in Colab](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_06_PyTorch_Basics.ipynb) |
| 7 | Pneumonia image classification | LeNet CNN / PneumoniaMNIST | [Open in Colab](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_07_LeNet_PneumoniaMNIST.ipynb) |
| 8 | Skin-lesion image classification | ResNet-50 Transfer Learning / DermaMNIST | [Open in Colab](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_08_ResNet50_DermaMNIST.ipynb) |
| 9 | Healthcare text classification | TextCNN | [Open in Colab](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_09_TextCNN_Drug_Reviews.ipynb) |
| 10 | Build a neural network from scratch | Fully Connected Network | [Open in Colab](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_10_Fully_Connected_Network.ipynb) |

### LLMs — Labs 11–12

| Lab | Healthcare problem / focus | Model / workflow | Run |
|---|---|---|---|
| 11 | Run a compact LLM online with low RAM | llama.cpp + quantised LLM | [Open in Colab](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_11_RAM_Safe_Online_LLM_CLI.ipynb) |
| 12 | Build a web/API LLM demonstration | LLM API + Gradio | [Open in Colab](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_12_Online_LLM_API_Gradio.ipynb) |

### Advanced Imaging and Architectures — Labs 13–16

| Lab | Healthcare problem / focus | Model | Run |
|---|---|---|---|
| 13 | Understand 3D medical AI tasks | 3D CNN + detector + 3D U-Net | [Open in Colab](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_13_3D_Classification_Detection_Segmentation.ipynb) |
| 14 | Compare model depth and efficiency | ResNet-18/34/50 | [Open in Colab](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_14_ResNet18_34_50_Comparison.ipynb) |
| 15 | Study training design choices | ReLU/Sigmoid + He/Xavier + L2 | [Open in Colab](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_15_Activation_Initialisation_L2.ipynb) |
| 16 | Understand what is inside ResNet | Custom BasicBlock + BottleNeck ResNet | [Open in Colab](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_16_ResNet_From_Scratch.ipynb) |

### Capstone and Responsible AI — Labs 17–18

| Lab | Healthcare problem / focus | Model / workflow | Run |
|---|---|---|---|
| 17 | Compare, explain, select, and deploy models | Logistic Regression + Decision Tree + MLP | [Open in Colab](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_17_Integrated_Capstone.ipynb) |
| 18 | Validate probabilities and thresholds responsibly | Calibrated Logistic Regression | [Open in Colab](https://colab.research.google.com/github/dr-lamia/AI-in-Healthcare-Huawei-Labs/blob/main/notebooks/Lab_18_Responsible_Model_Validation.ipynb) |

## What learners should ask in every lab

1. **Clinical question** — What decision or prediction matters?
2. **Healthcare data** — Are the inputs numbers, images, text, 3D volumes, or prompts?
3. **AI model** — What is the simplest appropriate model for the task?
4. **Evaluation** — Which metrics reflect the important healthcare errors?
5. **Validation** — Are calibration, uncertainty, bias, and dataset shift considered?
6. **Safe use** — What limitations must be stated before any real-world deployment?

## Classification, detection, and segmentation

- **Classification:** What is present? → one label or probability.
- **Detection:** Where is it? → bounding box plus confidence.
- **Segmentation:** Which exact pixels or voxels? → pixel/voxel mask.

## Match the healthcare data to the model family

- **Tabular data:** patient measurements → regression, trees, MLPs.
- **2D images:** X-ray, skin, pathology → CNNs and ResNets.
- **Text:** notes, reviews, prompts → TextCNN and LLM workflows.
- **3D imaging:** CT, MRI, CBCT → 3D CNNs, detectors, and U-Nets.
- **Deployment:** API or web interface → safe demonstration workflows.

## Responsible AI checkpoints

- Keep test data untouched.
- Use healthcare-relevant metrics rather than accuracy alone.
- Check calibration; a model score must not automatically be interpreted as true clinical risk.
- Quantify uncertainty where appropriate.
- Assess dataset and distribution shift.
- Document limitations, intended use, and prohibited use.
- Never upload identifiable patient information to teaching notebooks.

## Repository

[AI in Healthcare — Huawei-Inspired Labs on GitHub](https://github.com/dr-lamia/AI-in-Healthcare-Huawei-Labs)

## Full commented notebook editions

The full richly commented versions of the 18 notebooks are available in the course Google Drive folder:

[Open the full commented notebooks](https://drive.google.com/drive/folders/1CJgBd9inFLvnVzGmxpkIJfGkh0O2I-e7)

## Relationship to Huawei HCIA-AI

The laboratory sequence is an independent healthcare-focused educational adaptation inspired by the structure and learning progression of the Huawei HCIA-AI V4.0 laboratory material. Healthcare examples and original extensions are clearly separated from official Huawei material. This repository does not imply Huawei endorsement.
