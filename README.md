# basic_flask_api
basic flask api with deployment steps on heroku

Make sure to add following files:
* Procfile
* runtime.txt - to mention the python version to be used (must be supported by heroku, check from list https://devcenter.heroku.com/articles/python-support#supported-runtimes
* requirements.txt - package versions could sometime cause an issue (if not present in heroku, use a different version in that case)

After you code is pushed to github main, use following steps:

1. go to https://dashboard.heroku.com/apps and create a new app e.g. basicflaskapi
2. login to heroku cli in powershell / terminal using *heroku login* (for browser login) or *heroku login -i* (for login from powershell / terminal)
3. add you repo to heroku *heroku git:remote -a {project_name}* e.g. *heroku git:remote -a basicflaskapi*
4. push your code to heroku *git push heroku main*
5. if everything runs fine, a url would e generated for your app

App is running on *https://basicflaskapi.herokuapp.com/*