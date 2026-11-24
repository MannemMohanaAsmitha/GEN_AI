# WEEK 2 – Provider-Agnostic LLM Client

## Aim

To develop a provider-agnostic LLM client using Python that supports multiple AI providers, including Google Gemini API and a locally running Ollama model, through a common interface.

## Technologies Used

- Python
- Google Gemini API
- Ollama
- Qwen 2.5 (0.5B Model)
- Requests
- Python Virtual Environment

## Tools Used

- Python
- Visual Studio Code
- Google Gemini API
- Ollama

## Folder Structure

```text
WEEK2/
├── main.py
├── llm_client.py
├── test_client.py
├── requirements.txt
├── .env
├── Modelfile
└── README.md
```

## Installation Steps

1. Install Python on your system.
2. Install Ollama on your system.
3. Open the `WEEK2` folder in Visual Studio Code.
4. Create a Python virtual environment:

   ```bash
   python -m venv myenv
   ```

5. Activate the virtual environment:

   ```bash
   myenv\Scripts\activate
   ```

6. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

7. Download the Ollama model:

   ```bash
   ollama pull qwen2.5:0.5b
   ```

8. Create a `.env` file in the project folder and add your Gemini API key:

   ```env
   GEMINI_API_KEY=your_api_key_here
   ```

**Note:** Never upload your actual Gemini API key or `.env` file to GitHub. Add `.env` to your `.gitignore` file.

## Execution Steps

Run the following command in the VS Code terminal:

```bash
python main.py
```

### Working Procedure

1. The program starts and asks the user to select an AI provider.
2. Select either **Google Gemini** or **Ollama**.
3. Enter a prompt or question.
4. The prompt is sent to the selected LLM provider.
5. The selected AI model processes the prompt and generates a response.
6. The generated response is displayed in the terminal.

## Testing

To test the application, execute:

```bash
python -m unittest test_client.py
```

This command runs the unit tests to verify the functionality of the LLM client.

## Expected Output

The application accepts a prompt and generates an AI response using either Google Gemini or the locally running Ollama model.

**Example:**

**Input:**

```text
Explain Artificial Intelligence.
```

**Output:**

```text
Artificial Intelligence is a technology that enables
machines to perform tasks that normally require
human intelligence.
```

## Result

Successfully developed a provider-agnostic LLM client using Python that supports Google Gemini API and a locally running Ollama model through a common interface. The application allows users to switch between different AI providers without changing the main application code.
