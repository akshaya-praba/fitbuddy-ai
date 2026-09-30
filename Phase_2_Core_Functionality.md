# Phase 2 – Core Functionality Development

## Activity 2.1: Develop the Core Functionalities

### 1. Workout Plan Generation

Function:
`generate_workout_gemini()`

File:
`gemini_generator.py`

The application generates a structured 7-day workout plan using the user's:
- Name
- Age
- Weight
- Fitness goal
- Workout intensity

The generated plan contains day-wise workout activities, sets, reps, and safety guidance. :contentReference[oaicite:0]{index=0}

### 2. Feedback-Based Plan Updating

Function:
`update_workout_plan()`

File:
`updated_plan.py`

Users can submit feedback about their workout plan. The application uses the feedback to create an updated and lighter workout plan based on the user's requirements. :contentReference[oaicite:1]{index=1}

### 3. User and Plan Storage

File:
`database.py`

User details and workout plans are stored using SQLite and SQLAlchemy.

Stored details include:
- Name
- Age
- Weight
- Goal
- Intensity
- Workout plan

### Note

Gemini integration was prepared according to the project design. During local development and testing, a local workout-plan generator was used because live Gemini API quota was unavailable.
