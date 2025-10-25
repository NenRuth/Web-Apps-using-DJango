# Web-Apps-using-DJango
building interactive websites
A web app called Learning Log that allows users to log the topics they’re interested in and to make journal entries
as they learn about each topic. The Learning Log home page describes the site and invite users to either register or log
in. Once logged in, a user should be able to create new topics, add new entries, and read and edit existing entries.

Sample guide:
cd "C:\Users\Lady Nen\Projects"

Create a new folder
mkdir InstaBook
cd InstaBook

Create a virtual environment
python -m venv insta_env

Activate the environment
.\insta_env\Scripts\activate

Install Django   (you should install Django inside each new virtual environment (venv) you create for a project. But you don’t have to reinstall Django globally every time.)
pip install django

Create your Django project
still in the same folder (C:\Users\Lady Nen\Projects\InstaBook), run: 
django-admin startproject instabook .   (mind the dot; the dot (.) at the end — that means “create the project in the current folder.)

Inspect the result
insta_env/
instabook/
manage.py

Inside instabook/ you’ll find: (in sublime text)
__init__.py
settings.py
urls.py
wsgi.py
asgi.py

Run the server
python manage.py runserver
at "http://127.0.0.1:8000/", you should see the “Congratulations! You’ve successfully installed Django” page.

Stop the server
Press CTRL + C in PowerShell.


Close the server and deactivate the environment

If the server is still running:

Press CTRL + C in PowerShell to stop it.
Then deactivate your virtual environment:
deactivate
(Your prompt will look normal again (no (insta_env) prefix))

Navigate to your “Projects” folder in PowerShell:
cd "C:\Users\Lady Nen\Projects"
dir
Remove-Item -Recurse -Force InstaBook

This deletes:
The virtual environment folder (insta_env)
The Django files (manage.py, instabook/, etc.)
The SQLite database (if created)

To verify they’re gone
dir
