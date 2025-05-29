

# Gemini Multi-Turn Chat 🤖

A simple interactive console chatbot using the **Google Gemini API** (via the `google-genai` Python SDK). This script demonstrates multi-turn conversations with context retention and adjustable model parameters like temperature.

---

## 🧠 What It Does

- Initializes a Gemini chat session using `gemini-1.5-flash` (or `gemini-2.0-flash`).
- Prompts the user for multiple inputs and sends them as a conversation to Gemini.
- Preserves context across turns so the model can "remember" earlier messages.
- Allows temperature configuration to adjust creativity of responses.
- Outputs the model’s final response to the console.

---

## 🛠️ Setup Instructions

### 1. Clone the repository
```bash
git clone https://github.com/<your-username>/gemini-multi-turn-chat.git
cd gemini-multi-turn-chat
````

### 2. Create a virtual environment (optional but recommended)

```bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

**Or install directly:**

```bash
pip install google-genai python-dotenv
```

### 4. Add your Google API key

Create a `.env` file in the project root with:

```
GOOGLE_API_KEY=your-google-api-key-here
```

> ⚠️ **Do not commit your API key to GitHub.**

---

## 🚀 Run the Script

```bash
python gemini_chat.py
```

The script will:

1. Ask for a temperature (optional, default is 0.7).
2. Prompt for your first question.
3. Send it to Gemini.
4. Prompt for a second message (follow-up).
5. Send both as part of the chat and display the final response.

---

## 🔧 Optional Features

* Supports extended conversations (3 or more turns).
* Lets you adjust temperature at runtime for more focused or more creative answers.

---



