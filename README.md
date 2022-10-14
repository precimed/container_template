# Project ``container_template``

This is a template repository for singularity/dockerfile containers and build scripts

## Getting started

To use these codes, **do not** clone or fork this repository, but click the green 
[Use this template](https://github.com/espenhgn/container_template/generate)
button above.

You may then create a new repository on a GitHub organization or user account (`<user>`) under a new project name (`<project>`), 
that can be cloned by issuing in a terminal application

```
git clone git@github.com:<user>/<project>.git
cd <project>
```

The codes may then be adapted further to suit the requirements of the project, as described next

## Setup-requirements

After cloning the template repository as described above a few requirements must be in place.
Some scripts rely on [Python](https://www.python.org) with some packages available in the Python environment.

One convenient way to set up a Python environment is [Conda](https://docs.conda.io/en/latest/), available via [Miniconda](https://docs.conda.io/en/latest/miniconda.html) or [Miniforge](https://github.com/conda-forge/miniforge). 
Assuming one of these Python distributions is installed, issue one of the following to create a new Python environment using `conda`:

```
conda create -n <project> python=3 pip  # create environment named <project>
conda activate <project>  # activates enviromnent
pip install -r setup-requirements.txt
```

## Initial setup

To set up your own project from this template, issue in the terminal:
```
python scripts/init.py
```

The script is interactive, and will prompt the user for some info. 
It will modify certain files in the `<project>` directory and also replace this `README` file.
Remember to commit and push the changes after running the :
```
git commit -a -m "initial setup"
git push
```

The remaining codes may then be added to and be modified further to suit the requirements of the `<project>`.
