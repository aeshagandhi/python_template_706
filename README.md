# python_template_706
Task: create the Python Template project for Data Engineering Systems (IDS 706)


This repository creates a sample hello.py file and uses a Makefile to run requirement installations/setup, linting, and testing.
The files included in this repository are: 
1. README.md
2. Makefile
3. hello.py
4. test_hello.py
5. requirements.txt
6. main.yaml

Setup Instructions:
1. First clone this Github repository locally.
2. Run ```make install``` to install necessary dependencies.

Additionally, following commands can be run to try the makefile commands:

make test

make format

make lint

make clean



There is a github action/workflow in place via main.yaml which deals with setting up python, installing dependencies, and linting. This workflow runs on pull/push requests. 


Below is the successful build/test_badge:
[![Python Template for IDS706](https://github.com/aeshagandhi/python_template_706/actions/workflows/main.yml/badge.svg)](https://github.com/aeshagandhi/python_template_706/actions/workflows/main.yml)


Usage Examples:
hello.py contains two functions: say_hello, which returns a greeting message to students in the IDS class, and add, which returns the sum of two numbers. To use the functions in another file, do the imports and then the functions can be called. For example: 
```python
from hello import say_hello, add
say_hello("Aesha")
add(1,3)
```

Pytest can be used via python to run the test_hello.py as following:  
```
python3 -m pytest -vv --cov=hello test_hello.py
```

