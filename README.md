# OCR Project with EasyOCR  

This project uses EasyOCR and OpenCV to perform Optical Character Recognition (OCR) on images stored in a Google Drive folder. It focuses on extracting and standardizing numeric values from images.  

---

## Features  
1. **Processes multiple images** from a specified folder in Google Drive.  
2. **Applies advanced image preprocessing** techniques (contrast enhancement, adaptive thresholding).  
3. **Detects text** using EasyOCR and filters numeric values.  
4. **Displays extracted text** on the processed images.  

---

## How It Works  

### 1. Image Preprocessing  
- Enhances image quality using CLAHE and adaptive thresholding.  
- Detects and focuses on regions of interest (ROIs) using contour detection.  

### 2. OCR Processing  
- Uses EasyOCR to extract text from cropped ROIs.  

### 3. Standardization  
- Filters and combines numeric values using regular expressions.  

### 4. Results  
- Outputs extracted numbers and displays processed images with detected text.  

---

## Prerequisites  

Ensure you have the following installed:  
- **Python 3.7+**  
- Required Python packages:  
  ```bash
  pip install easyocr opencv-python-headless numpy
