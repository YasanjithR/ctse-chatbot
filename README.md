# CTSE Chatbot

A chatbot for software engineering students that answers questions about lecture material using RAG (Retrieval Augmented Generation) with OpenAI and LangChain.

## Features

- Question answering based on CTSE lecture content
- Uses OpenAI embeddings and LLM for accurate responses
- PDF document ingestion and chunking
- Vector similarity search for relevant context retrieval

## Setup

1. Clone this repository
2. Create a virtual environment:
   ```
   python -m venv venv
   ```
3. Activate the virtual environment:
   - Windows: `venv\Scripts\activate`
   - macOS/Linux: `source venv/bin/activate`
4. Install required packages:
   ```
   pip install -r requirements.txt
   ```
5. Place your lecture PDFs in the `documents` folder
   - The main lecture file should be named `ctse.pdf`
6. Set your OpenAI API key:
   - Create a `.env` file with: `OPENAI_API_KEY=your_api_key_here`
   - Or set it directly in your environment variables

## Usage

1. Run the Jupyter notebook:
   ```
   jupyter notebook ctse_chatbot.ipynb
   ```
2. Execute all cells in the notebook
3. Interact with the chatbot by typing questions
4. Type "exit" to end the session

## Project Structure

- `ctse_chatbot.ipynb`: Main Jupyter notebook containing the chatbot implementation
- `documents/`: Folder for storing lecture PDFs
- `requirements.txt`: List of required Python packages
- `.gitignore`: Configuration to prevent sensitive data from being committed

## Requirements

- Python 3.6+
- OpenAI API key
- Lecture materials in PDF format 