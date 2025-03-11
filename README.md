# AI-Powered Live Translation & Speech Conversion

This project leverages AI technologies to enable real-time speech translation and text-to-speech conversion. The system records audio via the browser’s microphone, recognizes the speech, translates it to a different language, and converts the translated text back into speech. This provides an immersive and interactive experience that can break down language barriers.

## Technologies Used:
SpeechRecognition: Converts spoken language to text using Google's Speech-to-Text API.
Google Cloud Speech-to-Text API: For real-time audio transcription with high accuracy.
deep-translator: A Python library that provides easy access to Google Translate and other translation services.
Word2Vec (from Gensim): Helps improve translation quality by finding similar words and refining the translation.
gTTS (Google Text-to-Speech): Converts translated text back into speech.
pydub: Used to process and manipulate audio files.
Google Colab: Used for running the code and interacting with the browser’s microphone through JavaScript.

## How It Works:
Audio Capture: The user speaks into the microphone, and JavaScript in the browser captures the audio in real time.
Speech Recognition: The recorded audio is transcribed into text using the SpeechRecognition library and Google Cloud Speech-to-Text API.
Text Translation: The transcribed text is translated to a target language using the deep-translator library (Google Translate).
Word Refinement: Word2Vec embeddings refine the translated text by replacing words with their semantically similar counterparts for more contextually accurate translations.
Text-to-Speech: The translated text is then converted back into speech using gTTS (Google Text-to-Speech).
Audio Playback: Finally, the translated speech is played back to the user.

## Requirements:
To run this project, you'll need the following libraries:

gensim: For Word2Vec and word embeddings.
nltk: For natural language processing and tokenization.
deep-translator: For text translation.
SpeechRecognition: For audio transcription.
gTTS: For converting text into speech.
pydub: For audio manipulation.
google-cloud-speech: For using Google's Speech-to-Text API.
IPython: For handling audio display in the notebook.
ffmpeg: For audio file format conversion.
To install the required dependencies, run:

## bash
Copy
pip install gensim nltk deep-translator SpeechRecognition gTTS google-cloud-speech pydub ffmpeg IPython
You can also install the latest versions using --upgrade flags.

bash
Copy
pip install --upgrade gensim nltk deep-translator SpeechRecognition gTTS google-cloud-speech pydub ffmpeg IPython
Running the Code:
Clone the repository:
bash
Copy
git clone https://github.com/Utkarshm1/Freespeech.git
cd ai-powered-live-translation
Open the notebook in Google Colab or Jupyter Notebook.

Run the cells. The notebook will guide you through the process:

The first step will record audio using your browser's microphone.
It will then process the speech, translate it into the desired language, and convert the translated text back to speech.
Finally, it will play the translated speech audio back to you.
The translated speech will be in the target language, ready to be heard!

Folder Structure:
bash
Copy
/ai-powered-live-translation
│
├── Freespeech.ipynb   # Main notebook for live translation
├── requirements.txt                  # List of required Python packages
├── README.md                         # This README file

Contributing:
Feel free to contribute to this project! You can help by:

Improving the code.
Reporting bugs.
Suggesting new features.
