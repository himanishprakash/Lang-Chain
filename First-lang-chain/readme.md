# Script GPT Creator

## Overview

Script GPT Creator is a web application built with Streamlit that allows users to input a prompt and generate a YouTube video script. It leverages OpenAI's language models via LangChain to generate a title and script based on the prompt and incorporates Wikipedia research to provide context. The application also stores conversation history for the title and script using memory buffers, allowing for better context retention during the session.

## Features
- **Prompt Input**: Users can input any topic for which they'd like to generate a YouTube video script.
- **Dynamic Video Title Generation**: The app creates a YouTube video title based on the user's input using an OpenAI model.
- **Wikipedia Research**: The app fetches relevant information from Wikipedia to provide context for the topic.
- **Video Script Generation**: The app generates a complete video script using both the video title and the Wikipedia research.
- **Memory Buffers**: Conversation memory is used to store the chat history, allowing the system to remember and reference past interactions.
- **Expander Features**: The app displays the history of generated titles, scripts, and the Wikipedia research within expandable sections for better navigation and transparency.

## Prerequisites

- Python 3.7 or higher
- OpenAI API key
- Streamlit
- LangChain
- WikipediaAPIWrapper
- dotenv

## Installation

1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd script-gpt-creator
   ```

2. Create a virtual environment and activate it:
   ```bash
   python3 -m venv venv
   source venv/bin/activate   # On Windows use: venv\Scripts\activate
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up the OpenAI API key:
   - Create a `.env` file in the project root directory.
   - Add your OpenAI API key:
     ```
     OPENAI_API_KEY=<your_openai_api_key>
     ```

## Usage

1. Run the Streamlit application:
   ```bash
   streamlit run app.py
   ```

2. Open the web app in your browser. You'll be presented with a text input box where you can enter your desired prompt.

3. After submitting the prompt, the app will generate a YouTube video title and video script based on the prompt, incorporating research from Wikipedia for context.

4. The results will be displayed on the screen, with the following additional information accessible via expandable sections:
   - **Title History**: Shows previously generated video titles.
   - **Script History**: Shows the previous video scripts.
   - **Wikipedia Research**: Displays the research fetched from Wikipedia for the prompt.

## Project Structure

- `app.py`: Main script for the Streamlit app.
- `requirements.txt`: List of required packages for the project.
- `.env`: Environment file for storing the OpenAI API key (not included in the repository).

#

