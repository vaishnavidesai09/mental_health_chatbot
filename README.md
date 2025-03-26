# Mental Health Chatbot

## Overview
This project is a **compassionate mental health chatbot** that provides supportive and thoughtful responses to users' queries. It utilizes **LangChain**, **ChromaDB**, and **HuggingFace embeddings** to process and retrieve relevant information from PDF documents. The chatbot is powered by **Llama 3.3-70B** via Groq API to ensure intelligent and context-aware interactions.

## Features
- Loads and processes PDF documents for knowledge retrieval.
- Uses **HuggingFace BGE embeddings** for vectorizing text.
- Stores embeddings in **ChromaDB** for fast retrieval.
- Implements **RetrievalQA** from LangChain for efficient response generation.
- Provides thoughtful responses based on retrieved information.
- Simple command-line interface for user interaction.

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/mental-health-chatbot.git
   cd mental-health-chatbot
   ```
2. Install dependencies:
   ```sh
   pip install langchain chromadb sentence-transformers
   ```
3. Ensure you have **Groq API Key**:
   - Replace `groq_api_key` in `initialize_llm()` with your actual API key.

## Usage
Run the chatbot using:
```sh
python chatbot.py
```
### Commands
- **Ask a question**: Simply type your query.
- **Exit**: Type `exit` to terminate the chatbot.

## Code Structure
- `initialize_llm()`: Initializes the language model.
- `create_vector_db()`: Loads and embeds documents into ChromaDB.
- `setup_qa_chain()`: Configures the chatbot's retrieval and response generation.
- `main()`: Runs the chatbot in an interactive loop.

## Example Interaction
```
Human: How can I manage stress?
Chatbot: Practicing mindfulness, deep breathing, and regular exercise can help in managing stress effectively.
```

## Future Enhancements
- Improve response personalization.
- Integrate with a frontend interface.
- Expand document types beyond PDFs.

## License
This project is licensed under the MIT License.



