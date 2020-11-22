# covid-dash-backend

To develop and run:

- [Install python3.9](https://www.python.org/downloads/).  Keep an eye on where this
  is installing, it'll make life easier.  You may want to add python to your PATH so
  you can run commands from cmd.
- Install IDE of choice (I'm using pycharm)
- Clone this repository.  You need to create a file:
  `covid-dash-backend/clyde/clyde/secret_settings.py`, and put a variable in there
  called `SECRET_KEY` with a string I'll send you in a chat on here or something.
- pip install virtualenv with (substute `python` for `python3` if that's how it
  works on your computer).  In the `covid-dash-backend` dir, run the command
  `python -m pip install virtualenv`
- Create a virtual environment.  In the `covid-dash-backend` dir, run the
  command `python -m virtualenv --python=<path-to-your-python-install> env`.
  My install is on linux on `/usr/bin/python3.9`.  Yours maybe somewhere else,
  you're looking for that `/bin/python3.9` path.
- Now you'll have a dir `covid-dash-backend/env`.  This will be your base python
  install.  Set it in your editor of choice, or if you run from cmd, activate the
  env by running `source env/bin/activate` on linux or `env/bin/activate.bat` on
  windows (something like that, take a look, its a script).  You'll see your
  interpreter is now prepended with `(env)`, means the env is activated, to deactivate
  just run `deactivate`.
- Install required packages: with your `env` active, run 
  `python -m pip install -r requirements.txt`.
- To run: use the command `python manage.py runserver`, with the file
  `covid-dash-backend/clyde/manage.py`.  Then navigate in your browser to
  http://localhost:8000.
