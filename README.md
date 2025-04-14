# LLM Video Avatar Training Program

This repository contains the code for the **LLM Video Avatar Training Program**, designed to enhance the training of undergraduate nursing students by simulating realistic patient interactions through AI-driven avatars. The program leverages the power of AI to simulate clinical scenarios, helping students engage in meaningful, real-time interactions for a more effective learning experience.

## Features
- **Multi-Modal Interactions:** Supports various interaction modes including text-to-text, text-to-audio, audio-to-audio, video-to-audio, and video-to-video.
- **Adaptive Learning:** Utilizes GPT-4 to tailor responses dynamically based on student input, simulating varied clinical scenarios.
- **Scalable and Modular:** Developed first in Google Colab for ease of use and then transitioned to Jupyter Notebook with an HTML interface for smooth deployment and integration into different systems.

## Academic Paper 
[Conversational LLM Video Avatar Training for Healthcare Students](https://github.com/user-attachments/files/17150059/Gaetano_MIDI_conference_deadline_august_21.docx)

## Prerequisites
Before running the project, make sure you have the following:

- **Python 3.x** installed: Ensure Python 3.x (preferably version 3.7 or higher) is installed on your system. You can download and install Python from [python.org](https://www.python.org/downloads/).
- **Jupyter Notebook**: Install Jupyter Notebook to run and interact with the code. If you don’t have it installed, follow these steps:
    1. Install Jupyter Notebook via pip (Python package manager). Open your terminal or command prompt and run:
       ```bash
       pip install notebook
       ```
    2. Once installed, you can run the following command to start Jupyter:
       ```bash
       jupyter notebook
       ```

- **Required API Services**: The project utilizes the following APIs:
    - **D-ID API**: Provides facial animation services to create dynamic video avatars.
    - **OpenAI API**: Used to generate AI-driven responses based on student input.

    Make sure you have an account with both services and the necessary API keys. 

## Add Your API Keys

Follow these steps to obtain and configure your API keys:

### D-ID API:
1. Go to the [D-ID website](https://www.d-id.com/) and sign up for an account.
2. After logging in, navigate to the "API" section of the D-ID dashboard.
3. Generate a new API key by following the on-screen instructions.
4. Copy your API key.

### OpenAI API:
1. Visit the [OpenAI API platform](https://platform.openai.com/).
2. Sign up for an account if you don’t already have one.
3. Once logged in, navigate to the "API" section to generate an API key.
4. Copy your OpenAI API key.

### Adding API Keys to Your Project:
1. **Create a `.env` file**: In the root directory of your project, create a file named `.env`.
2. **Add the keys**: Open the `.env` file and add the following lines, replacing `your_did_api_key_here` and `your_openai_api_key_here` with the keys you obtained:
3. **Install Python-dotenv**: To load the keys from the `.env` file, you’ll need the `python-dotenv` package. Install it by running:
```bash
pip install python-dotenv
```
4.Load the keys in your project: In your project code, add the following to load the API keys:
```python
from dotenv import load_dotenv
import os

load_dotenv()

did_api_key = os.getenv("DID_API_KEY")
openai_api_key = os.getenv("OPENAI_API_KEY")
```

## Running the Project
1. Open a terminal and navigate to the directory where you’ve downloaded or cloned the repository.
2. Start Jupyter Notebook by typing the following command in your terminal:
   ```bash
   jupyter notebook
   ```
3. In the Jupyter Notebook interface, open the .ipynb file corresponding to the LLM Video Avatar Training Program.
4. Follow the instructions within the notebook to run the program. The cells are designed to guide you through each step.
