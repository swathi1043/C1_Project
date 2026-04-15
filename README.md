# Image Caption Generation with Voice Assistance

## 📌 Project Description
This project focuses on developing an intelligent Image Caption Generation system integrated with Voice Assistance. The system automatically analyzes input images and generates meaningful, context-aware textual descriptions, which are further converted into speech output. 

It combines Computer Vision and Natural Language Processing techniques to bridge the gap between visual understanding and human language. The inclusion of voice output enhances accessibility, making the system especially useful for visually impaired users and real-time applications.

The application is designed with a simple and user-friendly interface using CustomTkinter, where users can upload an image or capture one using a webcam and instantly receive both textual and audio descriptions.

---

## ⚙️ Implementation Details
The system is implemented using a deep learning pipeline consisting of multiple stages:

### 🖼️ Image Input
The system accepts input images either through file upload or real-time webcam capture. This flexibility allows users to work with both stored and live images.

### 🔄 Image Preprocessing
The input image is resized to a fixed dimension (e.g., 224×224), normalized, and converted into tensor format. This ensures compatibility with deep learning models and improves performance.

### 🧠 Feature Extraction (CNN)
A pretrained Convolutional Neural Network (ResNet-50) is used to extract high-level visual features from the image. These features capture important objects, patterns, and spatial information.

### ✍️ Caption Generation (LSTM)
The extracted features are passed to an LSTM (Long Short-Term Memory) network, which generates captions sequentially, word-by-word, based on learned contextual relationships.

### 🎯 Attention Mechanism & Beam Search
The attention mechanism enables the model to focus on relevant parts of the image while generating each word. Beam search is used to improve caption quality by selecting the most probable word sequences.

### 🔊 Text-to-Speech
The generated caption is converted into speech using the `pyttsx3` library. This feature enhances accessibility and allows users to listen to image descriptions.

### 💾 Additional Features
- Caption saving for future reference  
- Session history tracking  
- Single-screen UI for seamless interaction  

---

## 🧪 Evaluation Metrics
The system performance is evaluated using standard metrics:
- BLEU Score (BLEU-1 to BLEU-4) for n-gram matching  
- METEOR Score for semantic similarity  
- Overall caption accuracy and relevance  

---

## 🛠️ Technologies Used
- Python  
- PyTorch  
- NumPy  
- Pandas    
- Transformers  
- Pillow  
- CustomTkinter  
- pyttsx3  

---

## ▶️ How to Run
```bash
pip install -r requirements.txt
python caption_generationn.py
