# Audio Transcription App

This is a simple web application that allows users to record audio through their microphone and transcribe the audio using the Groq API with Whisper model. The transcription results are displayed on the page.

## Features

- Record audio through the browser.
- Transcribe recorded audio using Groq API.
- Display transcription results on the page.
- Maintain a history of transcriptions without overwriting.

## Technologies Used

- FastAPI
- Pydub
- aiohttp
- HTML/CSS/JavaScript

## Getting Started

### Prerequisites

- Python 3.7+
- Pip (Python package installer)
- Groq API Key

### Installation

1. **Clone the Repository**:
   ```sh
   git clone https://github.com/siddharth-k03/Groq-API-Transcription.git
   cd Groq-API-Transcription
   pip install -r requirements.txt

### Running the Application

1. Start the FastAPI Server
    ```sh
    python server.py

2. Open your Browser:
- Navigate to `http://localhost:8000` to access the application.

### Usage

1. Click on "Start Recording" to start recording audio through your microphone.
2. Click on "Stop Recording" to stop recording. The transcription will be processed and displayed below.
3. Each transcription result is appended, separated by a line.
