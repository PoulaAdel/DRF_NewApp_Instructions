# DRF_NewApp_Instructions
Clear and easy steps to create a Django Rest Framework API

## Inital github repo
- create repo
- create files (gitignore / license)
- add data to .ginignore file
- copy repo link

- create project folder on local machine
- commands:
  
```
	$cd <project_folder>
	$code .
```

- vscode will open
- link git repo commands:
```
	$git init -b main
	$git add .
	$git remote add origin  <REMOTE_URL>
	$git remote -v
	$git branch --set-upstream-to=origin/main main
	$git pull
```


## create new djangorestframework project 
- open terminal on vs code within project folder
- commands:
```
	$python3 -m venv <env_name>
	$source <env_name>/bin/activate OR ./<env_name>/Source/activate (for windows)
	$pip3 install django OR djangorestframework
	$django-admin startproject <project_name> .
	$python3 manage.py startapp <app_name>
	$python3 manage.py migrate
	$python3 manage.py createsuperuser
```

- adjust setting.py file
```
	$add 'rest-framework' to INSTALLED_APPS
	$add '<app_name>.apps.ApiConfig' to INSTALLED_APPS
	$change key
```


## test app 
- on vscode terminal:
```
	$python3 manage.py runserver <ip>:<port>
```

- open browser and type <ip>:<port>


## upload working project to git repo 
- on vscode terminal:
```
	$git commit -m "First commit"
	$git push -u origin main
	$git remote set-head origin main 
```

## if gitignore not working fine 
- First commit any outstanding code changes, and then, run this command:
```
	$git rm -r --cached .
```

- This removes any changed files from the index(staging area), then just run:
```
	$git add .
```

- Commit it:
```
	$git commit -m ".gitignore is now working"
```
