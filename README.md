# Welcome.

This repository is dedicated to wind energy data analytics, with emphasis on turbine measured data, event/alarm logs, revenue meter data, and how to migrate analytic methods from notebook experiments to scheduled workflows.  It deals specifically with the issues faced by analysts of streamlining their methods and sharing code and results.

The repository is organized into several sections with folders dedicated to areas of interest, with most examples done in ipynb notebooks, in python, using polars dataframes.

### Entry level 

This section has a series of notebooks explaining primary features and manipulation of data using polars for datasets that will fit into memory. While almost all the code examples herein are simplified and overly verbose on comments, this section really does start, at the beginning, explaining about environments and showing how to deal with them.

#### Environment management

Environment management on teams that are only loosely coordinated is even harder, so we've included example notebook formats to deal with environments that might be used in different organizations that share work or even the same organization. We'll demonstrate this concept through all notebooks in this repository.

### A starting point

Where most operational teams have access to data streams from SQL Servers or PI historians or similar data stores, the typical consultant (or student/researcher) is given or assembles data from different sources.  In an effort to save time, they start with the data in its most raw state and jump right in.  We propose first establishing a common starting point using sqlite as a data container to store and organize our datasets prior to starting. These have the benefit of keeping related data, like the different series mentioned above, organized and in a single file.  With SQLite built into python, we really don't have an excuse to not be better organized.

### Creating taxonomies that work 

Where the ideas for a common starting point above cover its structure and management, this related section is dedicated to the content and relies on concepts introduced in:

https://wes.copernicus.org/articles/9/883/2024/ 
Knowledge engineering for wind energy.
Wind Energ. Sci., 9, 883–917, 2024
https://doi.org/10.5194/wes-9-883-2024
© Author(s) 2024.

A common task for consultants, analysts, and data scientists is aggregating or classifying data with certain characteristics.  We will add sections on how to deal with these issues and possible sources of data that are simple to assemble and use, but provide the context to ensure your assembled data is understood now and in 5 years when someone else reviews it, or reuses your data for other work.  your 'meta' data is as important as the datasets with which you are working.

#### Turbine manufacturer, model meta data.

In the wind energy world, a common grouping is by manufacturer and turbine model.

This simple notebook downloads data from the USGS website and identifies to the top 100 mfr/model combinations (irrespective of HH).

The purpose of the list is to serve as a high level grouping, with additional context added per turbine - hub height, controller revision, real capacity after uprates being key.


### Reference data

A significant portion of this repository is dedicated to practical examples. In this section we start with code to download ERA5 data from CDS for the Kelmarsh wind farm. This site, along with a few others, are used throughout the analytics portion, so we've started here, with getting an imporant supplemental dataset.



### Analytics

Step by step examples will be provided for all major steps associated with cleaning and classifying turbine operational data from both performance and health perspectives



### Process

With multiple examples in the sections above, we will next delve into process management. The goal of of the program features outlined above is to allow new methods to be created and refined, but a notebook is a temporary stepping stone and we'll cross the bridge of reaching a mature process and what to do next, providing examples of automated pipelines.


