# Setup Python 3 on CentOS

See https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-local-programming-environment-on-centos-7 
```shell
sudo yum -y install yum-utils
sudo yum -y install https://centos7.iuscommunity.org/ius-release.rpm
sudo yum -y install python36u
python3.6 -V
sudo yum -y install python36u-pip
```

# Create the projtect

Create the project
`python3.6 -m venv django`

Activate it. Once activate can just use 'python" and 'pip' commands.
`source django/bin/activate`

Set up the debug toolbar as per http://django-debug-toolbar.readthedocs.io/en/stable/installation.html
`pip install django-debug-toolbar`

# Django manage functions

1. Start the integrated web server: `python manage.py runserver`
1. Set up a sqllite database: `python manage.py migrate`
1. Add an app: `python manage.py startapp books`
1. Update database model: `python manage.py makemigrations`
