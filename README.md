🎭 Multimodal Emotion Recognition System
A hybrid emotion recognition system that analyzes facial expressions and vocal tone to identify human emotions from uploaded images and audio/video files. Built with Python, Whisper, Keras, Librosa, OpenCV, and hosted in Google Colab.
🚀 Features
•	• Speech Recognition & Transcription using OpenAI Whisper
•	• Audio Emotion Detection via MFCC + Pitch features and SVM
•	• Facial Emotion Detection using CNN on grayscale face images
•	• Language Detection from spoken audio
•	• Modular design for future integration (e.g., text-based emotion, video stream)
🛠️ Technologies Used
Component	Technology
Speech-to-Text	Whisper (base model)
Facial Emotion	Keras CNN
Audio Emotion	Librosa + Scikit-learn SVM
Visualization	OpenCV + cv2_imshow (Colab)
Audio Extraction	MoviePy
Interface	Google Colab
📁 Project Structure

emotion_recognition/
├── emotion_model.h5             # Trained CNN model for facial emotion
├── main_colab_notebook.ipynb    # Main Colab notebook (you run this)
├── sample_inputs/               # Example .jpg and .mp4 files (optional)
├── README.md                    # Project documentation

📦 Installation & Setup
•	• Open in Google Colab
•	• Upload Files (Image: .jpg/.png, Audio/Video: .mp3/.wav/.mp4)
•	• Get Results: Facial Emotion (OpenCV) + Audio Emotion + Language + Transcript
📊 Emotion Labels
Facial: Angry, Disgust, Fear, Happy, Sad, Surprise, Neutral
Audio: Happy, Sad, Angry, Neutral
(Text-based emotion classification can be added later)
⚙️ How It Works (Pipeline)
•	• Upload an image and/or audio/video file.
•	• Image is passed through OpenCV → Haar cascade → CNN for emotion prediction.
•	• Audio is converted to WAV → transcribed via Whisper → MFCC+Pitch features extracted.
•	• Audio features are classified using an SVM into emotion labels.
•	• Results are printed and/or shown with annotated images.
📈 Future Improvements
•	• Fusion-based multimodal deep model
•	• Real emotion-labeled audio training datasets
•	• Live webcam/video stream input
•	• Deployable mobile or edge version using TensorFlow Lite
•	• Text emotion classification from Whisper transcripts
❗ Limitations
•	• Audio classifier currently trained on random synthetic data
•	• No true integration/fusion between facial and audio predictions
•	• Not robust to poor lighting, occlusions, or high-noise audio
📄 License
This project is intended for educational and research purposes only. If you use it, please give credit to the developers and mention this repo.
👨‍💻 Author
Developed by [Your Name]
Email: your.email@example.com
Institution: [Your College or Organization]
🔗 References
•	• OpenAI Whisper
•	• FER2013 Facial Emotion Dataset
•	• Librosa Audio Feature Extraction
•	• Scikit-learn
•	• Keras & TensorFlow
•	• MoviePy for audio extraction
