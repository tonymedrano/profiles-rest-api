# profiles-rest-api
Source code for profiles REST API course
## A REST API that supports the following:

- Creating new profiles.
- Logging in with a profile.
- Adding profile status updates.
- Viewing users profile fields.
- Searching for users profiles.

## Development setup
- install virtual box
- install vagrant

## First steps
- terminal: vagrant up -> vagrant ssh 
- Note: after that, you should see terminal user switch to something like this  -> vagrant@ubuntu-xenial:
- It means you're in the vagrant virtual development server!
- Note: To quite type exit (that's it!)

## Testing environment
- Get into type: vagrant ssh
- Next: cd /vagrant -> touch test.txt

## Create a python environment using terminal

- Get into type in the root project
```sh
vagrant ssh
```

- Get into type in the vagrant folder,remember you're now vagrant@ubuntu-xenial: 
```sh
cd /vagrant
```

- Get into type in the vagrant folder,remember you're now vagrant@ubuntu-xenial: 
```sh
python -m venv ~/env
```

- If doesn't work tryi installing first (you're using python 3)
```sh
sudo apt-get install python3-venv
```

- Activate environment
```sh
source ~/env/bin/activate
```

- Should see terminal similar to this where (env) is the environment name
```sh
(env) vagrant@ubuntu-xenial:/vagrant$ 
```

## Deactivate from environment
```sh 
deactivate
```

## Project dependencies list

- django
- djangorestframework

## Create a requirements.txt file and add
`
django==2.2
djangorestframework==3.9.2
`

## Install dependencies now by running
```sh 
pip install -r requirements.txt
```

## New Django project named profiles_project (. == root)
```sh 
django-admin.py startproject profiles_project .
```
```sh 
python manage.py startapp profiles_api```

```sh 
python manage.py runserver 0.0.0.0:8080
```

Tony A. Medrano Twitter & Email – [@tonymedranocom](https://twitter.com/tonymedranocom) – info@tonymedrano.com
