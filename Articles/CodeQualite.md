Create hight-quality code on Python
==========

In this chapter we will discuss about how to create better code on Python, how to check your code on errors and how to find too conplex parts of your source code.


Check code on errors
----------

Linter is a program that check your source code and show found errors and warnings. Linters exists for different languages like JavaScript and CoffeScript, HTML and CSS, SASS and LESS, as well as for Python.

For Python is good choice is **flake8** because it has multiple checkers under the hood (including **pep8**). You can run checker in command like, but we recommend to use it in [SublimeText](Article/SublimeText.md) code editor to check your code on errors and warnings while you type code in code editor.


Check code complexity
----------

When you write source code you can forget about simplisity of your code. To help you find complex code parts and simplify them - you can use complexity checker.

This [article on wikipedia](https://en.wikipedia.org/wiki/Cyclomatic_complexity) tell about what is code complexity by McCabe. To create easy to support code we need to produce source code with low complxity. If your function is too big - you can divide it to multiple functions that do less and focused on one main goal.

You can check Python source code complexity with **flake8** by adding option `--max-complexity` when run code check. But do it in command line 0 isn't a good idea. It's why we have good plugins for [SublimeText](Article/SublimeText.md) to check code complexity when you type it in code editor.
