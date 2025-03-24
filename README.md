# TalkDB: Conversational Database Interface

This repository contains a Jupyter Notebook that extracts table schema from an SQLite database, generates a structured training plan, and uses an LLM to generate the results along with follow-up questions for SQL queries. It is designed to help users interact with databases more effectively by summarizing their structure and suggesting meaningful follow-up queries.

For detailed explanation of how this project works, including code walkthrough and implementation details, check out my [Medium article](https://medium.com/@vrajesh_b15/talking-with-your-database-using-llms-langchain-and-chromadb-d1ef08edde62).

## Overview

TalkDB creates a conversation-like interface to your SQL databases. Simply ask questions about your data in natural language, and TalkDB will:

1. Generate appropriate SQL queries
2. Execute them against your database
3. Return the results in a readable format
4. Remember your previous questions to avoid repetitive queries
5. Suggest meaningful follow-up questions

## Features

- Convert natural language to SQL automatically
- Cache similar questions to improve response time
- Maintain conversation context across sessions
- Generate relevant follow-up questions
- Support for multiple chat sessions

## Dependencies

- Python 3.8+
- Pandas
- NumPy
- SQLite3
- OpenAI API (or compatible LLM service)
- LangChain

## Configuration
You'll need:
- OpenAI API credentials (which can be replaced with Google's Gemini API using a free key from Google AI Studio or any other open-source LLMs)
- A SQL database connection (check the notebook for an example using the publicly available Chinook database)
- Basic Python environment

## License

[MIT License](LICENSE)
