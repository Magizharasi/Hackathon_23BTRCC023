# Hackathon_23BTRCC023
# Own Project
This is my own project which is present in the 'main' folder.

Real-time Speech Translator

A web application that transcribes English speech in real-time and translates it into French.

### Features

- Real-time speech recognition in English
- Instant translation to French
- Beautiful, responsive UI with animation effects
- WebSocket-based architecture for low latency
- Robust error handling and reconnection logic

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

      pip install vosk sounddevice aiohttp aiohttp_cors websockets asyncio requests

3.Download the Vosk model:
      
      # Download the small English model
      wget https://alphacephei.com/vosk/models/vosk-model-small-en-us-0.15.zip
      unzip vosk-model-small-en-us-0.15.zip

4.Update the model path in app.py:
'''bash
      MODEL_PATH = "path/to/vosk-model-small-en-us-0.15"

5.Obtain a Microsoft Translator API key:

  Sign up for the Microsoft Azure Translator service
 
  Create a resource and get your API key
  
  Update the API_KEY and REGION values in app.py:

      API_KEY = "your-api-key"
      REGION = "your-region"

### Usage
1.Start the server:

      python app.py

2.Open a web browser and navigate to:

    http://localhost:5000

3.Click "Start Listening" and begin speaking in English

4.Your speech will be transcribed and translated to the selected language

# AI-Powered Medical Assistant

An intelligent medical assistant application that seamlessly integrates voice and chat interactions, providing personalized healthcare support.

## Features

- Hybrid Voice & Chat AI Interaction with natural language processing
- Smart Medication Reminders and management
- Doctor Visit Reminders & Appointment Management
- Medical Timers & Task Management
- Personalized Health Insights
- Real-Time Functionality & Live Updates

## Technologies Used

- Backend: Python (Flask)
- Frontend: HTML, CSS, JavaScript
- AI Integration: Gemini API
- Text-to-Speech: Google Cloud TTS
- Real-Time Updates: WebSockets (Flask-SocketIO)
- Database: SQLite

## Setup Instructions

### Prerequisites

- Python 3.8 or higher
- pip (Python package manager)
- Google Cloud account with API access for:
  - Gemini API (for AI processing)
  - Google Cloud Text-to-Speech API
- Modern web browser (Chrome, Firefox, Edge recommended)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/medical-assistant-ai.git
   cd medical-assistant-ai
2. **Create and activate a virtual environment**

       # On Windows
        python -m venv venv
        venv\Scripts\activate

        # On macOS/Linux
        python3 -m venv venv
        source venv/bin/activate
3. **Install dependencies**

        pip install -r requirements.txt
4. **Set up Google Cloud credentials**
- Create a project in the Google Cloud Console
- Enable the Gemini API and Text-to-Speech API
- Create an API key for Gemini
- Create a service account and download credentials JSON file for Text-to-Speech
- Rename the credentials file to google_credentials.json and place it in the project root

## Configuration
1. Environment variables

Create a .env file in the project root:

    GEMINI_API_KEY=your_gemini_api_key_here
    GOOGLE_APPLICATION_CREDENTIALS=path_to_your_google_credentials.json
    FLASK_SECRET_KEY=your_random_secret_key

2. Database setup
   
The application uses SQLite and will automatically create a database file when first run.

## Running the Application
1. Start the Flask server

        # Development mode
        flask run --debug
        
        # Production mode
        gunicorn app:app
2. Access the application
   
Open your web browser and navigate to:

    http://127.0.0.1:5000

## First-time Setup

1.Create an account

- Register a new account using the registration form
- Log in with your credentials


2.Complete your medical profile

- Fill out your medical profile with required information:

  - Height
  - Weight
  - Blood type
  - Allergies (if any)
  - Medical conditions (if any)
  - Emergency contact




3. Enable permissions

- Allow microphone access if you plan to use voice commands
- Allow notifications for medication and appointment reminders

## Voice Commands
After setup, you can use voice commands like:

- "Add new medication"
- "Schedule an appointment with Dr. Smith"
- "Set a timer for 20 minutes"
- "What is my next appointment?"
