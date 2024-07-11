# Audio Transcription and Sentiment Analysis App

This is a simple web application that allows users to record audio through their microphone and transcribe the audio using the Groq API with the Whisper model. Additionally, the application performs sentiment analysis on the transcription using the Groq API with the Llama3 model. The transcribed text is then converted to speech using the ElevenLabs API, and the audio is played in the user's browser. The transcription, sentiment analysis results, and the audio are displayed on the page.

## Features

- Record audio through the browser.
- Transcribe recorded audio using the Groq API.
- Perform sentiment analysis on the transcribed text using the Groq API.
- Convert the transcribed text to speech using the ElevenLabs API.
- Play the generated audio in the user's browser.
- Display transcription and sentiment analysis results on the page.
- Maintain a history of transcriptions and sentiment analyses.

## Technologies Used

- FastAPI
- Pydub
- aiohttp
- Groq API (Whisper Large V3 and Llama 8b 8192)
- ElevenLabs API
- HTML/CSS/JavaScript

## Getting Started

### Prerequisites

- Python 3.7+
- Pip (Python package installer)
- Groq API Keys for Whisper and Llama separately
- ElevenLabs API Key

### Installation

1. **Clone the Repository**:
    ```sh
    git clone https://github.com/siddharth-k03/Groq-API-Transcription.git
    cd Groq-API-Transcription
    ```

2. **Install Dependencies**:
    ```sh
    pip install -r requirements.txt
    ```

### Running the Application

1. **Replace <voice-id> in `server.py`**:
You can find an appropriate voice and its respective voice-id from the ElevenLabs website (https://elevenlabs.io/docs/api-reference/get-voices).

2. **Start the FastAPI Server**:
    ```sh
    python server.py
    ```

3. **Open your Browser**:
    - Navigate to `http://localhost:8000` to access the application.

### Usage

1. Click on "Start Recording" to start recording audio through your microphone.
2. Click on "Stop Recording" to stop recording. The transcription will be processed and displayed below.
3. Each transcription result is appended, separated by a line.
4. Sentiment analysis of the transcription will be performed and displayed along with the transcription result.
5. The transcribed text will be converted to speech, and the generated audio will be played in the browser.

### Branches

- **main**: Contains the original transcription functionality.
- **sentiment-analysis**: Contains the updated code with added sentiment analysis functionality.
- **text-to-speech**: Contains the updated code with added sentiment analysis and text to speech functionalities.