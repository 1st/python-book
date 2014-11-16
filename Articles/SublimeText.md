SublimeText - source code editor
==========

SublimeText is one of the best source code editors. It's easy to use, fast and extansible with plugins. If you wish to create new plugin or fix bug in one of existing plugins - you can do it - because SublimeText plugins written on Python.


Install SublimeText
----------


Install SublimeText plugins
----------

Below we modify **User Settings**. To do so open **Sublime Text -> Preferences -> Package Settings -> SublimeLinter -> Settings - User**. It opens file in new tab where you can add or modify options. Save this file and changes will be made immediately.


### Python-related plugins

[SublimeLinter](https://github.com/SublimeLinter) - this plugin is required to install all **SublimeLinter-XXX** plugins.

[SublimeLinter-flake8](https://github.com/SublimeLinter/SublimeLinter-flake8) - plugin to lint Python code and detect code complexity.

Open **User Settings** *(see above)* and add (or modify) these options:
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


### Other useful plugins

 * git
