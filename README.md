Real-time Voice-Activated Customer Support Bot
This Python-based project is a real-time voice assistant for customer support automation, capable of listening to voice input, transcribing speech to text, responding to customer queries, and vocalizing the responses. It uses:

🎙️ speech_recognition for real-time speech-to-text

🗣️ pyttsx3 for text-to-speech responses

🧠 A simple rule-based logic for common support topics

📌 Features
✅ Real-time voice input via microphone

🧾 Speech-to-text transcription using Google Speech Recognition

🔄 Automated responses to common customer support queries

🗣️ Converts text response into speech using pyttsx3

🔊 Robust to background noise using ambient adjustment

🛠️ Requirements
Python 3.6+

Required libraries:

pip install SpeechRecognition pyttsx3 pyaudio
If pyaudio fails to install on Windows, try:


pip install pipwin
pipwin install pyaudio



Clone the repository:


git clone https://github.com/hemadharshini/customer-support-voicebot.git
cd customer-support-voicebot
Run the Python script:


python voice_support_bot.py
Speak into your microphone with queries like:

“Tell me my account details”

“Connect me to the support team”

“What about my payment?”

The bot will recognize your voice, display the transcribed query, generate a response, and speak it out loud.

🧠 Core Logic
python

def automated_response(user_query):
    if "account details" in user_query.lower():
        return "I can help you with your account details."
    elif "support team" in user_query.lower():
        return "Our support team is here to help you."
    elif "payment" in user_query.lower():
        return "I can assist you with payment-related queries."
    else:
        return "I'm here to help with any other questions."
💡 Example Interaction
vbnet
Real-time SRT System for Customer Support Automation
Listening...
User: I want to talk to the support team
Bot: Our support team is here to help you.

🔐 Limitations
Basic keyword matching (no NLP or AI-based intent detection)

Internet is required for Google Speech API

No user authentication or context tracking

🧱 Future Enhancements
Add NLP-based intent detection (e.g., using Hugging Face Transformers)

Support multilingual queries

Log user queries for analysis

Create a GUI using Tkinter or web interface with Flask

📄 License
This project is licensed under the MIT License. You are free to use and modify it for personal or commercial purposes.

