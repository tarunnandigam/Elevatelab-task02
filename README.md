##issues i have git while implementing 

--Issue:
1) When Jenkins tried to run Docker commands during the pipeline, I got this error:

==Got permission denied while trying to connect to the Docker daemon socket
solution:
i have Added the Jenkins user to the Docker group and restarted Jenkins.

2)Issue:
Jenkins couldn’t clone the repository and showed authentication errors when accessing GitHub.

Solution:
Configured Git credentials in Jenkins:

Open Jenkins → Manage Credentials.

Add GitHub username and Personal Access Token.

Used those credentials in the pipeline or job configuration.

3)Issue:
When redeploying the Docker container, Jenkins showed:

Error starting userland proxy: listen tcp :8000: bind: address already in use

solution:
Added cleanup commands before deploying a new container.


#####I have also include the images(screen shots of the project also ) in /images folder...#####



##NOTE :: we can also use the github webhook this help to noy use build commond to use every time as i make any change in the repo (means commit ) it will auto-matically trigger the build.

####resources :
1) jenkins documentations
2)train with subham tutoraials




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
