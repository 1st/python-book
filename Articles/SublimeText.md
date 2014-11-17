SublimeText - source code editor
==========

SublimeText is one of the best source code editors. It's easy to use, fast and extansible with plugins. If you wish to create new plugin or fix bug in one of existing plugins - you can do it - because SublimeText plugins written on Python.


Install SublimeText
----------

Download latest verson of [SublimeText](http://www.sublimetext.com/3) and follow instructions for your OS. On Mac OS X you need to unzip file from archive and move it to `/home/<user>/Applications` directory.


Install SublimeText plugins
----------

Below we modify **User Settings**. To do so open **Sublime Text -> Preferences -> Package Settings -> SublimeLinter -> Settings - User**. It opens file in new tab where you can add or modify options. Save this file and changes will be made immediately.


### Python-related plugins

[SublimeLinter](https://github.com/SublimeLinter) - this plugin is required to install all **SublimeLinter-XXX** plugins.

[SublimeLinter-flake8](https://github.com/SublimeLinter/SublimeLinter-flake8) - plugin to check Python code on errors (pyflakes, pep8) and detect code complexity. Before install: `pip install flake8`. After install: open **User Settings** *(see above)* and add these options:

```python
{
    "user": {
        "linters": {
            "flake8": {
                # check code complexity (bu default no check: -1)
                "max-complexity": 10,
                # change line length from 79 to 120 symbols
                "max-line-length": 110,
            }
        }
    }
}
```

[SublimeLinter-pep257](https://github.com/SublimeLinter/SublimeLinter-pep257) - check syntax of docstring. Before install: `pip install pep257`. After install: open **User Settings** *(see above)* and add these options:

```python
{
    "user": {
        "linters": {
            "pep257": {
                # ignore "docstring for module", "white space before docsting" and "one-line docstring"
                "ignore": "D100,D200,D203"
            }
        }
    }
}
```

[SublimeJEDI](https://github.com/srusskih/SublimeJEDI) - autocomplete Python code on dot. After install: make soma changes to **User Settings** as described on plugin page.

### Other useful plugins

[SublimeLinter-html-tidy](https://github.com/SublimeLinter/SublimeLinter-html-tidy) - HTML code validator. Before install: check if your have installed `tidy` on your computer.

[SublimeLinter-jshint](https://github.com/SublimeLinter/SublimeLinter-jshint) - JavaScript code validation. Before install: see instructions on plugin page.

[SublimeLinter-csslint](https://github.com/SublimeLinter/SublimeLinter-csslint) - CSS code validator. Before install: see instructions on plugin page.

### Some extra plugins

[SublimeLinter-json](https://github.com/SublimeLinter/SublimeLinter-json) - JSON code validator.

[SublimeLinter-coffee](https://github.com/SublimeLinter/SublimeLinter-coffee) - CoffeeScript code validator. Before install: see instructions on plugin page.

See also: git, mercurial.
