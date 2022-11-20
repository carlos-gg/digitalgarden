---
title: "Python"
---

> Python is a programming language that lets you work quickly and integrate systems more effectively


## Resources
- https://www.python.org/
- https://github.com/vinta/awesome-python
- https://github.com/DjangoEx/python-engineer-roadmap
- https://github.com/FavioVazquez/ds-cheatsheets/tree/master/Python
- https://github.com/ujjwalkarn/DataSciencePython
- [Optimizing Python code performance with cProfile](https://blog.alookanalytics.com/2017/03/21/python-profiling-basics/)
- [Consistent Python code with Black](https://www.mattlayman.com/blog/2018/python-code-black/)
- [Writing proper classes](https://aboucaud.github.io/slides/2016/python-classes)
- [Compiled C or Fortran to Python](http://people.duke.edu/~ccc14/sta-663/FromCompiledToPython.html)
- [Using Python as glue](https://docs.scipy.org/doc/numpy-1.13.0/user/c-info.python-as-glue.html)
- [Extending Python with Compiled Code](https://github.com/AstroHackWeek/AstroHackWeek2014/blob/master/day4/ExtendingPython.ipynb)
- [Wrapping C/C++ for Python](https://intermediate-and-advanced-software-carpentry.readthedocs.io/en/latest/c++-wrapping.html)

### Python and open source for science
- [Open source Science (IBM)](https://opensource.science/)
	- https://opensource.science/open-source-science-white-paper-c4940a0e9098
- [Python-for-Scientists](https://github.com/TomNicholas/Python-for-Scientists)
- [pyOpenSci](https://www.pyopensci.org/)
	- pyOpenSci promotes open and reproducible research through peer-review of scientific Python packages
- [Python for Scientific Computing](https://www.msi.umn.edu/tutorials/python-scientific-computing)

### Package management systems
- [Pip](https://pip.pypa.io/en/stable/#)
	- https://stackoverflow.com/questions/19048732/python-setup-py-develop-vs-install
	- https://pip.pypa.io/en/stable/cli/pip_install/
	- Pip local develop install. Instead of python setup.py install, use: `python -m pip install --no-deps .`
- [Conda](https://docs.conda.io/en/latest/)
- [Mamba](https://github.com/mamba-org/mamba) - The Fast Cross-Platform Package Manager
- [Miniforge and mambaforge](https://github.com/conda-forge/miniforge)

### Package publishing
- [Python Packaging User Guide](https://packaging.python.org/en/latest/)
- [Packaging Your Code](https://docs.python-guide.org/shipping/packaging/)
- [Python code packaging for scientific software](https://pythonpackaging.info/)
- [Pypi](https://pypi.org/)
- https://realpython.com/pypi-publish-python-package/#publish-your-package-to-pypi
```
python -m build
twine check dist/*
twine upload -r testpypi dist/*   # TESTING
twine upload dist/*
```

## Books
- #BOOK [Learning Scientific Programming with Python (Hill 2020)](https://scipython.com/about/the-book/)
- #BOOK [Problem Solving with Algorithms and Data Structures using Python (Interactive book)](https://runestone.academy/runestone/books/published/pythonds/index.html)
- #BOOK [Large Scale Machine Learning with Python (Sjandin 2016, PACKT)](https://www.packtpub.com/big-data-and-business-intelligence/large-scale-machine-learning-python)
- #BOOK [From Python to Numpy (Rougier 2017)](http://www.labri.fr/perso/nrougier/from-python-to-numpy/)


## Courses
- #COURSE [Python para principiantes (Microsoft)](https://learn.microsoft.com/es-es/training/paths/beginner-python/)
- #COURSE [Data Structures & Algorithms - Python](https://pythonschool.net/category/data-structures-algorithms.html)
- #COURSE [Python in High Performance Computing](https://www.futurelearn.com/courses/python-in-hpc)
- #COURSE [Scientific Computing with Python](https://www.freecodecamp.org/learn/scientific-computing-with-python/)
- #COURSE [SoloLearn Python 3 Tutorial](https://www.sololearn.com/Course/Python/)
- #COURSE [Learn Python by Example - Learneroo](https://www.learneroo.com/modules/65/nodes/366)


## Code
> Most of the code entries in this digital knowledge garden are in Python. Just look around!

### Package documentation
- https://realpython.com/documenting-python-code/
- [Documenting Python code](https://aboucaud.github.io/slides/2016/python-docstrings)
- #CODE [Mkdocs](https://github.com/mkdocs/mkdocs/)
	- [Mkdocstrings](https://github.com/mkdocstrings/mkdocstrings)
		- https://mkdocstrings.github.io/
	- [Pytkdocs](https://github.com/mkdocstrings/pytkdocs)
	- [docstring_parser](https://github.com/rr-/docstring_parser)
	- [mkapi](https://github.com/daizutabi/mkapi) - A documentation generation tool for MkDocs
- #CODE [Pdoc](https://pdoc.dev/)
	- [How to Generate Professional API Docs in Minutes from Docstrings](https://towardsdatascience.com/how-to-generate-professional-api-docs-in-minutes-from-docstrings-aed0341bbda7)
- #CODE [mkgendocs](https://github.com/davidenunes/mkgendocs)
	- https://towardsdatascience.com/five-tips-for-automatic-python-documentation-7513825b760e

### Packaging and dependency management
- #CODE [Poetry](https://github.com/python-poetry/poetry)
	- https://python-poetry.org/