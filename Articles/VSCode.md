# Visual Studio Code

**Visual Studio Code** is a good code editor with support of **Python** and extended features such as code Debuging.
It looks very similar to Sublime Text, works fast and extendable with extensions. Code autocomplition works fine,
allowing to see variable names and function descriptions.

## Configure Visual Studio Code

### Install requirements on MacOS

```bash
# First of all be sure that HomeBrew installed and up-to-date.
brew doctor
brew update
brew upgrade

# Install ctags to use 'Go to Symbol' functionality.
brew install ctags

# Create virtualenv with python packages for VS Code.
mkvirtualenv workspace
# And install required packages for Python support.
pip install pylint
```

### Install extensions for Visual Studio Code

Open Extensions sidebar and install next:
- `Python` - extension for improved support of Python code
