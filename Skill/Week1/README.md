# Week 1 – First LLM API Call

## Project Overview
This project demonstrates how to make a first Large Language Model (LLM) API call using Python and Google's Gemini API.

The program sends a prompt to the Gemini model and displays the AI-generated response.

## Technologies Used
- Python
- Google Gemini API
- Google Generative AI SDK
- python-dotenv

## Project Files
- `main.py` – Main Python program for making the Gemini API call.
- `requirements.txt` – Required Python libraries.
- `.gitignore` – Specifies files that should not be uploaded to GitHub.

## Setup Instructions

1. Install Python.
2. Install the required libraries:

```bash
pip install -r requirements.txt
```

3. Configure your Gemini API key in a local `.env` file:

```env
GEMINI_API_KEY=your_api_key_here
```

4. Run the program:

```bash
python main.py
```

## Learning Outcomes
- Understanding Large Language Models.
- Connecting Python applications with the Gemini API.
- Sending prompts and receiving AI-generated responses.
- Managing API keys securely.

## Security Note
Never upload your `.env` file or API keys to GitHub.
