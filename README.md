# 📄 End-to-End OCR Pipeline

An end-to-end Optical Character Recognition (OCR) pipeline designed to extract text from noisy, non-standard document layouts. This project combines robust classical image preprocessing techniques with both traditional and deep-learning-based OCR engines, featuring automated evaluation using industry-standard error metrics.

Developed at **AME, IIT Kanpur** *(Dec 2025 – Jan 2026)*.

---

## 🌟 Key Features

* **Advanced Image Preprocessing:** * Implemented an automated cleaning pipeline utilizing grayscale conversion, morphological operations (erosion/dilation), and adaptive thresholding to effectively remove background noise and enhance text contrast on degraded documents.
* **PyTesseract Optimization:** * Fine-tuned Tesseract’s Page Segmentation Modes (**PSM**) and OCR Engine Modes (**OEM**) to optimize bounding box accuracy and improve text region detection across complex, non-standard document structures.
* **Deep Learning Benchmarking via EasyOCR:** * Instantiated pre-trained deep learning OCR models using **EasyOCR** (based on CRAFT and CRNN architectures) to benchmark extraction performance against classical Tesseract.
* **Quantitative Performance Evaluation:** * Integrated the **Jiwer** library to rigorously evaluate model accuracy using **Word Error Rate (WER)** and **Character Error Rate (CER)**. Demonstrated demonstrably higher accuracy with deep learning approaches over classical engines on degraded text.

---

## 🛠️ Tech Stack

* **Language:** Python 3.8+
* **Image Processing:** OpenCV (`cv2`), Pillow (`PIL`), NumPy
* **OCR Engines:** * `pytesseract` (Tesseract OCR Engine)
  * `easyocr` (PyTorch-based Deep Learning OCR)
* **Evaluation Metrics:** `jiwer` (WER, CER, MER, WIL)
* **Data Manipulation & Visuals:** Pandas, Matplotlib

---

## 📁 Repository Structure

```text
End-to-End-OCR-Pipeline/
│
├── EasyOCR (1).ipynb        # Implementation and benchmarking using EasyOCR
├── Pytesseract.ipynb        # Tesseract pipeline with custom PSM/OEM configs
├── image_fundamentals.ipynb # Image preprocessing (grayscale, morphological ops, etc.)
└── README.md                # Project documentation
