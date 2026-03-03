FastAPI LLM Backend

A simple backend application built using FastAPI that integrates with an LLM API to generate AI responses. This project demonstrates REST API development, environment variable management, and LLM integration using Python.

Features

FastAPI-based REST API

LLM integration using OpenAI API

Secure API key handling using environment variables

Pydantic request validation

Interactive Swagger documentation

Clean and minimal backend structure

Tech Stack

Python

FastAPI

Uvicorn

OpenAI Python SDK

Pydantic

python-dotenv

Project Structure
ai-llm-fastapi/
│
├── main.py
├── .env
├── .gitignore
├── requirements.txt
Installation

Clone the repository

git clone https://github.com/nithish-ui/fastapi-llm-backend.git
cd fastapi-llm-backend

Create virtual environment

python -m venv venv

Activate virtual environment

Windows:

.\venv\Scripts\Activate.ps1

Install dependencies

pip install -r requirements.txt
Environment Setup

Create a .env file in the root directory:

OPENAI_API_KEY=your_api_key_here

Do not commit this file to version control.

Running the Server
python -m uvicorn main:app --reload

Server will start at:

http://127.0.0.1:8000

Interactive API docs available at:

http://127.0.0.1:8000/docs
API Endpoints
GET /

Health check endpoint.

POST /generate

Request body:

{
  "prompt": "Explain FastAPI in simple terms."
}

Response:

{
  "response": "FastAPI is a modern Python framework..."
}
Learning Outcomes

Building REST APIs with FastAPI

Integrating LLM APIs into backend systems

Managing secrets securely with environment variables

Structuring backend applications professionally

Running local development servers with Uvicorn