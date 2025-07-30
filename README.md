# 🍽️ Calorie Estimation from Food Images using Deep Learning

This project implements a two-step deep learning pipeline to estimate the **calorie content of food images**. It combines **image classification** using a fine-tuned CNN (ResNet18) and **regression modeling** to estimate calories based on the identified food type.

---

## 📂 Project Structure

| File/Folder                        | Description                                                |
|-----------------------------------|------------------------------------------------------------|
| `calorie_estimation.ipynb`        | Full Jupyter Notebook with code, analysis, and results     |
| `calorie_estimation.py`           | Python script version of the notebook                      |
| `calorie_estimation.html`         | Exported HTML version of the notebook                      |
| `calorie_estimation.pdf`          | PDF version of the notebook (useful for offline review)    |
| `Calorie_Estimation_Presentation_FINAL.pptx` | Final presentation with visuals + speaker notes   |

---

## 📊 Overview

The pipeline consists of two main components:

1. **Food Classification**  
   - Model: `ResNet18` (Transfer Learning)  
   - Dataset: Food-101  
   - Output: Predicted food class (e.g., pizza, sushi)

2. **Calorie Regression**  
   - Input: One-hot encoded food class  
   - Models: Linear Regression, Random Forest, Gradient Boosting  
   - Output: Estimated calorie count

> 🏆 Best performance: **Gradient Boosting**  
> - MAE: 19.23  
> - RMSE: 24.56

---

## 📁 Dataset

- **Name**: Food-101 Dataset  
- **Author**: Lukas Bossard, Matthieu Guillaumin, Luc Van Gool  
- **Details**:
  - 101 food categories
  - ~75,000 training images
  - ~25,000 test images
- **Note**: The dataset does not include calorie data.  
  Calories were mapped externally using nutrition databases.

🔗 **Download from Kaggle**:  
https://www.kaggle.com/datasets/kmader/food41  
📚 [Original Paper (ECCV 2014)](https://www.vision.ee.ethz.ch/datasets_extra/food-101/)

---

## 🔧 Tech Stack

- Python 3.10+
- PyTorch & Torchvision
- Scikit-learn
- Pandas, NumPy, Matplotlib, Seaborn
- Jupyter Notebook

---

## 📽️ Demo Video

🎥 [Insert link to your video presentation here — YouTube or Google Drive]

---
