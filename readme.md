# Scaffold project for interactive visual data analysis

This project is basically fork from [ivda-tutorial](https://gitlab.uzh.ch/ivda/ivda-tutorial) on Gitlab. Fully credits goes to the IVDA-team. This is just copy for scaffolding the later project.

## Server
Set up virtual environment with ``python -m venv env`` \
Select as interpreter in Pycharm or in VS Code:
``source ./env/bin/activate``
``code .`` \
Dependencies:
``
pip install flask==2.1.1 flask-restx==0.5.1 fastapi flask_pymongo pymongo flask_cors pandas statsmodels
`` \
I had to manually downgrade the Werkzeug package due to this [error](https://stackoverflow.com/questions/73105877/importerror-cannot-import-name-parse-rule-from-werkzeug-routing):
``pip install Werkzeug==2.1.2``

Using Brave as browser might result in a blocked request, try Chrome instead:
``GET http://127.0.0.1:5000/companies/4?algorithm=random net::ERR_BLOCKED_BY_CLIENT``