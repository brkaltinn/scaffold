# scaffold
This is a project scaffold for Python

* If there is an error activating the venv go to venv directory and run "virtaulenv .env" command

### Configuring Makefile

Paste the code below

"""
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
"""

### Configuring Requirement.txt

* pylint
* pytest
* click
* black
* pytest-cov

and run "make install" command