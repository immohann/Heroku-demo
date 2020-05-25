# Heroku-demo
A demo on hosting you ML model Flask app on heroku CLI using git.
### Note: Heroku provides only 500MB of space for deployment in all. 

_______________________
##### This is just a demo to deploy a Flask app on Heroku, there are plenty of other hosting platforms available like: [pythonanywhere](https://www.pythonanywhere.com/),[AWS](https://aws.amazon.com/getting-started/hands-on/launch-an-app/),[gcloud](https://cloud.google.com/ai-platform/prediction/docs/deploying-models) and more, do check them out.

### Prequisites
- Python
- pip
- Heroku CLI
- Git

### Files required for Heroku:
- templates : folder containing your index.html file
- Procfile : Procfile is a mechanism for declaring what commands are run by your application’s dynos on the Heroku platform
- requirements.txt : containing the list of all the required libraries.

Rest are the basic Flask App file 

### Steps: 
- create a virtual env: conda create --name venv
- do: pip install flask gunicorn
- get all the files from here or create new
- create and push all the files in a git repo: 
  - git add . 
  - git commit -m 'first commit'
  - git push
- do: heroku login
- do: heroku create name_you_want_for_your_app
- do: git push heroku master
- After the above command you'll get a link for the deployed app on your screen.

For more detailed steps: [Heroku](https://www.geeksforgeeks.org/deploy-python-flask-app-on-heroku/) 
