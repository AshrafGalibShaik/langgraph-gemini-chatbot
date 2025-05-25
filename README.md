# LangGraph Gemini Chatbot

A simple chatbot built using [LangGraph](https://github.com/langchain-ai/langgraph) and Gemini (Google Generative AI) via `langchain-google-genai`.

## Features

- Uses LangGraph for state management  
- Integrates Gemini (via `langchain_google_genai`)  
- Streamed chatbot responses  
- Easy interactive CLI loop  

## Getting Started

### 1. Clone the Repo

```bash
git clone https://github.com/yourusername/langgraph-gemini-chatbot.git
cd langgraph-gemini-chatbot
````

### 2. Create and Activate a Virtual Environment (Recommended)

**Linux/macOS:**

```bash
python3 -m venv venv
source venv/bin/activate
```

**Windows (PowerShell):**

```powershell
python -m venv venv
.\venv\Scripts\Activate.ps1
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Setup Environment Variables

Copy the example environment file:

```bash
cp .env.example .env
```

Edit `.env` and replace with your Google API key:

```env
GOOGLE_API_KEY=your_google_api_key_here
```

> Make sure you have a valid Google API key with access to Gemini or Google Generative AI.

### 5. Run the Chatbot

```bash
python main.py
```

### 6. Using the Chatbot

* Type your message after the prompt (`User:`)
* The assistant will reply interactively
* To exit the chat, type `quit`, `exit`, or `q`

### 7. Troubleshooting & Notes

* If the chatbot doesn’t respond or errors occur, check your API key and `.env` file
* Streaming responses may print incrementally in the console
* Customize chatbot logic by editing `chatbot_node` in `main.py`


