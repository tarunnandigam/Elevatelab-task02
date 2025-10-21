# Simple Django Todo App

A minimal todo application built with Django that allows you to create, edit, delete, and toggle completion status of tasks.

## Features
- Add new todos
- Mark todos as complete/incomplete
- Edit todo titles
- Delete todos
- Clean, responsive interface

## Setup Instructions

1. Install Python (3.8 or higher)
2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

3. Run migrations:
   ```
   python manage.py makemigrations
   python manage.py migrate
   ```

4. Start the development server:
   ```
   python manage.py runserver
   ```

5. Open your browser and go to `http://127.0.0.1:8000`

## Usage
- Type a task in the input field and click "Add" to create a new todo
- Click "Done" to mark a task as completed (or "Undo" to mark as incomplete)
- Click "Edit" to modify a task's title or completion status
- Click "Delete" to remove a task (with confirmation prompt)