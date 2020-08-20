# send-mail-Asynchronously
send mail Asynchronously using celery and redis

To run the application

Create a virtualenv and install the requirements.

Open a second terminal window and start a local Redis server.

Open a third terminal window. Set two environment variables MAIL_USERNAME and MAIL_PASSWORD to a valid Gmail account credentials (these will be used to send test emails). Then start a Celery worker: venv/bin/celery worker -A app.celery --loglevel=info.

Start the Flask application on your original terminal window: venv/bin/python app.py.

Go to http://localhost:5000/ and send email

