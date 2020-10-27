# denver
Denver API for Python

This API is specifically designed for python developers who want to use
advanced utilities but without coding much. The API requires you to
have minimum Python 3.8

## tools
this is a new package built into denver and now you can use every module inside it as a command line
tool. You can type the following command `python denver.tools` to get a list of available tools.

#### **WARNING**
The tools.cpic_editor is still a work in progress


## colored text (denver.ctext)
Colored console output have been a problem since long but here at denver API, we provide
cross-platform colored console output in almost any console. we also provide emulated
print and input function with extra keyword arguments for coloring and customizing. the
default print and input function of you code can be switched out to these one by
```python
from denverapi import ctext

print = ctext.print
input = ctext.input

# You can do the same with input
print("Hello", "World in colored", "text", fore="green", back="white", style="bright")
print("Hello", "World in simple", "environment")
```

## Installation
The package can be installed by
```commandline
pip install denverapi
```
and upgraded by
```commandline
pip install --upgrade denverapi
```

## Documentation
Documentation for denver can be found out at [this page](https://xcodz-dot.github.io/denverdocs) (*currently in progress
and may not be visible for some time*).
Also Documentation provided with this project can be used but you will have to install mkdocs
by the following command
```commandline
pip install mkdocs
```
or if you already have then you can upgrade it by following command
```commandline
pip install --upgrade mkdocs
```
After installation cd to `./docs/` and run this command `mkdocs build` or if you want to edit `mkdocs serve` and then 
you can edit any file (any file edited during `mkdocs serve` will be reflected on server every time you save a file)

## Community
This is a community driven project and accepts pull requests
of any kind (read [CONTRIBUTING.md](https://github.com/xcodz-dot/denver/blob/master/.github/CONTRIBUTING.md)), Thanks to all the contributors. Contributions are appreciated 

## Fixed Bugs
### 2.1.0
* `denver.pysetup.find_package_data` function is now fixed so it can include files at root level of a module

## What's New
### 2.2.0
* new indev tools
* renamed to a new project
### 2.1.0
* `denver.tools` package is now added as a standard interface to many modules (Many tools are still work in progress)