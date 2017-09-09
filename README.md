Learning to use django.

Package manager is conda. Actual dependencies should be available via yaml file.
create a virutal environment to isolate dependencies from other projects and host system
	- pip is what the django documentation is using. 

python manage.py 
	- runserver
	- migrate : applies database migrations after schema changes or to start up a db.
	- help

There is an admin portal to manage authentication, ui for manipulating entries.

Django philosophy:
Multiple apps installed within a django project. running manage.py will give you a clearer idea 
of this. 
See settings.py for managing the applications for the django project. Many of these apps are 
provided by django, such as auth, admin, sessions, messages, etc. 

Files of importance:
		settings.py : manages timezone, db engine of choice, other base directory stuff.
		urls.py: matching string patterns to endpoints in views.py
		models.py: oo representation of stuff.
		views.py: can be considered as "adapters", interfacing between the data and the actual views (html)
			- Large collection of available templates for common use cases. 
all db migrations are available.

Does it play well with React? 
yes, you can remove the templating library of django and replace that part with react. webpack to bundle react and then it just talks to django via http (duh)

Have you used it with postgresql? 

Tutorial: django girls tutorial
