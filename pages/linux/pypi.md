# Maintaining PyPI packages

> Maintaining packages on the Python Package Index
> More information: <https://packaging.python.org/tutorials/packaging-projects/>

- Build the package:

`python3 setup.py sdist bdist_wheel`

- Upload the package to the PyPI:

`twine upload dist/*`
