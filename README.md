# Flake8 for Python 3.x incompatible use of print operator

Runs [hacking](https://github.com/openstack-dev/hacking) selecting only the error: `H233  Python 3.x incompatible use of print operator`

## Fixing H233 issues

The __2to3__ utility that ships with Python can automatically fix all print statements so that they are compatible with both Python 2 and Python 3.

At the root of your project, run `2to3 -f print .` to see all the lines that need to be changed and then run `2to3 -f print -w .` to actually write (-w) the changes into the files.

https://docs.python.org/2/library/2to3.html
