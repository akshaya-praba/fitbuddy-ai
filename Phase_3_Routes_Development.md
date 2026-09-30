# Phase 3 – Routes Development

## Activity 3.1: Writing the Main Application Logic in routes.py

The `routes.py` file contains the main routing logic of the FitBuddy application. It connects the frontend, workout generation functions, feedback update function, and database operations.

## Core Routes

### 1. Home Route
Route:
`/`

- Displays the home page.
- Loads `index.html`.
- Provides the user input form.

### 2. Generate Workout Route
Route:
`/generate-workout`

- Receives user details using FastAPI Form parameters.
- Processes name, age, weight, goal, and intensity.
- Calls the workout plan generation function.
- Stores the user details and workout plan in the database.
- Displays the generated plan in `result.html`.

### 3. Update Plan Route
Route:
`/submit-feedback`

- Receives user feedback and user ID.
- Retrieves the existing workout plan.
- Calls `update_workout_plan()`.
- Updates the workout plan in the database.
- Displays the updated result.

### 4. Admin View Route
Route:
`/view-all-users`

- Retrieves user and plan records from the database.
- Displays all users and their workout plans.
- Uses `all_users.html` for the admin view.

## Backend Flow

User Input → FastAPI Route → Workout/Update Function → Database → HTML Result
