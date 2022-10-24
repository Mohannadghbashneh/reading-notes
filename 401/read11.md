# Data Visualization
Data visualization is a field in data analysis that deals with visual representation of data.
It graphically plots data and is an effective way to communicate inferences from data.


## Matplotlib

Matplotlib is a Python package for 2D-graphics, used for visualizing data.
- IPython

IPython is an enhanced interactive Python shell that has lots of interesting features including named inputs and outputs, access to shell commands, improved debugging and much more. It allows interactive matplotlib sessions that have Matlab/Mathematica-like functionality.

- pyplot

pyplot provides a convenient interface to the matplotlib object-oriented plotting library. It is modeled closely after Matlab(TM). Therefore, the majority of plotting commands in pyplot have Matlab(TM) analogs with similar arguments.

#### important method
|**Method**|**Use**|
|----------|-------|
|plt.ylabel()|Allows naming the y axis|
|plt.xlabel()|Allows naming the x axis|
|plt.axis()|Allows specifying the min and max of each axis|
|plt.title()|Allows specifying a title for the plot|
|plt.grid()|Allows enabling and disabling the grid for the plot|
|plt.text()|Allows placing a text in a specific point|

## Seaborn

Seaborn is a Python data visualization library based on matplotlib. It provides a high-level interface for drawing attractive and informative statistical graphics.

Seaborn is a library for making statistical graphics in Python. It builds on top of matplotlib and integrates closely with pandas data structures.

Seaborn helps you explore and understand your data. Its plotting functions operate on dataframes and arrays containing whole datasets and internally perform the necessary semantic mapping and statistical aggregation to produce informative plots. Its dataset-oriented, declarative API lets you focus on what the different elements of your plots mean, rather than on the details of how to draw them.



## Bokeh

Bokeh is an interactive visualization library that targets modern web browsers for presentation. It is good for:

- Interactive visualization in modern browsers
- Standalone HTML documents, or server-backed apps
- Expressive and versatile graphics
- Large, dynamic or streaming data
- Easy usage from python (or Scala, or R, or...)

Bokeh is an interactive visualization library for modern web browsers. It provides elegant, concise construction of versatile graphics, and affords high-performance interactivity over large or streaming datasets. Bokeh can help anyone who would like to quickly and easily make interactive plots, dashboards, and data applications.