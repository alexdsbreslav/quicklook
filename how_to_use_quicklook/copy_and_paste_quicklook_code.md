# Copy-and-paste code quicklook code using JupyterLab
JupyterLab and Jupyter Notebooks make it easy to copy and paste code directly into your notebook. Review these tips for making quicklook easy and efficient to use!
- **Step 1:** Make sure that quicklook is imported into your notebook. At the top of every one of my notebooks, I import quicklook along with several other key packages:
```python
import pandas as pd
import numpy as np
import os
import quicklook
```
- **Step 2:** in the next cell below type `quicklook.` and hit `tab`. When you hit `tab`, a drop-down of all of the functions in quicklook should show up. Notice that they all have a blue f next to them. This indicates that they are functions.
```python
quicklook.
```
![tab](https://github.com/alexdsbreslav/quicklook/blob/master/images/copy_paste/tab.png)

- **Step 3:** start typing out the function that you want, once it is the only one left in the list, you can hit `enter` and it will fill in the rest.
```python
quicklook.build_chart_skeleton
```

- **Step 4:** hold `shift` and hit `tab`. When you do, you should see a pop-up with the function's documentation. Scroll down to the part that says `Docstring:`. Copy everything under `Docstring:` though to the last `)`. Select the code in the cell and paste over it. The code in your cell should match what was in the `Docstring:`
![shift_tab](https://github.com/alexdsbreslav/quicklook/blob/master/images/copy_paste/shift_tab.png)

- **Step 5:** Fill in any blanks and adjust default settings in the code as needed. Hold `shift` and hit `enter` to execute the code cell and show your new chart! Notice in the code below that I changed the title, xlabel, ylabel, x_min_max, x_tick_interval, horizontal_gridlines_on, and vertical_gridlines_on from the defaults in the Docstring.
```python
chart_skeleton = quicklook.build_chart_skeleton(style = 'default', size = 'default',
title = 'Title',
xlabel = 'X-Axis Label',
ylabel = 'Y-Axis\nLabel',
x_min_max = (0,2), y_min_max = (0,1),
xtick_interval = 0.5, ytick_interval = 0.25,
horizontal_gridlines_on = True,
vertical_gridlines_on = True)
```

![chart](https://github.com/alexdsbreslav/quicklook/blob/master/images/copy_paste/chart.png)
