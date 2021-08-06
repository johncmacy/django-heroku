# django-basic

## About

This is a basic Django project that includes:

* Users app for user registration, authentication, etc.
* User model that extends the built-in User model by subclassing AbstractUser
* Project-level templates and static folders
* Base HTML templates
* site.css

## Getting Started

### Create repo from template

1. Click the green `Use this template` button above.
2. Choose the owner, name, and other initial settings as required for your project.
3. Click `Create repository from template`.

### Clone repo to local

1. In a terminal, change directory to the desired location. For example, `cd C:/apps`.
2. On your new repo's main page, click the `Code` dropdown button.
3. With HTTPS selected, copy the URL.
4. In the terminal, `git clone <paste url from step 3>`.
5. Change directory into the new folder, like so: `cd my-project`.
6. Run `code .` to open it in Visual Studio Code.

### Set up your local environment

1. In the terminal, run `py -m venv env` to set up a virtual environment named "env".
2. Activate the virtual environment with `env/scripts/activate`.
3. Run `py -m pip install -r requirements.txt`.
4. Configure database settings from Heroku config vars.
5. Run `py manage.py migrate` to initialize the database tables.
6. Create a superuser record for yourself by running `py manage.py createsuperuser`, and follow the prompts for username, email, and password.
7. Run the server (with `py manage.py runserver`, or F5 once you've set up a "launch.json" file).
8. Navigate to http://127.0.0.1:8000/ to verify that it is working. You should see a welcome page, with links for Home, Profile, and Admin in the navbar.

### Push to Heroku
1. In your Heroku dashboard, click the **Deploy** tab, then connect to your project's GitHub repo in the **Deployment method** section.
2. Make sure **main** is selected as the branch to deploy, then click the **Enable Automatic Deploys** button.
3. `git add .`
4. `git commit -m "..."`
5. `git push`
6. Assuming the branch is **main**, this will trigger a build.
7. Once the build is complete, go to your Heroku app's url to verify it is basically working.