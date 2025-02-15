  ---

# 🎙️ Speech Emotion Detection  

This project implements a **Speech Emotion Detection** model using **CNNs** and audio features from the **TESS dataset**. It classifies speech into seven emotions using deep learning techniques.  

---

## 📌 Features  
- 📂 Processes the **TESS** dataset with 7 emotions.  
- 🧠 Implements a **CNN-based** deep learning model using PyTorch.  
- 🎨 Includes **visualizations** for analysis.  

---

## 📊 Dataset  
The **TESS (Toronto Emotional Speech Set)** dataset contains recordings labeled with the following emotions:  
- 😡 **Angry**  
- 🤢 **Disgust**  
- 😨 **Fear**  
- 😃 **Happy**  
- 😐 **Neutral**  
- 😲 **Pleasant Surprise**  
- 😢 **Sad**  

---

## 🏗️ Model Architecture  
The model is a **1D CNN** designed to extract features from speech signals and classify emotions.  

### 🔧 Architecture Details  
- **Input**: Extracted features from speech audio (e.g., MFCCs).  
- **Conv1D Layer 1**:  
  - Input: 40 channels (audio features)  
  - Output: 64 channels  
  - Kernel size: 3, Stride: 1, Padding: 1  
  - Activation: **ReLU**  
  - Followed by **MaxPool1D** (kernel=2)  
- **Conv1D Layer 2**:  
  - Input: 64 channels → Output: 128 channels  
  - Kernel size: 3, Stride: 1, Padding: 1  
  - Activation: **ReLU**  
  - Followed by **MaxPool1D** (kernel=2)  
- **Flatten Layer**: Converts the output into a feature vector.  
- **Fully Connected Layer 1 (FC1)**:  
  - Input: Flattened feature vector  
  - Output: 128 neurons  
  - Activation: **ReLU**  
- **Fully Connected Layer 2 (FC2 - Output Layer)**:  
  - Input: 128 neurons  
  - Output: 7 neurons (one for each emotion)  
  - Activation: **Softmax** (for classification)  

---

## 🛠️ Installation & Setup  

### 📥 Clone the Repository  
```bash
git clone https://github.com/wajee-ul-hassan/speech-emotion-detection.git
cd speech-emotion-detection
```  

This version enhances readability and keeps the formatting clean and professional. Let me know if you need further refinements! 🚀
