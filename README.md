# Image-Caption-Generator-Using-CNN-and-LSTM-
Image Caption Generator using CNN and LSTM that automatically generates textual descriptions for images. A pre-trained Xception CNN extracts visual features, and an LSTM network generates captions word by word. Trained on the Flickr8k dataset, combining Computer Vision and NLP.

Project Overview
This project implements an **Image Caption Generator** that automatically generates textual descriptions for images using **Deep Learning**. It combines **Computer Vision** and **Natural Language Processing** by using a **Convolutional Neural Network (CNN)** for image feature extraction and a **Long Short-Term Memory (LSTM)** network for caption generation.

The model is trained on the **Flickr8k dataset** and can generate captions for unseen images.

---

 Technologies Used
- Python
- TensorFlow / Keras
- CNN (Xception – pre-trained on ImageNet)
- LSTM
- Natural Language Processing (NLP)
- NumPy, PIL, Matplotlib

---

 Dataset
- **Flickr8k Dataset**
- 8,000 images
- Each image has 5 human-written captions
- Dataset is split into training and testing sets

 Dataset files are not included in this repository due to size limitations.

---

 Model Architecture
- **Encoder:** Pre-trained Xception CNN (feature extractor)
- **Decoder:** LSTM-based language model
- **Embedding Layer:** Converts words into vector representations
- **Softmax Layer:** Predicts the next word in the caption

---

Workflow
1. Input image is resized and preprocessed  
2. CNN extracts visual features from the image  
3. Captions are tokenized and converted to sequences  
4. LSTM generates captions word by word  
5. Caption generation stops when the `<end>` token is predicted  

---

How to Run the Project

 Install Dependencies
```bash
pip install -r requirements.txt

Run Caption Generation
python test.py -i Flicker8k_Dataset/image_name.jpg

Sample Output

Input Image:
Dog running in water

Generated Caption:

a dog running through water
