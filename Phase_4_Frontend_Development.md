# Phase 4 – Frontend Development

## Activity 4.1: Designing and Developing the User Interface

FitBuddy provides a user-friendly and visually structured interface for fitness planning.

### index.html
- Acts as the main user input page.
- Collects user fitness information.
- Includes fields for basic details, fitness goal, and workout intensity.
- Uses a clean fitness-oriented design.

### result.html
- Displays the generated 7-day workout plan.
- Displays the nutrition or recovery information.
- Provides a feedback form for updating the workout plan.

### all_users.html
- Provides an admin view.
- Displays registered users and their workout plans.

### Responsive Design
- Uses Flexbox for layout.
- Includes responsive styling.
- Provides styled buttons and input fields.
- Uses spacing, rounded corners, and readable result sections.

## Activity 4.2: Creating Dynamic Templates with FastAPI's Jinja2

FitBuddy uses FastAPI's Jinja2Templates for dynamic HTML rendering.

### Template Integration
- FastAPI routes render the required HTML templates.
- Backend data is passed to the templates using context values.
- User information and workout plans are displayed dynamically.

### Form Binding
- index.html submits user information to the workout generation route.
- result.html displays workout details and accepts feedback.
- all_users.html displays user records using Jinja2 loops.

## Frontend Flow

User Input → FastAPI Route → Generated Workout Plan → result.html → Feedback → Updated Plan
