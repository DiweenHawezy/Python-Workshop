# Python-Workshop #

## Setup ##

To begin, we need to install Python and an integrated development environment (IDE).

Lets begin by installing Python and a corresponding Package manager, conda/mamba. This allows you to create 'environments' where you work, using selected 'packages' (code libraries that do specific things as plugins to Python)

We begin by getting installing the correct version of Mambaforge for our system:

https://github.com/conda-forge/miniforge

Scroll down to the download section and select Mambaforge, with the link for your system. Linux, Mac or Windows. Install it with the following settings:

* Just for me
* We can use the default destination folder (unless you specifically want a different destination)
* Create start menu shortcuts
* register mambaforge as my default python 3.9
* clear the package cache upon completion

That should install the package manager for Python. 

The next step is to create a Python environment. 

Click start, run the 'miniforge' cmd terminal. At the commandline, run the following command to create an environment called 'Data' with python version 3.10:

**conda create --name Data python=3.10**

This will download a number of packages including Python. Type **'y'** to give consent to install them when prompted.

We will now install packages required to do some analysis into our new environment. Let's activate it by typing hte following:

**conda activate Data**

You'll notice on the left where it said **(base)** it now says **(Data)** signalling we have now in this environment.

We will begin by installing packages. Mamba works as a subsitute for conda - where we can install packages in parallel instead of sequentially. We will install several packages at once. Type the following:

**mamba install pandas numpy matplotlib seaborn geopandas ipykernel openpyxl**

Type *'y'* when prompted. Notice that it will also install many other packages that these packages depend on. 
