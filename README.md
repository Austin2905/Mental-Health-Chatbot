# Baymax: Your Personal Healthcare Assistant

Baymax is a conversational healthcare assistant application built using LangChain, Streamlit, and various NLP tools. This application allows users to interact with a large language model (LLM) to get answers to their healthcare-related questions by analyzing and retrieving information from PDF documents.

## Features

- **PDF Document Loader**: Load PDF files from a specified directory.
- **Text Chunking**: Split large text documents into manageable chunks.
- **Embeddings**: Use HuggingFace embeddings for semantic search.
- **Vector Store**: Store document embeddings using FAISS for fast retrieval.
- **Conversational Agent**: Engage in a conversation with a healthcare assistant powered by the LLaMA model.
- **Streaming Responses**: Get responses from the LLM in real-time.
- **Memory Buffer**: Maintain conversation history to provide context-aware responses.

## Prerequisites

Ensure you have the following installed:

- Python 3.7 or higher
- `pip` (Python package installer)
- Download the Llama quantisized model: llama-2-7b-chat.ggmlv3.q4_0.bin from https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/tree/main

## Installation

1. **Clone the Repository**:

    ```sh
    git clone https://github.com/Austin2905/Mental-Health-Chatbot.git
    cd Baymax
    ```

2. **Set Up Virtual Environment** (optional but recommended):

    ```sh
    python -m venv venv
    source venv/bin/activate    # On Windows, use `venv\Scripts\activate`
    ```

3. **Install Required Packages**:

    ```sh
    pip install -r requirements.txt
    ```

## Usage

1. **Prepare Data**:

    Place your PDF documents in the `data/` directory. Ensure that the directory contains only PDF files that you want the assistant to use.

2. **Run the Application**:

    ```sh
    streamlit run app.py
    ```

    This will start the Streamlit server, and you can access the application in your web browser at `http://localhost:8501`.

## Customization (If you plan on using this code for your personal requirements):

- **Model and Embeddings**: You can switch to different models and embeddings as needed by adjusting the respective class initializations.
- **Text Splitter**: Adjust the `chunk_size` and `chunk_overlap` to better suit your document structure.

## Troubleshooting

- **Import Errors**: Ensure all packages are correctly installed and that your Python environment is activated.
- **Model Loading Issues**: Verify the model file path and ensure it is compatible with the `CTransformers` class.

## A Big Shout out to The Bloke for the Llama Quantisized model.

Enjoy using Baymax!!
