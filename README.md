# RAG_Odoo_LLM
FastAPI with LangChain Integration

This repository contains a FastAPI application designed to showcase the integration of FastAPI with LangChain, utilizing external tools like Odoo and services for enhanced language understanding and processing capabilities. The application also demonstrates the use of JWT for authentication and handling of user sessions.

Features

User Authentication: Secure login with JWT-based authentication.
LangChain Integration: Utilizes LangChain to enhance responses with real-time data from external APIs like Odoo.
Odoo ERP Integration: Interacts with Odoo to fetch and manipulate data regarding companies and contacts.
Dynamic Response Translation: Includes functionality to detect the user's query language and translate responses accordingly.
Appointment Scheduling: Allows users to schedule appointments through the Odoo calendar.
Technologies

FastAPI: High-performance web framework for building APIs with Python 3.6+ based on standard Python type hints.
LangChain: Used to integrate language understanding capabilities.
Odoo: Open-source ERP for managing various business operations.
JWT: Used for secure authentication handling.
Pydantic: Data validation and settings management using Python type annotations.
ngrok: Exposes local servers behind NATs and firewalls to the public internet over secure tunnels.
Installation

Prerequisites
Python 3.6+
Pip
Setup Environment
# Clone the repository
git clone https://github.com/sravaninni/RAG_Odoo_LLM.git
cd RAG_Odoo_LLM

# Create a virtual environment
python -m venv venv

# Activate the virtual environment
# Windows
venv\Scripts\activate
# Unix or MacOS
source venv/bin/activate

# Install the dependencies
pip install -r requirements.txt
Configuration
Before running the application, ensure you set up the necessary API keys and database credentials:

Set your Odoo API credentials and other relevant settings in config.py or as environment variables.
Configure your JWT secret key and other security features.
Usage

To run the FastAPI application:

# Start the application
uvicorn app:app --reload

# The API will be available at http://127.0.0.1:8000
# ngrok URL will be printed to the console for public access
API Endpoints

/login: Authenticate users and receive JWT for accessing protected routes.
/agent_query: Submit queries to be processed by LangChain integrated tools.
Additional endpoints for managing contacts, companies, and appointments are documented in the Swagger UI accessible at /docs once the server is running.
Contributing

Contributions to this project are welcome! Please fork the repository and submit a pull request with your features or fixes.
