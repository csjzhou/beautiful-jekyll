---
layout: post
title: 5 Matplotlib Plotting Methods
show-avatar: true
tags:
  - blogs
  - python
  - matplotlib
  - plot
published: true
---


## 5 Matplotlib Plotting Methods



* [Scatter Plot](#scatterplot)
* [Line Plot](#lineplot)

From [机器之心](https://mp.weixin.qq.com/s?__biz=MzA3MzI4MjgzMw==&mid=2650738591&idx=2&sn=be82005eedd1edf650aee0d6059c2926)

### Scatter Plot <a id="scatterplot"></a>
Draw scatterplot with scatter.

``` python
import matplotlib.pyplot as plt
import numpy as np

def scatterplot(x_data, y_data, x_label="", y_label="", title="", color = "r", yscale_log=False):

    # Create the plot object
    _, ax = plt.subplots()

    # Plot the data, set the size (s), color and transparency (alpha)
    # of the points
    ax.scatter(x_data, y_data, s = 10, color = color, alpha = 0.75)

    if yscale_log == True:
        ax.set_yscale('log')

    # Label the axes and provide a title
    ax.set_title(title)
    ax.set_xlabel(x_label)
    ax.set_ylabel(y_label)
```
----

### Line Plot <a id="lineplot"></a>
Draw lineplot.

``` python
def lineplot(x_data, y_data, x_label="", y_label="", title=""):
    # Create the plot object
    _, ax = plt.subplots()

    # Plot the best fit line, set the linewidth (lw), color and
    # transparency (alpha) of the line
    ax.plot(x_data, y_data, lw = 2, color = '#539caf', alpha = 1)

    # Label the axes and provide a title
    ax.set_title(title)
    ax.set_xlabel(x_label)
    ax.set_ylabel(y_label)

```
----
