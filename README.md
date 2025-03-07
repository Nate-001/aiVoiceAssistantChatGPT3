# AI Voice Assistant with ChatGPT

## Description
This project is an AI-powered voice assistant that uses OpenAI's GPT-3.5 model for natural language processing, combined with speech-to-text and text-to-speech capabilities. It allows users to interact with an AI assistant using voice commands or text input.

## Features
- Speech-to-text conversion
- Text-to-speech conversion with voice selection
- Natural language processing using OpenAI's GPT-3.5 model
- Web-based interface for interaction

## Technologies Used
- Python
- Flask (Web Framework)
- OpenAI API
- Watson Speech-to-Text API
- Watson Text-to-Speech API
- HTML/CSS/JavaScript (Frontend)

## Setup and Installation
1. Clone the repository
2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```
3. Set up your OpenAI API key as an environment variable:
   ```
   export OPENAI_API_KEY=your_api_key_here
   ```
4. Run the server:
   ```
   python server.py
   ```

## Usage
1. Open a web browser and navigate to `http://localhost:8000`
2. Use the interface to either type a message or click the microphone icon to speak
3. The AI assistant will process your input and respond with both text and speech

## Docker Support
A Dockerfile is included for containerization. To build and run the Docker container:

1. Build the Docker image:
   ```
   docker build -t ai-voice-assistant .
   ```
2. Run the container:
   ```
   docker run -p 8000:8000 ai-voice-assistant
   ```

## API Endpoints
- `/`: Serves the main HTML page
- `/speech-to-text`: POST endpoint for converting speech to text
- `/process-message`: POST endpoint for processing user messages and generating AI responses

## Notes
- This project uses Watson APIs for speech-to-text and text-to-speech conversion. Make sure you have the necessary credentials and access.
- The OpenAI API key is required for the natural language processing capabilities.

## Future Improvements
- Add user authentication
- Implement conversation history
- Enhance the UI for a better user experience
- Add support for multiple languages

## Contributors
- Nate-001
