# Goal: Set up python version and deps for a new project

0. Install pyenv and pipenv

pyenv manages the python version. pipenv manages the deps.

`brew install pyenv`
`pip install pipenv`

1. Use pyenv to install the version of python you want to use for the project

`pyenv versions` to see what versions you have installed

`pyenv install --list` to see what versions you can install

`pyenv install <VERSION>` to install your desired version

Now specify the version to use for the project with

`pipenv --python <VERSION>`

It will create a Pipfile specifying the required version of python.

2. Create a 'virtualenv' with dependencies for the project

`pipenv install <PACKAGE>`

This will add the package to the Pipfile and Pipfile.lock

3. You can now use `import` statements in your python project files and run them with 

`pipenv run python main.py`

4. You can run the python interpreter with those deps installed using

`pipenv shell`

5. Check Pipfile and Pipfile.lock into version control

# Goal: Install dependencies for an existing project

0. Clone the project and make sure pipenv is installed

1. Run `pipenv install`

More things

https://pipenv.pypa.io/en/latest/basics/#example-pipenv-upgrade-workflow
https://pipenv.pypa.io/en/latest/basics/#specifying-versions-of-a-package
https://pipenv.pypa.io/en/latest/basics/#specifying-versions-of-python

