# geez-script-recognition-crnn
Deep learning-based Ge'ez script recognition system using CRNN (CNN + BiLSTM + CTC) with advanced preprocessing for historical manuscript digitization.
# Ge'ez Script Recognition Using CRNN for Historical Manuscript Digitization

A deep learning-based Optical Character Recognition (OCR) system for recognizing Ge'ez script from historical manuscripts using a Convolutional Recurrent Neural Network (CRNN) with Connectionist Temporal Classification (CTC) loss and an advanced image preprocessing pipeline.

This project was developed as my final-year Computer Science and Engineering thesis.

---

## Overview

Historical Ge'ez manuscripts preserve centuries of religious, linguistic, and cultural heritage in Ethiopia and Eritrea. Digitizing these documents is challenging due to page degradation, skew, noise, faded ink, and the large Ge'ez syllabary, where many characters differ only by subtle visual details.

This project introduces an automated recognition system that combines classical image preprocessing with deep learning to accurately recognize Ge'ez script from historical manuscripts.

---

## Key Features

* Automatic border removal
* Skew detection and correction
* Noise filtering
* Contrast enhancement
* Adaptive image binarization
* CNN-based feature extraction
* Bidirectional LSTM sequence modeling
* CTC loss for sequence recognition
* Full-page text line extraction
* Character Error Rate (CER) evaluation

---

## Model Architecture

The recognition model consists of:

* Five-block Convolutional Neural Network (CNN)
* Two-layer Bidirectional LSTM
* Fully Connected Classification Layer
* Connectionist Temporal Classification (CTC) Loss

This architecture enables end-to-end sequence recognition without requiring character-level segmentation.

---

## Dataset

* 57,891 clean text-line images
* Three-fold data augmentation
* Approximately 121,000 training samples per epoch

---

## Performance

### Line-Level Recognition

* Character Error Rate (CER): **0.58%**
* Character Accuracy: **99.42%**

### Full-Page Recognition

* Character Error Rate (CER): **26.35%**

The significant difference between line-level and page-level performance highlights the importance of robust document layout analysis and handling severe manuscript degradation.

---

## Technologies

* Python
* PyTorch
* OpenCV
* NumPy
* Pillow (PIL)
* Matplotlib
* Google Colab

---

## Repository Structure

```text
├── Final_project_Thesis.ipynb
├── README.md
├── requirements.txt
├── preprocessing/
├── models/
├── checkpoints/
├── sample_images/
├── results/
└── images/
```

---

## Applications

* Historical manuscript digitization
* Digital preservation of Ge'ez manuscripts
* OCR for low-resource languages
* Digital humanities
* Ethiopian and Eritrean cultural heritage preservation

---

## Future Work

* Transformer-based OCR architectures
* Improved page layout analysis
* Recognition of severely degraded manuscripts
* Language-model-assisted post-processing
* Deployment as a web application

---

## Citation

If you use this work in your research, please cite the accompanying thesis.

---

## Authors

**Leake Abrha**, **Leake Adisalem**, **Biniam Gebreyesus**, **Freweyni Asgedom**

B.Sc. in Computer Science and Engineering

Research Interests:

* Artificial Intelligence
* Computer Vision
* Deep Learning
* Optical Character Recognition (OCR)
* Natural Language Processing
* Low-Resource Language Technologies
