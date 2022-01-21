# CIE 
# Constructiveness and Inclusiveness Evaluator


## To create a nev virtual environment run in the project's directory:
```python -m venv .venv```
You should do it once. Each next time you should activate and deactivate the venv

To activate env run in the project's directory:
```source .venv/bin/activate```

To deactivate env run in the project's directory:
```deactivate```

### To install a new package/library (requirement) into env 
```pip install <package/library name>```

After each requirement was changed, please don't forget to update requirements.txt file by running in the project's directory:
<br>
```pip freeze > requirements.txt```

### To install all requirements
```pip install -r requirements.txt```

### To install app locally run from /back folder
```pip install -e ./flaskr``` 

### To start application locally
```export FLASK_APP=flaskr```
<br>
```flask run```
<br>
It should start and print a link to access it in browser.


### To run training_dt_rf_knn_models.py
To run module as a file use -m:
```python -m models.training_dt_rf_knn_models```

## To run the project in a Docker:

Build the image:
```docker-compose build```

When the image is built, run the container:
```docker-compose up```

After a successful start it should show the link for accessing http://172.19.0.3:8000/ 
It is an internal link, for accessing the site in browser please use localhost:8000/

To close and exit:
```docker-compose down -v```
