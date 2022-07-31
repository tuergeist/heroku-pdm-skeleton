# Heroku PDM Example (project skeleton)

Heroku buiildpacks for Python (version 20 or 22) do not yet support [PDM](https://pdm.fming.dev/latest/) out of the box.

This repo provides a workaround. 

## tl;dr

This example provides a requirements.txt with just pdm in it.
The Procfile installs the environment from pyproject.toml and runs the service (unicorn-fastapi)


.
