[![Python application test with Github Actions](https://github.com/brkaltinn/scaffold/actions/workflows/main.yml/badge.svg)](https://github.com/brkaltinn/scaffold/actions/workflows/main.yml)

# Scaffold
This is a project scaffold for Python


## AWS Setup

### Git Commands
* Check status with "git status"
* If the file is already exist in the repo, "git add <filename>" or * for all files.
* git commit -m "<Explanation>"
* git push


* If there is an error activating the venv go to venv directory and run "virtaulenv .env" command

### Configuring Makefile

Paste the code below

```
install:
	pip install --upgrade pip &&\
		pip install -r requirements.txt
		
format:
	black *.py
	
lint:
	pylint --disable=R,C hello.py
	
test:

	python -m pytest -vv --cov=hello test_hello.py

all: install lin test
```

### Configuring Requirement.txt

* pylint
* pytest
* click
* black
* pytest-cov

and run "make install" command

## Azure Setup

### Git Commands
* Check status with "git status"
* If the file is already exist in the repo, "git add <filename>" or * for all files.
* git commit -m "<Explanation>"
* git push


* If there is an error activating the venv go to venv directory and run "virtaulenv .env" command
### Configuring Makefile

Paste the code below

```
install:
	pip install --upgrade pip &&\
		pip install -r requirements.txt
		
install-azure:
		pip install --upgrade pip &&\
		pip install -r requirements-azure.txt

format:
	black *.py
	
lint:
	pylint --disable=R,C hello.py
	
test:

	python -m pytest -vv --cov=hello test_hello.py

all: install lin test
```