.PHONY: clean build deploy

all: build

clean:
	find . -name '*.pyc' -exec rm -f {} +
	rm -rf lib/*

build:
	pip install -r requirements.txt -t lib/

deploy: clean build
	appcfg.py -A {{cookiecutter.appengine_project_id}} --oauth2 update .
