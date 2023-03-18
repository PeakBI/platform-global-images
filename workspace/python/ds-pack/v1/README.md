# workspace-python-ds-pack-v1
This is the Python Data Science pack image made for Workspaces. 
The image runs a [Jupyterhub](https://jupyter.org/hub) server that has [PyCharm](https://lp.jetbrains.com/projector/) and [VSCode](https://github.com/coder/code-server) pre-installed with all of the essential and most used packages.

## Image details
### Base image
This image uses [python:3.10-bullseye](https://hub.docker.com/layers/library/python/3.10-bullseye/images/sha256-a4fbd0cbe6e333ed05a2af41d0771aecc90ad804fe8a58023c52265ad2bfea36?context=explore) as its base which is maintained by [the Docker Community](https://github.com/docker-library/python).

### OS and other details
```
Debian         GNU/Linux 10 (buster)
Linux Kernel   5.10.104-linuxkit
Python         3.10.10
```

### Important Linux packages installed
```
aws-cli        2.7.20
curl           7.74.0
git            2.30.2
jq             1.6-2.1
nano           5.4-2
vim            8.2.2434-3
fish           3.1.2-3
zsh            5.8-6
R              4.2.3
node           18.15.0
docker         23.0.1
htop           3.0.5-7
pandoc         2.9.2.1-1
less           551-2
latex          3.14159265-2.6-1.40.21
libpq-dev      13.9-0
```

### Python libraries installed
```
ipywidgets                          8.0.4
jupyter-server-proxy                3.2.2
jupyterhub                          3.1.1
jupyterlab-git                      0.41.0
jupyterlab-lsp                      4.0.0
jupyterlab                          3.6.1
jupyterlab_widgets                  3.0.5
jupytext                            1.14.5
lckr-jupyterlab-variableinspector   3.0.9
mypy-ls                             0.5.1
nbconvert                           7.2.10
notebook                            6.5.3
pyls-black                          0.4.7
pyls-flake8                         0.4.0
pyls-isort                          0.2.2
pyls-mypy                           0.1.8
python-lsp-black                    1.2.1
python-lsp-server[all]              1.7.1
virtualenv                          20.21.0
```

## Building the image
To build the image locally, run the docker build command and pass in the required build arguments:
```
docker build . -t workflow-python-ds-pack-v1
```

## Using the image
To use the image, select it when configuring the Workspace.
If you need to install additional dependencies or add some use case specific environment variables, it can be easily extended.
