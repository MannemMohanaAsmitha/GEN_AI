WEEK 2 – Provider-Agnostic LLM Client
Aim
To develop a provider-agnostic LLM client using Python that supports multiple AI providers, including Google Gemini API and a locally running Ollama model, through a common interface.

Technologies Used
Python
Google Gemini API
Ollama
Qwen 2.5 (0.5B Model)
Requests
Python Virtual Environment
Tools Used
Python
Visual Studio Code
Gemini API
Ollama
Folder Structure
WEEK2/
├── main.py
├── llm_client.py
├── test_client.py
├── requirements.txt
├── .env
├── Modelfile
└── README.md
Installation Steps
Install Python on your system.

Install Ollama on your system.

Open the WEEK2 folder in VS Code.

Create and activate a virtual environment:

python -m venv myenv
myenv\Scripts\activate
Install the required packages:
pip install -r requirements.txt
Download the Ollama model:
ollama pull qwen2.5:0.5b
Create a .env file and add your Gemini API key:
GEMINI_API_KEY=your_api_key_here
Note: Never upload your actual API key to GitHub.

Execution Steps
Run the following command in the terminal:

python main.py
The program starts and asks the user to select an AI provider.
Select Gemini or Ollama.
Enter a prompt or question.
The prompt is sent to the selected LLM provider.
The selected model generates a response.
The response is displayed in the terminal.
To test the application, run:

python -m unittest test_client.py
Expected Output
The program accepts a prompt and generates an AI response using either Gemini or Ollama.

Example:

Input:

Explain Artificial Intelligence.
Output:

Artificial Intelligence is a technology
that enables machines to perform tasks
that normally require human intelligence.
Result
Successfully developed a provider-agnostic LLM client using Python that supports both Google Gemini API and the locally running Ollama model through a common interface.
