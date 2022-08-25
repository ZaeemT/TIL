# TIL: Today I Learned :books:

It is a webapp that is similar to twitter. Using `python` and `html`, along with various other technologies.

Implemented Django's class-based views. Access detailed documetation of this at <https://ccbv.co.uk/>. Install `Django` for the backend of the project. Write following commands on your `cmd`:

```
pip install django
```
 
To start with the *project* run the command below on the `cmd`. It will make a folder for the project. Here **til** is the name of the project, and the `.` after the name project means to create the folder in the current directory.

```
django-admin startproject til . 
```

To run your project over your browser run following command, it will *locally host* your project over port 8000. You can access it at `http://localhost:8000/`.

```
python manage.py runserver 
```

Create a *user* that could access and manage the django admin. The admin site could be accessed at `http://localhost:8000/admin` by logging in with the credentials of the super user. You will be asked to enter name, email and password. Run this command to create the user:

```
python manage.py createsuperuser
```

The project is your enviorment while an *app* performs a function, and a project is collection of multiple apps. To create app ending with the name of it, in this case it is **feed**:

```
python manage.py startapp feed
```

Afterwards you have to models in the app. Models acts as database tables. Some configurations are to be made while making the model you can learn more at <https://docs.djangoproject.com/en/4.1/intro/tutorial01/>. After making a model you have to define your app in `settings.py` of the project under the variable **INSTALLED_APPS**. Then run following commands:

```
python manage.py makemigrations
python manage.py migrate
```

TODO: Add details about django-allauth and tailwind css.







