# Heroku PDM Example (project skeleton)

[Heroku buildpacks](https://github.com/heroku/heroku-buildpack-python) for Python (version 20 or 22) do not yet support [PDM](https://pdm.fming.dev/latest/) out of the box. (See [Heroku docs](https://devcenter.heroku.com/articles/python-support))

This repo provides a workaround. 

## tl;dr

This example provides a [requirements.txt](requirements.txt) with just pdm in it.
The [Procfile](Procfile) installs the environment from [pyproject.toml](pyproject.toml) and runs the service (unicorn-fastapi)

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

## How to use this repository

- checkout the repo
- cd into the repo
- `rm -rf .git`
- then you can create a new git repo with `git init .`
- add your code
- `git add .`
- `git commit -m 'initial'`
- configure heroku
  - `heroku create example-pdm-app-foobar`
  - `heroku git:remote -a example-pdm-app-foobar`
  - `git push heroku main` will deploy the app
  - `heroku logs --tail` to see the logfiles
