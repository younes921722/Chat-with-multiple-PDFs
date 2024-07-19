# Chat with your PDFs using Hugging Face LLMs and Embeddings

This project demonstrates how to leverage Retrieval-Augmented Generation (RAG) to create a chatbot that interacts with PDF documents. By combining Hugging Face's language models and embeddings with the help of LangChain, we can extract relevant information from PDFs and generate context-aware responses. The user-friendly interface is built using Streamlit.

## Features

- **PDF Text Extraction:**
  - The project extracts text from PDF documents, making it accessible for further processing.
- **Embeddings for Retrieval:**
  - We use embeddings (vector representations) to retrieve relevant information from the PDFs.
- **Hugging Face Language Models:**
  - Hugging Face provides powerful pre-trained language models. We incorporate them for response generation.
- **Streamlit Interface:**
  - The project includes a Streamlit app, allowing users to interact with the chatbot easily.

## Installation

### Requirements

Before you begin, ensure you have Python 3.7 or higher installed. Then, follow these steps:

1. **Create a Virtual Environment (Recommended):**
   - It's a good practice to create a virtual environment to isolate dependencies for your project. You can use `venv` or `conda`:
     ```bash
     # Using venv
     python -m venv myenv
     source myenv/bin/activate

     # Using conda
     conda create --name myenv python=3.7
     conda activate myenv
     ```

2. **Install Required Packages:**
   - Navigate to your project directory and install the necessary packages from `requirements.txt`:
     ```bash
     pip install -r requirements.txt
     ```

3. **Set Up Your Hugging Face API Token:**
   - To access Hugging Face's models, you'll need an API token.
   - Create a `.env` file in your project directory (if it doesn't exist).
   - Add your Hugging Face API token to the `.env` file:
     ```
     HUGGINGFACE_TOKEN=your-api-token-here
     ```

### Running the Project

Now that everything is set up, you can run the Streamlit app:

```bash
streamlit run app.py
