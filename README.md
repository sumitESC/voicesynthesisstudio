# Voice Synthesis Studio

![Project Screenshot](https://raw.githubusercontent.com/sumitESC/Voice-Synthesis-Studio/main/screenshot.png)

A Dockerized web application for text-to-speech conversion using IBM Watson's Text-to-Speech API.

## Features

- 🎤 40+ languages and 100+ neural/expressive voices
- 🔊 Real-time speech generation with IBM Watson
- 🐳 Docker support for easy deployment
- 📝 Character counter with visual limit indicator
- 🎧 Built-in audio player with custom controls
- ⬇ Download audio as WAV files
- 📊 Usage statistics tracking

## Quick Start with Docker

### 1. Clone the repository
```bash
git clone https://github.com/sumitESC/Voice-Synthesis-Studio.git
cd Voice-Synthesis-Studio
```

### 2. Build and run with Docker
```bash
docker build -t voice-synthesis .
docker run -p 3000:3000 -e VITE_WATSON_API_KEY="your_api_key" -e VITE_WATSON_SERVICE_URL="your_service_url" -e VITE_WATSON_INSTANCE_ID="your_instance_id" voice-synthesis

Open http://localhost:3000 in your browser
```
### Getting IBM Watson Credentials

1.Go to IBM Cloud Text-to-Speech
2.Create a service instance (Lite plan is free)
3.After creation, go to "Manage" tab and copy:
-API Key
-Service URL (e.g., https://api.au-syd.text-to-speech.watson.cloud.ibm.com)
-Instance ID (from the API endpoint URL)
