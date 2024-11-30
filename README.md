# Amazon ML Challenge 2024 - Entity Extraction and Validation  

## Overview  
This repository contains our team's solution to the **Amazon ML Challenge 2024**, focusing on automating **entity extraction and validation** from images. The project demonstrates the extraction of structured information (e.g., weight, dimensions, voltage) from unstructured image data, leveraging advanced machine learning techniques.

**Final Rank:** **357 out of 75,000+ participants**

---

## Problem Statement  
The challenge was to extract entity values (e.g., "item weight: 34 grams") from product images, standardize the extracted values, and validate them against predefined rules. This is essential for industries such as e-commerce, healthcare, and content moderation, where accurate metadata directly impacts operations like inventory management, recommendation systems, and quality control.

---

## Solution Approach  

### 1. **Text Extraction (OCR)**  
- Implemented **EasyOCR** for robust text extraction from images.  
- Addressed challenges like varied fonts, noisy backgrounds, and low-quality images.  

### 2. **Text Preprocessing**  
- Used **Pandas** and **Regex** for cleaning, standardizing, and tokenizing text data.  
- Ensured consistent formatting to align with the output requirements.  

### 3. **Entity Extraction and Validation**  
- Designed a custom **Convolutional Neural Network (CNN)** model optimized for image features.  
- Fine-tuned the model using **Keras Tuner** with metrics such as **F1 Score** to maximize precision and recall.  

### 4. **Unit Detection**  
- Built an **NLP-based parser** to detect allowed units from constants.py.  
- Implemented rules to validate and convert units into the expected format.  

### 5. **Hyperparameter Optimization**  
- Employed **Random Search** for efficient hyperparameter tuning.  
- Focused on batch size, learning rates, and layer configurations.  

### 6. **Image Preprocessing**  
- Applied techniques like sharpening, resizing, and contrast enhancement to improve OCR accuracy.  
- Batch processed large image datasets using GPU acceleration for efficiency.  

---

## Dataset  

- **Training Dataset:** Contains product images with labeled entity values (e.g., weight, dimensions).  
- **Test Dataset:** Contains product images with no labeled values, requiring predictions to be made.  
- **Output Format:** Predictions must match a specific format, e.g., `12.5 gram`.  

---

## Features  

- **Efficient OCR Integration:** Robust text extraction from diverse and noisy image datasets.  
- **Entity Standardization:** Automated validation against predefined unit rules and formats.  
- **Real-World Scalability:** Preprocessing techniques and GPU acceleration allow handling of large datasets.  
- **Custom CNN Model:** Fine-tuned model for high accuracy on challenging image data.  

---


