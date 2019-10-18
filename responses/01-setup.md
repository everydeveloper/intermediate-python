Welcome to this (mildly) advanced Python tutorial! Today we'll be writing a script to mimic a common real-world action. If you've ever played a tabletop game, you know there are many dice rolls to make. This tutorial will show how to harness a combination of Python skills to make an automatic dice roller. But first, before we do that, we'll need to get a few things set up on your system. 

## Having Python 

First, in order to do anything in Python, you need to *have* Python on your computer! Let's make sure it's installed. Open up a terminal and type `python -V. There are a few possible things it can output here:

If the output begins with `Python 3`, you're good to go! This tutorial was tested on a system running Python 3.7.4, but it should be compatible with any version of Python 3. 

If the output begins with `Python 2`, you have Python, but it's an outdated version. You'll need to download Python 3 to follow this tutorial. Go to the [Python](https://www.python.org/downloads/) website to download it.

If you get a command that reads something similar to `command not found`, no version of Python is on your system. You'll need to go to the [Python](https://www.python.org/downloads/) website to download it.

## Having Git

We also need to make sure Git is installed on your system. Check that by typing `git --version` in a terminal. If it outputs a `git version` you're good to go! If not, go to the [Git](https://git-scm.com/downloads) website to download it.

## Cloning this Repository

Now that we have Git, we can clone the repository containing the building block of the code you'll be writing. In the terminal type `git clone {{ repoUrl }}`

Inside the repo you'll see two files:

- `README.md`: a markdown file that details some info about the project
- `dice-roller.py`: a Python file containing the code you'll be building off of

Now that we have everything we need, we can actually begin writing our dice roller! Let's begin!