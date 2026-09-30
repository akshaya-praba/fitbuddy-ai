# Phase 1 – Project Setup

## Milestone 1: Model Selection and Architecture

### Activity 1.1: Research and Select the Appropriate Generative AI Model

FitBuddy requires an AI model to:
- Generate structured 7-day workout plans
- Provide concise nutrition tips
- Update workout plans based on user feedback
- Support real-time web-based interaction

After evaluating different models, Google Gemini models were selected because they are API-based, easy to integrate with FastAPI, and suitable for structured responses.

### Activity 1.2: Define the Application Architecture

FitBuddy follows a modular FastAPI-based architecture:

- Frontend: HTML + Jinja2 templates
- Backend: FastAPI
- AI Layer: Google Gemini APIs
- Database: SQLite with SQLAlchemy

Main frontend files:
- index.html – User input form
- result.html – Workout plan and feedback
- all_users.html – Admin view

### Activity 1.3: Set Up the Development Environment

The development environment includes:

- Python and pip
- Virtual environment
- FastAPI
- Uvicorn
- Jinja2
- SQLAlchemy
- python-multipart
- Gemini integration library

Project structure:

- /app – Python files
- /templates – HTML templates
- /static/images – image assets

The application can be run locally using FastAPI and Uvicorn.
