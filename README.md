### Project setup

1. Create a virtual environment in your project folder using the command - python3 -m venv virtualenvironmentname
2. Source the virtual env using the command - source virtualenvironmentname/bin/activate
3. Install the packages required from requirements.txt file - pip3 install -r requirements.txt

#### To setup Database and superuser credentials
1. Create your database app using the command - __python3 manage.py startapp dbname__
2. Create the model structure in the models.py file that has been generated inside the directory generated with dbname.
3. After creating model structure or whenever you make changes to your model, create migration script using the command -
   __python3 manage.py makemigrations dbname__
4. Execute the migration script every time after you create the migration script - __python3 manage.py migrate dbname__
5. Create the superuser - __python3 manage.py createsuperuser__
6. Change the password for an user - __python3 manage.py changepassword username__

Run the server using the command - __python3 manage.py runserver__

http://127.0.0.1:8000/admin - Login to admin page using super user credentials 