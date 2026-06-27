# Blood Cell Classification — Deep Learning Project

**Student:** YOUR_NAME_HERE | **SRN:** YOUR_SRN_HERE
**University:** Hazara University, Mansehra
**Supervisor:** Mam Romana Saleem

## Dataset
- Source: Kaggle — bloodcells_dataset
- 8 classes: basophil, eosinophil, erythroblast, ig,
  lymphocyte, monocyte, neutrophil, platelet
- Total: 17,092 images
- Split: 70% Train | 15% Val | 15% Test

## Environment Setup
pip install torch torchvision torchaudio
pip install numpy pandas matplotlib scikit-learn
pip install opencv-python Pillow captum seaborn tqdm jupyter

## Dataset Preparation
1. Download from Kaggle: bloodcells_dataset
2. Place in: data/raw/bloodcells_dataset/
3. Each class should be a subfolder with images

## How to Train
1. Activate venv: C:\Users\User\venv\Scripts\Activate.ps1
2. cd C:\Users\User\BloodCell-Project
3. Run: jupyter notebook
4. Open BloodCell_DL_Project.ipynb
5. Run all cells in order

## Model Results
| Model        | Accuracy | F1 Score |
|-------------|----------|----------|
| CNN3        | 66.1%    | 0.6138   |
| CNN4        | 74.5%    | 0.6939   |
| CNN5        | 88.0%    | 0.8748   |
| MobileNetV2 | 86.0%    | 0.8570   |
| SqueezeNet  | 85.6%    | 0.8574   |
| ResNet34    | 97.7%    | 0.9774   |

## Outputs
All results saved in outputs/:
- class_distribution.png
- sample_images.png
- ModelName_learning_curves.png
- ModelName_confusion_matrix.png
- ModelName_gradcam.png
- final_model_comparison.csv

## Git Commit History
- Task1.1: Dataset placement and validation
- Task1.2: Data validation - 0 corrupted images
- Task1.3: Preprocessing transforms defined
- Task1.4: Train/val/test split and DataLoaders created
- Task2.1: Custom CNN3/CNN4/CNN5 architectures implemented
- Task2.2: All custom CNNs trained
- Task2.3: Evaluation complete - CNN5 best at 88%
- Task3: Transfer learning - ResNet34 best at 97.7%
- Task4: Grad-CAM XAI applied to CNN5 and ResNet34
- Task5: Report and README complete