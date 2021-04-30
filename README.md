# Run Flask App
1. Install Flask Requirements by running command `pip install requirements.txt`
2. Set App File and Run with following commands
 
     (Mac/Linux)
     `export FLASK_APP=app.py`

     (Windows)
     `set FLASK_APP=app.py`

     `flask run`


# Run Python Console
In the same directory as login.db

run command $ `python`

# Query Database
1. Import database and user class `from app import db, User`
2. Query all `results = User.query.all()` OR  Query specific column and select first result user = User.query.filter_by([column name = entry]).first() Example `user = User.query.filter_by(username = 'TestUser').first()`
3. results[0].[column name] Example `results[0].username`


# Change CaliberAdmin Password
1. Import database and user class `from app import db, User`
2. Query for admin `admin = User.query.filter_by(username = 'CaliberAdmin').first()`
3. Change passwors `admin.password = "enterNewPassword"`
4. commit changes to database `db.session.commit()`

# Final Video
The file size for our final presentation is too large for Github to process, so it can be found at this link: https://drive.google.com/file/d/1z4aiWRxwrzr-ssnoofEHiarLLAk3HDBx/view?usp=sharing
