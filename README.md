# Image Caption Generation with Voice Assistance

## Project Description
This project develops an Image Caption Generation system with Voice Assistance. It automatically generates meaningful captions for images and converts them into speech, improving accessibility and user interaction.

## Implementation Details
The system follows a deep learning pipeline:

- Image Input: Upload or capture image using UI  
- Preprocessing: Resize, normalize, convert to tensor  
- Feature Extraction: CNN (ResNet-50) extracts image features  
- Caption Generation: LSTM generates captions word-by-word  
- Attention & Beam Search: Improves caption quality  
- Text-to-Speech: Converts caption into audio  
- Additional Features: Caption saving and session history  

## Technologies Used
- Python  
- PyTorch  
- NumPy  
- Pandas  
- Transformers  
- Pillow  
- CustomTkinter  
- pyttsx3  

## How to Run
```bash
pip install -r requirements.txt
python caption_generationn.py
