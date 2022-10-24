# Data Visualization

Data visualization is an interdisciplinary field that deals with the graphic representation of data and information. It is a particularly efficient way of communicating when the data or information is numerous as for example a time series.

## What is Matplotlib?

Matplotlib is the "grandfather" library of data visualization with Python. It was created by John Hunter. He created it to try to replicate MatLab's (another programming language) plotting capabilities in Python. Matplotlib is probably the single most used Python package for 2D-graphics. It provides both a very quick way to visualize data from Python and publication-quality figures in many formats.


* Installing Matplotlib

`pip install matplotlib`


* Importing and using matplotlib
```
import matplotlib.pyplot as plt # Importing it
%matplotlib inline # to see plots in the notebook
```
### Plot types 
1. scatter
2. hist
3. boxplot

## Seaborn

Seaborn is a library for making statistical graphics in Python. It builds on top of matplotlib and integrates closely with pandas data structures.



* Installing  Seaborn

`pip install seaborn`


* Importing Seaborn

`import seaborn as sns`

## Bokeh 
 an interactive visualization library for modern web browsers. It provides elegant, concise construction of versatile graphics, and affords high-performance interactivity over large or streaming datasets. Bokeh can help anyone who would like to quickly and easily make interactive plots, dashboards, and data applications.

* Import bokeh

```
from bokeh.io import output_notebook, show
output_notebook()
```


# Refrences 
1. GitHub - rougier/matplotlib-tutorial: Matplotlib tutorial for beginner. (n.d.). GitHub. Retrieved October 24, 2022, from https://github.com/rougier/matplotlib-tutorial
2. User guide and tutorial — seaborn 0.12.1 documentation. (n.d.). Retrieved October 24, 2022, from https://seaborn.pydata.org/tutorial.html
3. Jupyter Notebook. (n.d.). Retrieved October 24, 2022, from https://notebooks.gesis.org/binder/jupyter/user/bokeh-bokeh-notebooks-8ik5f34e/notebooks/tutorial/00+-+Introduction+and+Setup.ipynb