# Welcome.

This repository is dedicated to wind energy data analytics, with emphasis on turbine measured data, event/alarm logs, revenue meter data, and how to migrate analytic methods from notebook experiments to scheduled workflows.  It deals specifically with the issues faced by analysts of streamlining their methods and sharing code and results.

The repository is organized into several sections with folders dedicated to areas of interest, with most examples done in ipynb notebooks, in python, using polars dataframes.

### Entry level 

This section has a series of notebooks explaining primary features and manipulation of data using polars for datasets that will fit into memory. While almost all the code examples herein are simplified and overly verbose on comments, this section really does start, at the beginning, explaining about environments and showing how to deal with them.

Environment management on teams that are only loosely coordinated is even harder, so we've included example notebook formats to deal with environments that might be used in different organizations that share work or even the same organization. We'll demonstrate this concept through all notebooks in this repository.

### A starting point

Where most operational teams have access to data streams from SQL Servers or PI historians or similar data stores, the typical consultant (or student/researcher) is given or assembles data from different sources.  In an effort to save time, they start with the data in its most raw state and jump right in.  We propose first establishign a common starting point using sqlite as a data container to store and organize our datasets prior to starting. These have the benefit of keeping related data, like the different series mentioned above, organized and in a single file.  With SQLite built into python, we really don't have an excuse to be better organized.

### creating taxonomies that work 

Where the ideas for a common starting point cover its structure and management, this related section is dedicated to the content and relies on concepts introduced in:

https://wes.copernicus.org/articles/9/883/2024/ 
Knowledge engineering for wind energy.
Wind Energ. Sci., 9, 883–917, 2024
https://doi.org/10.5194/wes-9-883-2024
© Author(s) 2024.

a common task for consultants, analysts, and data scientists is aggregating or classifying data for certain characteristics.  We will add sections on how to deal with these issues and possible sources of data that are simple to assemble and use, but provide the context to ensure your assembled data is understood now and in 5 years when someone else reviews it, or reuses your data for other work.

#### Turbine manufacturer, model meta data.

In the wind energy world, a common grouping is by manufacturer and turbine model.

This simple notebook downloads data from the USGS website and identifies to the top 100 mfr/model combinations (irrespective of HH).

The purpose of the list is to serve as a high level grouping, with additional context added per turbine - hub height, controller revision, real capacity after uprates being key.


### Reference data


