# Image Caption Generator

This project implements an image captioning model using a combination of **VGG16** for image feature extraction and a **Bidirectional LSTM** for generating natural language descriptions. The goal is to produce meaningful and grammatically correct captions for input images.

---

## Objective

To generate text-based descriptions for images using deep learning techniques that combine computer vision and sequence modeling.

---

## Model Summary

- **Feature Extractor**: VGG16 (pre-trained on ImageNet), used to convert images into feature vectors.
- **Caption Generator**: A Bidirectional LSTM model trained to predict sequences of words based on extracted image features.
- **Dataset**: Flickr8k dataset (8,000 images, each with five human-written captions).

---

## Folder Structure

image-caption-generator/
│
├── model/ # Trained model weights (optional)
├── captions/ # Processed caption data
├── images/ # Image dataset samples
├── utils.py # Tokenizer, preprocessing, helper functions
├── caption_generator.py # Main script to load model and generate captions
├── train.py # Model training script
├── requirements.txt # Required Python packages
└── README.md # Project documentation




---

## How to Use

1. **Install dependencies**
```bash
pip install -r requirements.txt


2.Example Output
Input Image → "Two children are playing with a soccer ball in the park."
(Note: Sample output will vary based on training data and configuration.)

Dependencies
Python 3.8+
TensorFlow 
NumPy
Matplotlib (for visualization)


3.Future Improvements
Integrate attention mechanism
Add web interface (e.g., with Flask or Streamlit)
Extend support for larger datasets (e.g., MS COCO)

