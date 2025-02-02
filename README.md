# Chat With AI

## Overview

Chat With AI is an advanced chatbot application designed to handle multiple use cases, including text summarization, content generation, code generation, sentiment analysis, translation, question answering, and more. The chatbot leverages **Streamlit** for the frontend and **LangChain** with **Groq LLM** for AI-based conversational capabilities.

## Features

- Multi-purpose AI chatbot with various use cases
- User-friendly interface using Streamlit
- Supports natural language processing for multiple domains
- Uses **LangChain** and **Groq LLM** for response generation
- Secure environment variable support for API keys

## Technologies Used

- **Python** (Core programming language)
- **Streamlit** (Web interface)
- **LangChain** (AI model handling)
- **Groq LLM** (Language Model)
- **Dotenv** (Environment variable management)

## Installation

1. Clone this repository:
   ```sh
   git clone https:https://github.com/JISHUBISHI/chat_with_llama3.3
   cd chat-with-ai
   ```
2. Create a virtual environment (optional but recommended):
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```
3. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
4. Set up your API key:
   - Create a `.env` file in the root directory and add:
     ```sh
     GROQ_API_KEY="your_api_key_here"
     ```
   - Ensure your API key is loaded securely within the script.

## Usage

1. Run the application:
   ```sh
   streamlit run main.py
   ```
2. Select a use case from the dropdown menu.
3. Enter the input text and additional details as required.
4. Click the "Generate Response" button to receive AI-generated output.

## Environment Variables

To keep your API key secure, you can set an environment variable instead of hardcoding it:
```sh
export GROQ_API_KEY="your_api_key_here"
```
Then, modify the code to use:
```python
import os
from dotenv import load_dotenv

load_dotenv()
api_key = os.getenv("GROQ_API_KEY")
```

## Example Use Cases

- **Summarization:** "Summarize this article in a concise paragraph."
- **Content Generation:** "Write a short story about a space adventure."
- **Code Generation:** "Generate a Python function for sorting a list."
- **Sentiment Analysis:** "Analyze the sentiment of this customer review."
- **Translation:** "Translate this text from English to French."
- **Question Answering:** "What are the key principles of machine learning?"

## Author

Agnik Bishi

