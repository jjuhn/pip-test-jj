# pip-test-jj

Just an exmaple library for distributing this library to pip. 

1. create account at pypi and pypi test
2. create .pypirc file in your home directory
3. Make the right python package directory structure. 
    source_dir/                 # the source directory
|-- my_python_package       # your package
|   |-- __init__.py
|   `-- FILES ....          # your package files
|-- README.md
|-- setup.cfg
|-- setup.py

4. Release on GitHub
5. Publish package on pypi-test and pypi

python setup.py register -r pypitest
python setup.py sdist upload -r pypitest

Check on Pypi Test

python setup.py register -r pypi
python setup.py sdist upload -r pypi

