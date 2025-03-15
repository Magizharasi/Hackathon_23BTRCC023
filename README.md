# Hackathon_23BTRCC023
# Own Project
This is my own project which is present in the 'main' folder.

Real-time Speech Translator

A web application that transcribes English speech in real-time and translates it into French.

### Features

Real-time speech recognition in English

Instant translation to French

Beautiful, responsive UI with animation effects
  
WebSocket-based architecture for low latency
  
Robust error handling and reconnection logic

### How It Works

1. Speech is captured through your device's microphone
2. Audio is processed on the server using Vosk for speech recognition
3. Recognized text is translated using Microsoft's Translator API
4. Both the original transcription and translation are displayed in real-time

### Technologies Used
#### Backend

1. Python 3.12
2. Vosk (speech recognition)
3. Microsoft Translator API
4. aiohttp (WebSocket server)
5. sounddevice (audio capture)

#### Frontend

1. HTML5
2. CSS3
3. JavaScript (Vanilla)
4. WebSocket API

#### Requirements

1. Python 3.12 or higher
2. Vosk speech recognition model
3. Microsoft Translator API key
A microphone connected to your device

### Installation
1.Clone this repository:

      https://github.com/Magizharasi/Hackathon_23BTRCC023/tree/main/main
      cd main
2.Install Python dependencies:

      bashCopypip install vosk sounddevice aiohttp aiohttp_cors websockets asyncio requests

3.Download the Vosk model:
      
      bashCopy# Download the small English model
      wget https://alphacephei.com/vosk/models/vosk-model-small-en-us-0.15.zip
      unzip vosk-model-small-en-us-0.15.zip

4.Update the model path in app.py:

      pythonCopyMODEL_PATH = "path/to/vosk-model-small-en-us-0.15"

5.Obtain a Microsoft Translator API key:

Sign up for the Microsoft Azure Translator service
Create a resource and get your API key
Update the API_KEY and REGION values in app.py:
pythonCopyAPI_KEY = "your-api-key"
REGION = "your-region"
