# CodeAlpha_Emotion_Recognition_From_Speech

## Emotion Recognition from Speech

### How to Run

1. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

2. **Train the model:**
   ```bash
   python emotion_recognition.py
   ```
   This will train the model on the audio files in the `dataset/` folder and save the trained model as `emotion_model.h5` and the label encoder as `label_encoder.pkl`.

3. **Predict emotion from a new audio file:**
   You can use the `predict_emotion` function in `emotion_recognition.py` to predict the emotion from a new `.wav` file:
   ```python
   from emotion_recognition import predict_emotion
   emotion = predict_emotion('path_to_audio.wav')
   print('Predicted emotion:', emotion)
   ```

### Dataset
- Place your RAVDESS (or similar) dataset in the `dataset/` folder, organized by actor as subfolders.

### Features
- MFCCs (Mel-Frequency Cepstral Coefficients) are extracted from each audio file.
- Model: Feedforward neural network (can be replaced with LSTM/CNN for further improvement).

---