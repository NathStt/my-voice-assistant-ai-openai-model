# 🎙️ AI Voice Assistant Chatbot

An AI-powered voice assistant chatbot that converts speech to text, processes it with an AI model, and responds with synthesized speech.

This project demonstrates how to build a full voice interaction pipeline using Python, APIs, and a web interface.

---

## 🚀 Features

* 🎤 Speech-to-Text (STT)
* 🧠 AI Chat Processing (LLM)
* 🔊 Text-to-Speech (TTS)
* 🌐 Web interface using Flask
* ⚡ Real-time voice interaction flow

---

## 🧠 How It Works

The system follows a simple pipeline:

1. User speaks into the microphone
2. Audio is sent to backend (`worker.py`)
3. Speech is converted to text (STT API)
4. Text is processed by AI model (OpenAI / Watson)
5. Response text is converted to speech (TTS API)
6. Audio is returned and played to the user

---

## 🏗️ Project Structure

```
chatapp-with-voice-assistant/
│
├── server.py          # Flask backend server
├── worker.py          # Core logic (STT, AI, TTS)
├── templates/         # HTML frontend
├── static/            # JS, CSS assets
├── models/            # AI model configs (if any)
├── certs/             # SSL certificates (if used)
├── requirements.txt   # Python dependencies
└── README.md
```

---

## ⚙️ Tech Stack

* Python 3.11
* Flask
* OpenAI API (LLM)
* IBM Watson Speech-to-Text
* IBM Watson Text-to-Speech
* HTML / CSS / JavaScript

---

## 🧪 Installation

### 1. Clone the repository

```bash
git clone https://github.com/NathStt/my-voice-assistant-ai-openai-model.git
cd my-voice-assistant-ai-openai-model
```

### 2. Create virtual environment

```bash
python3 -m venv my_env
source my_env/bin/activate   # Mac/Linux
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 Environment Variables

You need API keys for:

* OpenAI
* IBM Watson STT
* IBM Watson TTS

Set them like this:

```bash
export OPENAI_API_KEY=your_key_here
```

(Repeat for other APIs)

---

## ▶️ Run the Application

```bash
python server.py
```

Then open your browser:

```
http://localhost:5000
```

---

## 📸 Demo Flow

1. Click record
2. Speak a sentence
3. AI processes your request
4. Response is spoken back

---

## ⚠️ Notes

* Ensure microphone permissions are enabled in your browser
* Internet connection is required for API calls
* Do not commit API keys to GitHub

---

## 📌 Future Improvements

* Add streaming voice responses
* Improve latency
* Add conversation memory
* Deploy to cloud (AWS / GCP)
* Add authentication

---

## 👤 Author

Built by NathStt as part of an AI engineering assignment.

---

## 📄 License

This project is for educational purposes.
