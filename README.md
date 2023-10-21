# Ask Qdrant - Remote Database Querying with AI

## Introduction

**Ask Qdrant** is a Python application that allows you to query a remote database using natural language questions. It leverages state-of-the-art AI models and vector stores for efficient retrieval.

## Getting Started

To use **Ask Qdrant**, follow these steps:

### Prerequisites

Make sure you have the following installed:

- Python 3.x
- Required Python packages (install using `pip`):
  - `dotenv`
  - `streamlit`
  - `qdrant_client`

### Installation

1. Clone this repository to your local machine:

   ```
   git clone https://github.com/Gitcomplex/Qdrant-VectorDB.git
  
   ```

2. Install the necessary Python packages:

   ```
   pip install -r requirements.txt
   ```

3. Create a `.env` file in the project root directory and set the following environment variables:

   - `QDRANT_HOST` - The host URL of your Qdrant instance.
   - `QDRANT_API_KEY` - Your Qdrant API key.
   - `QDRANT_COLLECTION_NAME` - Name of the collection in Qdrant.
   - `HUGGINGFACEHUB_API_TOKEN` - API key for huggingface embedding and chatmodels

   Optional: you can also make use of OPEANI in that case add OPENAI_API_KEY instead of huggingfacehub.

### Usage

To run the application, execute the following command in your terminal:

```
streamlit app.py
```

Replace `your_script_name.py` with the name of your Python script containing the code provided.

The application will launch in your web browser. You can enter natural language questions about your remote database in the provided text input box. The application will then query the database and provide answers using a combination of AI models and vector stores.

## Configuration

- **Vector Store Configuration**: You can configure the vector store in the `get_vector_store` function. This code uses Qdrant as the vector store, but you can modify this function to use a different vector store.

- **AI Model Configuration**: The AI model used for answering questions can be adjusted in the `main` function. This code utilizes the Hugging Face Hub to load the model, but you can change the model and its parameters to fit your requirements.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Qdrant](https://github.com/qdrant/qdrant) - For providing efficient vector search capabilities.
- [Hugging Face Transformers](https://github.com/huggingface/transformers) - For state-of-the-art language models.
- [Streamlit](https://streamlit.io/) - For creating the user interface.

## Author

- DIPANSHU YADAV
- github.com/Gitcomplex

---
