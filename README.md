AI Author Bot
Overview
This repository contains the code for an AI Author Bot that analyzes and interacts with a collection of an author's writings. The bot uses embeddings to understand the author's writing style and generate intelligent responses to questions based on their work. It leverages the LangChain library to split text, embed it, and retrieve relevant information through pre-trained language models.

The bot supports both paid and free language models, providing flexibility in terms of API usage and performance. It can store memory of past interactions for more coherent conversations and return source documents when necessary.

Features
Text Embedding: Supports embeddings from both OpenAI and Hugging Face models.
Retrieval-based Question Answering: Uses a retrieval mechanism to answer questions based on the author's writings.
Memory Integration: Maintains conversation history with a memory buffer for more natural interactions.
Customizable LLMs: Easily switch between OpenAI (paid) and Hugging Face (free) models.
Prompt Template: Uses a customizable prompt template to ensure accurate and contextual responses.
Interactive Session: Allows users to engage with the bot in real-time via an interactive console.
Requirements
Python 3.7 or higher
API keys for OpenAI or Hugging Face Hub
Dependencies listed in requirements.txt
Installation
Clone this repository:

bash
Copy code
git clone https://github.com/yourusername/ai-author-bot.git
cd ai-author-bot
Install the required dependencies:

bash
Copy code
pip install -r requirements.txt
Create a .env file in the project root and add your API keys:

bash
Copy code
OPENAI_API_KEY=your_openai_api_key
HUGGINGFACEHUB_API_TOKEN=your_huggingfacehub_api_token
Add a text file named sample_writings.txt containing the author's writings in the project directory.

Usage
To run the bot, execute the following command:

bash
Copy code
python ai_author_bot.py
During the session, you can ask the bot questions about the author's writings. Type exit to end the session.

Configuration
Embedding Models: The bot can be configured to use either OpenAI or Hugging Face embeddings. Modify the embedding_model variable in the code ("openai" for OpenAI and "huggingface" for Hugging Face).
LLM Models: Similarly, you can switch between OpenAI and Hugging Face models by changing the llm_model variable in the main function.
Logging and Error Handling
The bot uses Python's logging module to log important events and errors. If an error occurs, it will be logged, and the bot will continue functioning where possible.
