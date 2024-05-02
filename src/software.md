## Intro
This year's robot code is written in Python, meaning that it is deployed to the robot in source form and interpreted by a Python runtime directly on the RoboRIO. This process requires several things to be in place on the development computer. This document will guide you through the process of setting this system up. 

## Prerequisites
- Laptop computer
- Operating system: Windows version >=8.1 OR POSIX-compliant OS (MacOS, Linux, etc.) All are fully supported, but Mac and Linux are significantly easier to set up. 
- Python installation >=3.11.0: [download](https://www.python.org/downloads/) or install from package manager
- Git installation
- GitHub account
- Text editor (If you don't have one, Team 801 recommends [Visual Studio Code](https://code.visualstudio.com/). If you're feeling particularly adventurous, try [Helix](https://helix-editor.com/)).
- General command line usage abilities (basic)

Not having any of these things will *most likely* hinder your ability to contribute to the team's code.


## Steps
1. Install Poetry
	- Poetry is a virtual environment manager that Team 801 uses for its project packaging. It makes dependency management simpler for our developers. 
	- Install Poetry with your package manager of choice, or follow their [online instructions](https://python-poetry.org/docs/#installing-with-the-official-installer)
2. Clone the Git repository
	- Our team uses a version control system called Git to manage changes to our codebase. Git is an industry standard for version management, so it is in your best interest to learn its use. Contributing to the team's code will be fairly difficult without a basic working knowledge of Git. 
	- GitHub is a repository hosting service, distinct from the version management software called Git. 
	- Authenticate GitHub in your Git installation: [Instructions](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/about-authentication-to-github#authenticating-with-the-command-line )
	- Clone our repository. Navigate to the repository's webpage on GitHub, then click the green button titled "Code" to clone. Follow GitHub's official instructions for this step. Remain on branch `main`.
3. Set up the Poetry environment
	- Navigate to the repository root via the command line and run `poetry install` to install the Poetry virtual environment and all development dependencies. 
	- Run `poetry shell` to enter the development environment. 
4. Install pre-commit hooks
	- While inside the Poetry environment, run `pre-commit install` to install the pre-commit hooks for linting, formatting, and type checking. This will set up automatic inspection of your code before you commit changes to Git. 
5. Set up your editor
	- If you're using Visual Studio Code, install the official Python extension pack. Set its Python interpreter to be the Poetry environment for this project. Our team members are able to help you with this setup process. 
	- If you're not using Visual Studio Code, you are assumed to be capable of configuring your own system. However, several of our team members use nonstandard editor setups, and we are *probably* willing to assist you in configuring your computer. 

## Now what?
If you've followed the above steps, move on to the page about writing code and deploying to the robot. 

### Authors
This page was authored by Ishaan Sen.
