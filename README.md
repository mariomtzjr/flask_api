# flask_api

## Requirements
- Flask
- Flask Restful
- Flask SQLAlchemy
- Flask Migrate
- Flask Marshmallow
- Marshmallow SQLAlchemy

## Create virtual environment
`python3 -m vev flask_api`  

## Activate virtual environment
`source flask_api/bin/activate`

## Install requirements
`pip3 install -r requirements.txt`

## Export variables
`export FLASK_APP="entrypoint:app"` 
`export FLASK_ENV="development"` 
`export APP_SETTINGS_MODULE="config.default"`  

## Set up database
At the same level of entrypoint.py file, run the following commands:  
1. `flask db init`  
2. `flask db migrate -m "Initial_db"`
3. `flask db upgrade`

## Run server
`flask run`