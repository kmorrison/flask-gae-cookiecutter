## Python Flask Cookiecutter for Google App Engine

A skeleton for building Python applications on Google App Engine with the
[Flask micro framework](http://flask.pocoo.org).

## Usage

1. Use the [Admin Console](https://appengine.google.com) to create a
   project/app id. (App id and project id are identical)
2. Install the [App Engine Python SDK](https://developers.google.com/appengine/downloads).
See the README file for directions. You'll need python 2.7 and [pip 1.4 or later](http://www.pip-installer.org/en/latest/installing.html) installed too.

3. install `cookiecutter`

    ```
    pip install cookiecutter
    ```
4. Clone this repo with

   ```
   cookiecutter https://github.com/kmorrison/flask-gae-cookiecutter.git
   ```
5. Follow instructions in your new project's README :)

### Relational Databases and Datastore
Appengine gives you a lot of stuff for free if you're willing to do it their
way. ndb (non-relational storage), users (user auth), memcache, and more.

### Feedback
Star this repo if you found it useful. Use the github issue tracker to give
feedback on this repo.

## Author
Heavily inspired by https://github.com/GoogleCloudPlatform/appengine-python-flask-skeleton, written by Logan Henriquez and Johan Euphrosine
Kyle Morrison

### Work to be done
This cookiecutter still needs work. Tests, for one. I'd also like to build in
Flask-S3 for serving static files, and come up with an easy way to store secret
values like AWS keys.
