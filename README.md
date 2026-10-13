# 🎙️ AI Voice Assistant

A voice assistant you talk to in the browser. You record or upload audio, Distil-Whisper on Groq transcribes it, and Llama 3 70B on Groq writes the reply. Both the transcription and the answer are shown side by side in a Gradio interface.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Gradio](https://img.shields.io/badge/Gradio-F97316?style=flat-square&logo=gradio&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-F55036?style=flat-square&logoColor=white)
![Llama 3](https://img.shields.io/badge/Llama_3_70B-0467DF?style=flat-square&logo=meta&logoColor=white)
![Whisper](https://img.shields.io/badge/Distil--Whisper-412991?style=flat-square&logoColor=white)

## ✨ Features
- 🎤 Record from the microphone or upload an audio file (mp3, mp4, mpeg, mpga, m4a, wav, webm)
- 📝 Speech to text with `distil-whisper-large-v3-en` on Groq
- 🤖 Replies from `llama3-70b-8192` on Groq
- 🔐 API key read from the environment or a `.env` file, with a clear message in the UI when it is missing

## 🚀 Run locally

```bash
git clone https://github.com/ziauldin/ai-voice-assistant.git
cd ai-voice-assistant
pip install -r requirements.txt
cp .env.example .env   # then put your key in .env: GROQ_API_KEY=...
python app.py
```

Gradio prints a local URL (usually http://127.0.0.1:7860). Get a free API key at [console.groq.com](https://console.groq.com).

## 🛠️ Tech stack
Python · Gradio · Groq API · Llama 3 70B · Distil-Whisper · NumPy · SoundFile
