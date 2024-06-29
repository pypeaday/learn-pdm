# Learn PDM

## TLDR

Overall this is nice, but definitely a personal project. If I didn't have a workflow for python I liked, or if I didn't mutate it a little bit constantly then something like this makes a ton of sense... 

## Notes

https://github.com/pdm-project/pdm

Installed with pipx

## venv

`pdm venv create` will create a venv at `~/.local/share/pdm/venvs/...` so it's kind of like `pipx` where it has a virtual environment folder to put everything in. 

Looks to me like it assumes the parent folder is the projet name you're in, and so it puts that in the venv name, a hash of something, and the name of the environment.

Then `pdm venv list` must look at your parent directory and list all the venvs.... Frustrating to not have a `--all` option to see all the venvs that `pdm venv` has created

## Questions

`pdm init` asked for a python interpreter and put it in `.pdm-python`

`pdm venv` is a way to create virtual environments associated with the project... so I'm confused on the difference/distinction between the python binary referenced in `.pdm-python` and what the point of the `pdm venvs` is... it's confusing that they fit into the workflow of AFTER `pdm init` which required me to associate a python interpreter with this project in the first place
