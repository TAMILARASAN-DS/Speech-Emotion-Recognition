# 🎙️ Speech Emotion Recognition (SER) using Deep Learning & Traditional ML

This project implements an End-to-End **Speech Emotion Recognition (SER)** system using the **RAVDESS** (Ryerson Audio-Visual Database of Emotional Speech and Song) dataset. It classifies audio clips into 8 different emotions (Neutral, Calm, Happy, Sad, Angry, Fearful, Disgust, Surprised) and performs frame-wise sentiment analysis over time.

---

### 📊 Project Workflow
1. **Data Preprocessing & Normalization:** Automatically downloads the RAVDESS dataset and normalizes all audio files to a fixed duration (4.0 seconds) and sample rate (22050 Hz).
2. **Feature Extraction:** Extracts robust audio features combining:
   - **MFCCs** (Mel-Frequency Cepstral Coefficients)
   - **Chroma STFT**
   - **Mel-Spectrogram**
   - **Spectral Contrast**
3. **Model Training & Comparison:**
   - **Deep Learning (Keras/TensorFlow):** A multi-layer Sequential Neural Network with Dropout and Early Stopping.
   - **Traditional Machine Learning Models:** Logistic Regression, Random Forest, and Support Vector Machine (SVM) evaluated for performance comparison.
4. **Time-Series / Frame-wise Prediction:** Splits uploaded audio files into frames to visualize emotion progression, timelines, and overall sentiment distribution over time.

---

### 🛠️ Tech Stack & Libraries
- **Language:** Python
- **Audio Processing:** `librosa`, `soundfile`
- **Machine Learning & Deep Learning:** `TensorFlow / Keras`, `Scikit-Learn`, `NumPy`
- **Visualization:** `Matplotlib`, `Seaborn`

---

### 🚀 How to Run the Project
1. Clone this repository or open the Jupyter Notebook in **Google Colab**.
2. Install the required dependencies:
   ```bash
   pip install librosa soundfile tensorflow scikit-learn tqdm matplotlib seaborn
