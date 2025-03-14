# Personal AI Voice Assistant

This is a **Flask-based AI Voice Assistant** that takes voice input, processes it using **Google's Generative AI (Gemini 1.5 Pro)**, and responds with an AI-generated answer. The project also maintains a conversation history and provides speech synthesis for AI responses.

## Features
- 🎙 **Voice Input:** Uses Web Speech API for speech recognition.
- 🤖 **AI Responses:** Generates intelligent responses using Google's Gemini model.
- 📜 **Conversation History:** Stores and displays user-AI interactions.
- 🔊 **Text-to-Speech:** Reads AI-generated responses aloud.
- 🌐 **Flask Web App:** Simple front-end UI for user interaction.

## Project Structure
```
Personal-AI-Voice-Assistant/
│── app.py                  # Flask server with AI response logic
│── requirements.txt         # List of dependencies
│── templates/
│   └── index.html           # Front-end UI
│── static/
│   ├── style.css            # CSS for styling
│   └── script.js            # JavaScript for voice interaction
│── README.md                # Project documentation
```

## Setup & Installation
### 1️⃣ Clone the Repository
```bash
git clone https://github.com/VoonaSriraj/Personal-AI-Voice-Assistant.git
cd Personal-AI-Voice-Assistant
```

### 2️⃣ Create a Virtual Environment
```bash
python -m venv venv
source venv/bin/activate  # For macOS/Linux
venv\Scripts\activate     # For Windows
```

### 3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 4️⃣ Set Up Google Generative AI API Key
- Replace `YOUR_API_KEY` in `app.py` with your actual Google API Key:
```python
os.environ["GOOGLE_API_KEY"] = "YOUR_API_KEY"
```

### 5️⃣ Run the Flask App
```bash
python app.py
```
- The app will start running at **http://127.0.0.1:5000/**

## Usage
1. Click on the **"🎤 Speak Now"** button.
2. Speak your query.
3. The AI will process the query and respond.
4. The conversation history will be displayed below.

## Troubleshooting
- **ModuleNotFoundError: No module named 'google.generativeai'**
  - Run: `pip install google-generativeai`
- **TemplateNotFound: index.html**
  - Ensure `index.html` is inside the `templates/` folder.
- **Git Error: "src refspec main does not match any"**
  - Run:
    ```bash
    git branch -M main
    git push -u origin main
    ```

## Dependencies
- Python 3.10+
- Flask
- Google Generative AI SDK
- Web Speech API (for speech recognition)

## License
This project is **MIT Licensed**. Feel free to modify and use it.

---
### Author: [Sriraj Voona](https://github.com/VoonaSriraj)

