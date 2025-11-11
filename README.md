[![View precipitation-variability-analysis-matlab on File Exchange](https://www.mathworks.com/matlabcentral/images/matlab-file-exchange.svg)](https://www.mathworks.com/matlabcentral/fileexchange/160986-precipitation-variability-analysis-matlab)
[![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=mathworks/Precipitation-Variability-Analysis-MATLAB&file=Tutorial_LiveScript.mlx)

* DATA UPDATE: As of **November 2025** the links to the datasets are (they have been updated in the code):
> URLpast = "https://esgf-data04.diasjp.net/thredds/dodsC/esg_dataroot/CMIP6/HighResMIP/AS-RCEC/HiRAM-SIT-HR/highresSST-present/r1i1p1f1/day/pr/gn/v20210713/pr_day_HiRAM-SIT-HR_highresSST-present_r1i1p1f1_gn_19530101-19531231.nc";

> URLproj = "https://esgf-data04.diasjp.net/thredds/dodsC/esg_dataroot/CMIP6/HighResMIP/AS-RCEC/HiRAM-SIT-HR/highresSST-future/r1i1p1f1/day/pr/gn/v20210707/pr_day_HiRAM-SIT-HR_highresSST-future_r1i1p1f1_gn_20430101-20431231.nc";

# Analyzing and Visualizing Open Precipitation Data in MATLAB®

A MATLAB® Live Script with accompanying

-   [Jupyter®
    Notebook](https://github.com/mathworks/Precipitation-Variability-Analysis-MATLAB/blob/main/Tutorial_Jupyter_Notebook.ipynb),

-   [.m
    file](https://github.com/mathworks/Precipitation-Variability-Analysis-MATLAB/blob/main/Tutorial_mfile.m)
    and

-   reproducible [capsule on Code Ocean® with DOI](https://codeocean.com/capsule/0990523/tree/v2) 

to access, process and visualize global climate (precipitation) data
from the WCRP CMIP6 (World Climate Research Programme Coupled
Intercomparison Project - Phase 6) database.

**Get started**

-   No downloads, no installations

-   **[Open directly in MATLAB Online](https://matlab.mathworks.com/open/github/v1?repo=mathworks/Precipitation-Variability-Analysis-MATLAB&file=Analyzing_and_Visualizing_Open_Precipitation_Data.mlx)**

-   Step-by-step tutorial shows how to

    -   Re-use available climate data. **Access a list of openly
        available sources** such as NASA, ECMWF, CMCC

    -   **Query and inspect the metadata** associated with these
        projects using commands directly from MATLAB (RESTful API)

    -   Avoid downloads. **Access specific data** from within the
        database directly and **avoid time-consuming downloads** of
        large data

    -   **[Read NetCDF](https://uk.mathworks.com/help/matlab/network-common-data-form.html) (\*.nc) data** from within MATLAB corresponding to
        specific geospatial parameters (e.g., temperature, precipitation
        flux, sea ice thickness, etc.) 

    -   **Filter, analyze and visualize climate data** using standard
        MATLAB functions, mapping projections, graphical tools and
        statistical methods.

    -   Let others run your code and reproduce your results quickly.
        **Publish the results on GitHub** and **make them accessible**
        using *"Open With MATLAB Online"*

    -   Allow people to cite you! **Generate a DOI** for your code by
        linking your GitHub repository to one of several DOI-generating
        sites.

-   **[Live Script](https://uk.mathworks.com/products/matlab/live-editor.html)** contains **easy-to-use menus** and **interactive
    tools**

-   Available on [**File
    Exchange**](https://uk.mathworks.com/matlabcentral/fileexchange/160986-precipitation-variability-analysis-matlab)
    for directly installing onto your MATLAB path with one click using
    the [Add-Ons
    button](https://www.mathworks.com/help/matlab/matlab_env/get-add-ons.html)

-   Accompanying [**Jupyter notebook** (.ipynb)](https://github.com/mathworks/Precipitation-Variability-Analysis-MATLAB/blob/main/Tutorial_Jupyter_Notebook.ipynb) for use in a Jupyter
    environment. More information on MATLAB kernel
    [here](https://www.mathworks.com/products/reference-architectures/jupyter.html)

-   Accompanying [**Code Ocean reproducible capsule**](https://codeocean.com/capsule/0990523/tree/v2) for one-click
    reproducibility of the code by anyone, including reviewers.

**About the WCRP-CMIP6 Database**

The [Coupled Model Intercomparison
Project](https://www.wcrp-climate.org/wgcm-cmip), began in 1995 under
the auspices of the [World Climate Research Programme
(WCRP)](https://www.wcrp-climate.org/about-wcrp/wcrp-overview). By 2024
it is in its sixth phase (CMIP6). CMIP6 coordinates independent model
intercomparison activities and their
experiments which
have adopted a common infrastructure for collecting, organizing, and
distributing output from models performing common sets of experiments.

The [Earth System Grid Federation](http://esgf.llnl.gov/) (ESGF)
maintains a global system of federated data centers that allow access to
the largest archive of model climate data world-wide. This portal
(<https://esgf-data.dkrz.de/search/cmip6-dkrz/>), hosted by the [German
Climate Computing
Centre](https://www.dkrz.de/?set_language=en&cl=en) (DKRZ),
is an interface for users to access model data that are distributed in
several data centers, also called data nodes. Such portals provide
access to the output of the climate models contributing to the next
assessment report of the Intergovernmental Panel on Climate
Change [IPCC](http://www.ipcc.ch/). 



**Required Products**

This tutorial uses the following products:

-   [MATLAB®](https://www.mathworks.com/products/matlab.html)

-   [Mapping Toolbox™](https://www.mathworks.com/help/map/index.html)

-   [Statistics and Machine Learning Toolbox™](https://www.mathworks.com/help/stats/)

This code has been developed and tested using MATLAB 2023b

**Note** This tutorial works best when delivered by a tutor. It is
important to highlight best practices when working with Open Data,
publishing Open Code or making research output reproducible.
> ***You can use [this link to download the data](https://aims2.llnl.gov/search?project=CMIP6&activeFacets=%7B%22cf_standard_name%22%3A%22precipitation_flux%22%2C%22frequency%22%3A%22day%22%2C%22source_id%22%3A%22HiRAM-SIT-HR%22%7D) used in this example from the ESGF website***
