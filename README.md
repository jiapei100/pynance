PyNance
===
Lightweight Python library for assembling and analysing
financial data. Wraps Pandas and matplotlib for maximum
ease of use in accomplishing routine tasks in working with financial data.

Dependencies
---
Tested on:
* [Python](https://www.python.org/) 2.7.8, 3.4.2
* [matplotlib](http://matplotlib.org/index.html) 1.4.2
* [NumPy](http://www.numpy.org/) 1.9.0
* [Pandas](http://pandas.pydata.org/) 0.14.1

PyNance will definitely work with other versions of Python
and Python packages. To verify that it works with yours,
simply run the unit tests for data retrieval, then try
making some charts with sample data you retrieve.

Installation
---
Download this repository, then (preferably) create
a symlink to the standard directory to which you
have Python libraries installed or (alternatively) add
the library path to your Python search path.

### Example
I keep the repository for PyNance on a flash drive. So, in order
to have access to it on my Mac, where all dependencies are
installed, I did this:

1\. Find out where my other Python packages are located:  
```python
% python
...
>>> import sys
>>> sys.path
[ ... , '/usr/local/lib/python2.7/site-packages']
```

2\. Create a symlink to the pynance subdirectory in the appropriate directory.
Note that you want to symlink to `<path>/pynance/pynance` because
`<path>/pynance` includes tests and documentation in addition
to the package code.  
```python
% cd /usr/local/lib/python2.7/site-packages
% ls
...
numpy
...
pandas
...
% ln -s /Volumes/SANDISK64/Workspace/pynance/pynance
```

3\. Use PyNance. Note: The package will take a few seconds to load because
of its dependencies. While PyNance is very lightweight,
its dependencies aren't.  
```python
% python
>>> import pynance
>>>
```
