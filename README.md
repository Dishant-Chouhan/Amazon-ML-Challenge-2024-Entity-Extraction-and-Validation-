
# Amazon ML Challenge 2024 - Entity Extraction and Validation  

## Overview  
This repository contains our team's solution to the **Amazon ML Challenge 2024**, where we tackled the task of automating **entity extraction and validation** from images using state-of-the-art AI techniques. The challenge involved processing image data to extract critical entities such as dates, amounts, and measurements with high accuracy and efficiency.  

**Final Rank:** **357 out of 75,000+ participants**

---

## Problem Statement  
The challenge required participants to extract text-based entities from images, preprocess the extracted text for standardization, and validate the extracted data against predefined rules or formats. Our solution focuses on leveraging **OCR**, **NLP**, and **deep learning** to handle noisy, low-quality images with challenging text formats.

---

## Solution Approach  

### 1. **Text Extraction**  
- Used **EasyOCR** to extract text from images.  
- Handled challenges such as low-contrast images, noisy backgrounds, and varied fonts.  

### 2. **Text Preprocessing**  
- Employed **Pandas** and **Regex** to clean and standardize text data.  
- Ensured uniformity across datasets for efficient entity extraction and validation.  

### 3. **Entity Extraction**  
- Built a custom **Convolutional Neural Network (CNN)** optimized using **Keras Tuner** for hyperparameter tuning.  
- Batch processing was implemented to handle large datasets, leveraging the power of an **RTX 3050 GPU** for faster training and inference.  

### 4. **Hyperparameter Optimization**  
- Applied **Random Search** to fine-tune hyperparameters like learning rate, number of layers, and filter sizes.  
- Evaluated models based on the **F1 Score** to balance precision and recall for optimal performance.  

### 5. **Image Preprocessing**  
- Enhanced image quality through preprocessing techniques such as:  
  - **Sharpening**  
  - **Resizing**  
  - **Contrast Enhancement**  
- Improved OCR accuracy on distorted or low-quality images.  

---

## Results  

- **Rank Achieved:** **357th out of 75,000+ participants.**  
- Our model demonstrated high accuracy in extracting and validating entities, with a strong balance between precision and recall.

---

## Challenges Addressed  

1. **Low-Quality Images:** Addressed through advanced preprocessing techniques.  
2. **Challenging Fonts and Layouts:** Overcame using robust OCR and NLP pipelines.  
3. **Large Datasets:** Optimized training and inference with batch processing and GPU acceleration.  

---

## How to Use  

### Prerequisites  
- Python 3.8+  
- NVIDIA GPU (recommended for faster training)  
- Required libraries:  
  - TensorFlow  
  - EasyOCR  
  - Keras Tuner  
  - Pandas  
  - scikit-learn  
  - tqdm  

Install dependencies using:  
```bash
pip install -r requirements.txt
```


## File Structure  

```
├── dataset/
│   ├── train/
│   ├── test/
├── scripts/
│   ├── preprocess.py
│   ├── train.py
│   ├── predict.py
├── results/
│   ├── predictions.csv
├── README.md
├── requirements.txt
```

---



## Future Work  

- Integrating more advanced NLP techniques for improved entity extraction.  
- Scaling the model for deployment in real-world applications.  
- Exploring additional OCR libraries for better multilingual support.  

---


