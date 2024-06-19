# Database Q&A 🤖

Welcome to the **Database Q&A** project! This tool leverages advanced language models and semantic search to provide accurate and insightful answers to your database queries. By integrating cutting-edge technologies, it aims to streamline the way we interact with databases.

## Features

- **Advanced LLM Integration**: Uses GooglePalm and Ollama for precise language understanding and query generation.
- **Semantic Similarity Matching**: Employs HuggingFace embeddings to select the most relevant examples.
- **Efficient Vector Storage**: Utilizes Chroma for efficient vector storage and retrieval.
- **Interactive UI**: Built with Streamlit for a user-friendly and interactive experience.

## How It Works

1. **User Input**: Enter your question in natural language.
2. **Query Generation**: The system generates a relevant MySQL query.
3. **Query Execution**: The query is executed against the specified database.
4. **Result Interpretation**: The results are interpreted and presented in a clear, concise manner.

## Technology Stack

- **LangChain Community**: For seamless integration of language models.
- **HuggingFace Embeddings**: `sentence-transformers/all-MiniLM-L6-v2` for semantic similarity.
- **Chroma**: Efficient vector storage and retrieval.
- **Streamlit**: Interactive and user-friendly interface.

## Setup

1. Clone the repository:
    ```bash
    git clone https://github.com/owais-mazhar/database-qa.git
    cd database-qa
    ```

2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

3. Set up your database connection in `langchain_helper.py`:
    ```python
    db_user = "root"
    db_password = ""
    db_host = "localhost"
    db_name = "task_6"
    ```

4. Obtain your Google API key and set it in the `get_few_shot_db_chain` function:
    ```python
    api_key = "your_google_api_key"
    ```

## Usage

1. Run the Streamlit app:
    ```bash
    streamlit run app.py
    ```

2. Enter your question in the provided text input.

3. View the generated SQL query and the resulting answer.

## Contributing

We welcome contributions! Please fork this repository and submit pull requests.

## Contact

For questions or suggestions, feel free to reach out to me via [LinkedIn](https://www.linkedin.com/in/owaismazhar/).