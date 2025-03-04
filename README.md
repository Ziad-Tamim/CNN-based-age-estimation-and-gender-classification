# Age Estimation and Gender Classification Using CNNs

This repository contains a project focused on predicting a person's age and gender from facial images using Convolutional Neural Networks (CNNs). The project explores two distinct approaches:

- Model A: A CNN built from scratch that learns features directly from the training data. The trained model is saved as age_gender_A.keras.
- Model B: A CNN that leverages transfer learning by fine-tuning a pre-trained model. This approach benefits from previously learned feature representations, with the final model saved as age_gender_B.keras.

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

Feel free to explore the notebooks and models, and contribute to further improvements!
