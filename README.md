# Text-Recognition-and-NLP-Processing-in-Native-Language

## 📝 Handwritten Hindi Text Recognition & Translation

This project is an end-to-end OCR and NLP pipeline built in **Google Colab** to extract **handwritten Hindi text** from images, clean and process the text, and then translate it into **English** using cutting-edge NLP tools.


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SHREYASINGHMAURYA/Text-Recognition-and-NLP-Processing-in-Native-Language/blob/main/NLPTA2SHREYA_SINGH_MAURYA.ipynb)

---

## 🚀 Features

- 🖼️ **Image Preprocessing**: Grayscale conversion and noise reduction using OpenCV  
- 🔎 **OCR**: Text extraction from Hindi handwriting using Tesseract  
- 🔤 **Text Normalization**: Clean and standardize Hindi text using Indic NLP Library  
- 📚 **Tokenization**: Word-level tokenization in Hindi  
- 🌍 **Translation**: Translate normalized Hindi text to English using Hugging Face Transformers  
- 📥 **Colab Support**: Fully executable in Google Colab with easy setup  

---

## 🛠️ Technologies Used

- `OpenCV` – for image processing  
- `Tesseract OCR` – for text extraction (`hin` language pack)  
- `Indic NLP Library` – for Hindi text normalization and tokenization  
- `HuggingFace Transformers` – for translation using MarianMT model  
- `SentencePiece` – tokenizer support for MarianMT  
- `Google Colab` – for cloud-based execution and GPU support  

---

## 🔧 Installation (for Google Colab)

Paste this in the first code cell of your Colab notebook:

```python
!pip install opencv-python pytesseract nltk indic-nlp-library transformers sentencepiece
!apt-get install -y tesseract-ocr-hin

import os
os.environ['TESSDATA_PREFIX'] = '/usr/share/tesseract-ocr/4.00/tessdata'
```

To display images in Colab:
```python
from google.colab.patches import cv2_imshow
```

---

## 📂 How It Works

1. Upload an image of handwritten **Hindi** text
2. Preprocess the image (grayscale, denoise)
3. Use Tesseract OCR to extract Hindi script
4. Normalize and tokenize the Hindi text
5. Translate the result into English using MarianMT (via Hugging Face)
6. Display outputs: raw text, tokens, and English translation

---

## 🧪 Sample Output

**Input Image:**  
*(handwritten Hindi)*

**Extracted Text (OCR):**  
> यह एक परीक्षण वाक्य है।

**Normalized Text:**  
> यह एक परीक्षण वाक्य है।

**Tokenized:**  
> ['यह', 'एक', 'परीक्षण', 'वाक्य', 'है', '।']

**Translated:**  
> This is a test sentence.

---

## 📌 Future Enhancements

- Streamlit or Gradio-based GUI  
- Named Entity Recognition (NER) on extracted text  
- Multilingual support for other Indian languages  
- Dataset expansion for better OCR accuracy  

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you’d like to change.

---

## 📜 License

This project is open source and available under the [MIT License](LICENSE).

---

