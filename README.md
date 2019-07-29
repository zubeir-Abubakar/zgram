# Instagram
#### Web clone of the Instagram app

## Description
This is a simple web clone of the instagram website. A user can create an account and sign into it. 
The site supports uploading images,liking and commnting on images.
users can view photos uploaded by other users in the home page of app and also give out their feedback.



## Set Up and Installations

### Prerequisites
1. LINUX
2. Python3.6
3. [Postgres](https://www.postgresql.org/download/)
4. python virtualenv

### Clone the Repo
Run the following command on the terminal:
`git clone git@github.com:zubeir-Abubakar/Zgram && cd Zgram

### Activate virtual environment
Activate virtual environment using python3.6 as default handler
```bash
virtualenv -p /usr/bin/python3.6 venv && source venv/bin/activate
```

### Install dependancies
Install dependancies that will create an environment for the app to run
`pip3 install -r requirements.txt`

### Create the Database
```bash
psql
CREATE DATABASE insta;
```
### .env file
Create .env file and paste paste the following filling where appropriate:
```python
SECRET_KEY = '<Secret_key>'
DBNAME = 'insta'
USER = '<Username>'
PASSWORD = '<password>'
DEBUG = True

EMAIL_USE_TLS = True
EMAIL_HOST = 'smtp.gmail.com'
EMAIL_PORT = 587
EMAIL_HOST_USER = '<your-email>'
EMAIL_HOST_PASSWORD = '<your-password>'
```
### Run initial Migration
```bash
python3.6 manage.py makemigrations insta
python3.6 manage.py migrate
```

### Run the app
```bash
python3.6 manage.py runserver
```
Open terminal on `localhost:http://127.0.0.1:8000/`

## Known bugs
Like functionality not well implemented and some functionalities not yet well implimented 

## Technologies used
    - Python 3.6
    - HTML
    - Bootstrap 4,3
    - Heroku
    - Postgresql
    - Virtual studio code

## Support and contact details
Contact me for further help/support through +254743046778

