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

  ## Setup and Usage  

1. **Prepare Your Dataset**:  
   - Upload images to a folder in your Google Drive (e.g., `My Drive/Dataset/`).  

2. **Run the Code**:  
   - Open the script in Google Colab.  
   - Mount Google Drive when prompted.  
   - Update the `image_folder` variable to match your Google Drive path.  

3. **View Results**:  
   - Numeric values extracted from images will be printed.  
   - Processed images with detected text will be displayed.  

---

## Folder Structure  

```plaintext
|-- Dataset/            # Folder containing input images in Google Drive  
|-- ocr_project.py      # Main Python script  
|-- README.md           # Project documentation  

## Dependencies  

Install the following Python libraries:  
- [EasyOCR](https://github.com/JaidedAI/EasyOCR)  
- OpenCV  
- NumPy  

To install all dependencies, you can create a `requirements.txt` file and add the following content:

```plaintext
easyocr
opencv-python-headless
numpy

To install the required Python libraries, run the following command:

```bash
pip install easyocr opencv-python-headless numpy
