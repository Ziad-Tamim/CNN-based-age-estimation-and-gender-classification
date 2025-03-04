# Age Estimation and Gender Classification Using CNNs

<p align="center">
  <img src="https://github.com/user-attachments/assets/157dad2d-dd3c-406c-8be8-f7e08b677ec6" width="600" alt="Age Estimation and Gender Classification">
</p>

This repository contains a project focused on predicting a person's age and gender from facial images using Convolutional Neural Networks (CNNs). The project explores two distinct approaches:

- Model A (Scrach model): A CNN built from scratch that learns features directly from the training data. The trained model is saved as age_gender_A.keras.
- Model B (MobileNetV2): A CNN that leverages transfer learning by fine-tuning a pre-trained model. This approach benefits from previously learned feature representations, with the final model saved as age_gender_B.keras.

## Dataset
The experiments are conducted on a subset of the UTKFace dataset, which comprises 23,708 labeled face images. Each image is resized to 128 x 128 pixels, and the data is organized within the Dataset/ directory.

## Performance Metrics
Age Estimation: Evaluated using Mean Absolute Error (MAE).
Gender Prediction: Evaluated based on accuracy.

## Repository Structure
Notebooks: Detailed Jupyter notebooks that document the data preprocessing, model training, and evaluation processes.
Models: Saved model files (age_gender_A.keras and age_gender_B.keras) representing the trained models.
Dataset: The subset of the UTKFace dataset used in this project, located in the Dataset/ directory.

## How to Run
1. Clone the Repo: ```git clone <repository-url>```
2. Navigate to the project directory:
```cd age-estimation-gender-classification```
3. Install the required dependencies:
``` pip install -r requirements.txt ```
4. Run the notebooks to reproduce the experiments.


## Results
### Model A

<p align="center">
  <img src="https://github.com/user-attachments/assets/670faa0c-38d5-4d43-9ee6-2bc271f49c7b" width="600" alt="Age Estimation and Gender Classification">
</p>
Over 10 epochs, the model shows strong improvements: training loss dropped from ~377 to ~69 and validation loss from ~224 to ~91, with age MAE decreasing from ~14.8 to ~6.2 (training) and ~11.2 to ~7.1 (validation), while gender accuracy increased from ~58.8% to ~87.1% (training) and ~76.1% to ~87.1% (validation).

### Model B

<p align="center">
  <img src="https://github.com/user-attachments/assets/a3098b83-bb68-44cd-97c8-08e88247fc79" width="600" alt="Age Estimation and Gender Classification">
</p>
Model B’s performance over 10 epochs shows a clear reduction in training loss and age MAE—from about 194.7 to 114.9 and 10.3 to 7.7 respectively—indicating solid learning on the training data. However, the validation metrics fluctuate considerably, with validation loss and age MAE not following a steady decline and gender accuracy varying between roughly 61% and 73%. This suggests that while the model fits the training set well, its generalization on unseen data is inconsistent and may benefit from further tuning or regularization.


Feel free to explore the notebooks and models, and contribute to further improvements!
