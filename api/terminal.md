1. Find the correct file path.
2. Create python virtual environment by python
```
python3 -m venv <env_name>
python3 -m venv .api
```
3. Activate the virtual environment
```
source <env_name>/bin/activate
source .api/bin/activate
```
4. Install necessary packages: flask
```
pip3 install flask
pip3 install flask-sqlalchemy
```
5. Export the environment requirements
```
pip3 freeze > requirements.txt
```
6. Create the coding file
```
touch <file_name>.py
touch application.py
```
7. Flask looks for a file named <file_name>.py to find the Flask app.
Setting the environment to development mode activates the debugger and the reloader.
```
export FLASK_APP=<file_name>.py
export FLASK_ENV=development
```
```
export FLASK_APP=application.py
export FLASK_ENV=development
```
8. Enter into python to create table
```
python3
# Launches an interactive Python shell in the context of a Flask application - automatically sets up the application context
flask shell
from application import db
db.create_all()
```
9. Enter data,add a new record to the database and then commit the transaction
```
from application import Drink
drink = Drink (name="Grape soda", description="taste good")
db.session.add(drink)
db.session.commit()
```

```
db.session.add(Drink(name="Cherry",description="taste great"))
db.session.commit()
```
10. Retrieve all drink list
```
Drink.query.all()
```
11. Go to postman to try post and delete method
choose 'post' - body (raw) - json
choose 'delete' - body - (n/a)

12. Run flask
```
flask run
```