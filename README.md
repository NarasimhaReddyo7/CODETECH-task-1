Name : KOTA UGRA NARASIMHA REDDY
Company:CODETECH IT SOLUTIONS
ID :CT6WDS2240
Domain:Machine Learning
Duration :october to December 2024
Mentor :NEELA SANTOSH KUMAR

OVER VIEW OF THE PROJECT
**1. Project Title**
Text-to-Speech Conversion Web Application

**2. Introduction**
The Text-to-Speech (TTS) Conversion Web Application is designed to convert user-entered text into spoken audio. It is a simple, interactive, and dynamic application that allows users to:

Enter text in various languages.
Select the gender of the voice (male or female).
Hear the synthesized speech directly on the webpage.
The application leverages modern web technologies alongside Python libraries for natural-sounding speech generation.

**3. Objectives**
The main objectives of this project are:

To provide an easy-to-use web interface for converting text to speech.
To allow users to select different languages and voice preferences (male/female).
To ensure the speech can be played directly on the webpage without downloading.
To handle text-to-speech operations efficiently on both the client and server side.
**4. Technologies Used**
4.1. Frontend
HTML5: For creating the structure of the web page.
CSS3: For styling the interface.
JavaScript (Vanilla JS): For dynamically handling user interactions and making asynchronous requests to the server.
4.2. Backend
Python: The core programming language used to implement the server-side logic.
Flask: A lightweight web framework used for hosting the application and handling requests.
Flask-CORS: Used to enable Cross-Origin Resource Sharing for better communication between the frontend and backend.
4.3. Text-to-Speech Libraries
gTTS (Google Text-to-Speech): For generating female voice output in various languages.
pyttsx3: A library that provides offline text-to-speech functionality and is used for male voice synthesis.
**5. System Design**
5.1. Architecture
The application follows a client-server architecture:

The user interacts with the web page to enter text, choose a language, and select a voice gender.
The frontend sends the user’s input to the Flask server via a POST request.
The Flask server processes the request, converts the text to speech using either gTTS or pyttsx3, and streams the audio back to the frontend.
The frontend plays the audio using an embedded <audio> player.
5.2. Flow Diagram
User Inputs Text → Selects Language & Gender → Clicks "Convert to Speech".
Frontend sends a POST request with the user’s input to the backend.
Flask server generates speech audio using TTS libraries.
Audio is streamed back to the frontend and played on the webpage.
**6. Features**
Multilingual Support:
The application supports multiple languages, including English, Spanish, and French.
Gender Selection:
Male Voice: Generated using pyttsx3 (offline).
Female Voice: Generated using gTTS (requires internet connection).
Live Audio Playback:
Users can hear the synthesized speech directly on the webpage.
Error Handling:
Provides user-friendly error messages for invalid input or system errors.
**7. Implementation**
7.1. User Interface
The UI is built using HTML and CSS, featuring:

A text area for input.
Dropdown menus for selecting language and voice gender.
A button to trigger the conversion.
An audio player to play the generated speech.
7.2. Backend Processing
The Flask server handles:

Validation of user input.
Selection of the appropriate TTS library based on the user’s choice.
Audio file generation and streaming back to the client.
**8. Challenges Faced**
Voice Selection:

pyttsx3 sometimes does not provide a proper male voice on some operating systems.
Solution: Fallback to the default voice if a male voice is unavailable.
Real-Time Playback:

Streaming the audio file to the frontend without requiring a download.
Solution: Used Flask’s send_file method with audio/mpeg mimetype.
Multilingual Support:

Some languages were not supported by pyttsx3.
Solution: Used gTTS for more reliable language support.

**9. Conclusion**
The Text-to-Speech Conversion Web Application successfully provides a seamless user experience for generating and playing synthesized speech. It effectively combines frontend and backend technologies to handle user inputs and real-time audio playback. This project demonstrates the potential of integrating machine learning libraries like gTTS and pyttsx3 with modern web frameworks for practical applications.

![Screenshot 2024-12-06 231047](https://github.com/user-attachments/assets/b3fc38fb-37c4-4b50-8f51-cf38ebcbcdc2)
![Screenshot 2024-12-06 231023](https://github.com/user-attachments/assets/6866314b-9aac-4b6c-ac8f-76867b69725e)
