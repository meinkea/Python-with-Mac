# Python-with-Mac
Omnibus tutorial covering setting up Python with macOS, learning Python basics, and Engineering Python packages.  This combines tutorials, documation, and articles that already do a great job at explaining certain topics already; Why reinvent the wheel?  Anything typed up is to:
    - Fill in gaps inbetween tutorials and/or articles
    - Explain why/what you should read in a particular turtorial or atricle
    - Give digested information, expecially if the article or tutorial is really long and wordy for what it is explaining 
      (_no point in wasting time_).
    - Give quick reference to go back to, to advoid of having to reopen the article for simple things.

## • Nomenclature I use (To avoid confusion)
1. Keystrokes:
    * `SHIFT + CTRL + c`, means press at the same time shift, control, and the letter c.
    * `SHIFT - CTRL - c`, means press sequentually shift, then control, then letter c.
2. Directories
    * In a directory (file path) the ( ) used for in example: `/home/(user_name)/Documents/(youe_folder)`, refer to a name unique to what you named it.  Typically an account name or user chosen file name scheme.



# Installing Python3
Python2 comes default with OSx.  However, I recommend upgrading to seperate Python3 installation, because a seperate installation will avoid conflicts between your normal computer programs and your coding endevours.  This is important because even though you can use Python2 that comes with macOS, the Python Software Fondation does not recommend changing, altering, or deleteing these file associated with it, as this installation of Python is used by Apple and third-party software. A good source for Macintosh can be found in the Python's documentation, which provides a good source of documentation about using Python on macOS.

 - Official doc: https://docs.python.org/3.7/using/mac.html

There is also the MacPython wiki,

 - Official wiki: https://wiki.python.org/moin/MacPython

Lastly, here a walk through of two methods to walk you through doing an installation of Python3, one of which I recommend over the other (the **Terminal Installation Method**).  It's less involved as it sounds, and often when you install a pacakge, it vastly easier than an installer.

## • Python.org macOS installer (not recommended)
This method does not involve terminal and is here if you wish.  I do not recommend this because it does not expose you to terminal (something needed for PIP), you upgrading or reverting to previous versions of Python is harder, does have the automatic tools of the **Terminal Installation Method** which ultimatly save you time, and I am not sure as to how seperate it keeps Python2 (macOS) and Python3 from each other.

 - Link to download the Latest Python 3 Release: https://www.python.org/downloads/mac-osx/

## • Teminal instalation Method (recommended)
 Outline
  1. **How to open terminal** section - Need to know
  2. **Using Terminal** - can just reference
  3. **Installing Python3 using Homebrew** - can just follow along

When it comes to installing and updating things on Unix like machines (like macOS), your about to be blown away how EASY it is to do with a package manager.  They are SUPPER useful ensemble of tools to automate installing, updating, configuring, and removing programs and modules.  It's helpful, but you don't need to _know_ terminal, but I do recommend becoming familiar with the couple of commands that are listed in the table under **Using Terminal**.  Lastly, Homebrew will install Python in a directory that macOS will never touch, and make it the default Python for you.  This keeps you happy, macOS happy, and it's third-party applications happy.

**1. How to open Terminal**
I. Quick shortcut to open terminal:

   1. type: `CMD +  SPACE` (_opens spotlight search_)
   2. type: `terminal - RETURN` (_opens terminal_)

II. GUI
    
   1. Open Applictions folder
   2. Open Utilities folder
   3. Open Terminal Application (you can add this to your dock)
      
**2. Using Terminal**
Command | Name | Laymen Terms 
--- | --- | ---
`pwd` | Print Working Directory | Tells you which folder you are in
`ls` | List Stuff | Shows you everything in the folder you are in
`cd` | Change Directory | Lets you move in and out of folders
`cd (folder_names)` | | Like double clicking a folder to open it
`cd ..` | | Backs out of the folder your in
`cd ~` | | ~ is short hand for homefolder

Introduction to the Mac OS X Command Line, by Jim Hoskins,

 - article: http://docs.python-guide.org/en/latest/dev/virtualenvs/#virtualenvironments-ref

**3. Installing Python3 using Homebrew**
1. Open Terminal
2. Install Homebrew package manager <br />
    `ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
3. Insert Homebrew directory at the top of your PATH enviroment variable 
    `export PATH=/usr/local/bin:/usr/local/sbin:$PATH`
4. Install Python3 using Homebrew
    `brew install python`
**Done!**

Installing Python3 on Mac OS X, by Kenneth Reitz,

 - article: http://docs.python-guide.org/en/latest/starting/install3/osx/

Now time for pip!



# Quick intro to PIP
When you installed Python3 it came with pip by default.  Pip stand for (stands for PIP installs Python); it is another wonderful package manager that comes with Python!  So once you installed it yourself, either though Homebrew or through the Installer, you'll have pip. ^-^

To use PIP, generally do this
1. open termianl
2. type `pip install (package_you_want)`
**Done!**

Let's try installing matplotlib!
`pip install matplotlib`

Go have lunch because that's it.  The only legwork you will ever need to do is to know the name of the package you want.  They can be found through google searchs, youtube, website, forum post, or other Pythoneers.  A website to bookmark is PyPi, a Python package index site where you can discover more packages.

 - Official site: https://pypi.org/

# Open IDLE (Interactive Development Enviroment)
The Python's IDLE is where you will code in Python.  You can open in one of two methods.

## 1. Applications Folder (recommended)
In your Applications folder, you should see:
IDLE - the Developement Enviroment
PythonLauncher - Handle what happens when you double click on Python scrpits (I recommend for when you are starting out, having it open the IDLE)
Build Applet - A tool too package Python scripts as standalone applications

## 2. Terminal
Type in termianl `IDLE`
note: _This is not the preffered method..._

# Learning Python
From here, watch this Python Programming tutorial series on youtube from thenewboston,

 - youtube: https://www.youtube.com/watch?v=HBxCHonP6Ro&list=PL6gx4Cwl9DGAcbMi1sH6oAMk4JHw91mC_

Even if you have a higher version like 3.7, as he used 3.4 in the tutorial, it will work just fine at showing you all the basics in Python.  I recommend watching videos (as these are what I used to learn Python).  Python is extremely powerful and has LOTS of features, data types, and high level abstracts.  However, one might not be interest in *everything* Python has to offer.  Therefore, I recommend binging the videos in the Basics column in the table below.  That way you can have more time to explore cooler libraries that pertain more to you.  The Comprehensive column is there if you wanted to know more about basic Python..

Basic | Comprehensive
--- | ---
2 | 2 _to_ 5
7 _to_ 16 _and_ 21 | 7 _to_ 21
23 | 23
29 _to_ 33 _and_ 40 | 28 _to_ 41
na | 50
na | 53 _to_ 56
18 Total | 39 Total


# Packages
Here are a list of packages you might be insterested in.

## • SciPy
A good start for computing with Python.  Involves a large collection of open source computation and ease of use libraries, which include Matplotlib, NumPy, Pandas, and SymPy. <br />
 - Official site: https://www.scipy.org/

## • Matplotlib (recommended)
Ploting library that can generate plots with few lines of code
_If you have not already_, to install: `pip install matplotlib`
Analog of ploting in matlab

A youtube series that you can pick out what exactly your interested in, by sentdex, <br />
 - youtube: https://www.youtube.com/watch?v=q7Bo_J8x_dw&list=PLQVvvaa0QuDfefDfXb9Yf0la1fPDKluPF

A continuation of the previous series, going into 3D plots, <br />
 - youtube: https://www.youtube.com/watch?v=ZlpFQNVhB7I&list=PLQVvvaa0QuDe60TfxLrJzdQEacMEItxl-

Here is a forum post talking about plotting in polar, <br />
 - youtube: https://stackoverflow.com/questions/36816537/spherical-coordinates-plot-in-matplotlib

Another comprehensive series can be found here, by Fluidic Colours, <br />
 - youtube: https://www.youtube.com/watch?v=b3lK639ymu4&list=PLNmACol6lYY5aGQtxghQTq0bHXYoIMORy <br />
(**note**: _I recommend polar plots, video number 24, as I believe this pertains to you_)

 - Official site: https://matplotlib.org/

## • Numpy (recommended)
The Python package for scientific/engineering computation.  It is convenient, fast, and uses less memory than normal Python list.  

The official tutorials for NumPy can be found here,

 - doc: https://docs.scipy.org/doc/numpy/user/quickstart.html

 - Official site: http://www.numpy.org/

Here is a link for Matlab users,

 - article: https://docs.scipy.org/doc/numpy/user/numpy-for-matlab-users.html

Cool thing, is that NumPy uses BLAS, which takes advantage of multi core CPU's (which uou need to pay for in Matlab's Parallel Computing Toolbox)

If you have a need for speed you can reinstall numpy to use more than 1 CPU, <br />
 - article: http://scipy-cookbook.readthedocs.io/items/ParallelProgramming.html

If you need EXTREME parrallel speed (like we are almost approaching super computer level), you can add CuPy to NumPy.  This library in one line of code can take your NumPy array and use your graphics card (You comp has a REALLY high end quadro card btw that is MADE for this purpose) to shread through large data sets.

 - site: https://cupy.chainer.org/

## • Pandas (recommended)
Library providing high-performance, easy-to-use data structures and data analysis tools for the Python programming language. 
It's good for relational data. Also can iteract with a ton of file formats from what I remember, like cvc, txt, excell, etc...

A youtube series showing how to use this useful library,

 - youtube: https://www.youtube.com/watch?v=Iqjy9UqKKuo

 - Official site: https://pandas.pydata.org/

## • IPython
Interactive notebook with interactive visuals and GUI toolkits.  It's leverages the flexibility of python interpreters and even has high preformance tools for parallel computing.

 - Official site: http://ipython.org/

## • Sympy
Symbolic mathematics with Python.  Has a full CAS system and aims to keep code as simple as possible.

 - Official site: http://www.sympy.org/en/index.html

## • Python Resources for NI Hardware and Software
You can take you Python scripts, and put them into a labview code.  
(Imagine putting your Matlab scripts into your Labview testing equipement)

You can have labview code wrap your Python (great for embedding Matlab like routines in your testing equipement) and/or use Python to call and wrap your labview code to interact with other equpiment, computers, servers, or data centers in your building in the cloud.

 - site: http://www.ni.com/white-paper/53059/en/

## • GSL
GNU Scientific Library is a numerical library for mainly C and C++.  But you bet you can use that in Python!

Heres a source outlining of everything this library has to offer, <br />
 - site: https://www.gnu.org/software/gsl/

## • Jupyter
Evolving from IPython, it is an open-source web application that expands apon the whole notebooks idea.
"create and share documents that contain live code, equations, visualizations and narrative text. Uses include: data cleaning and transformation, numerical simulation, statistical modeling, data visualization, machine learning, and much more."
It's writen in Python, but supports over 40 languages now.

It reminds me of Mathmatica, take a looksy, <br />
 - Official site: http://jupyter.org/

## • Matlab
If you wanna keep matlab, and you don't have to give it up.
Python can call your matlab functions and code, and use best of both worlds! <br />
 - doc: https://www.mathworks.com/help/matlab/matlab_external/call-user-script-and-function-from-python.html

If you had Matlab, Python, and Labview on the same computer, you could wrap your matlab code in Python and feed it to a labview test system.

## • Small Matlab to Python compiler, LibreMate, and OMPC
If you decided to make a complete switch over from Matlab to Python, you don't need to rewrite all of your Matlab code (although rewriting some of them would be great practice).  Instcompetesead, there are Source-to-Source Compilers.  These essentually rewrite your Matlab code into Python code, mostly using the packages mentioned earlier.

 - forum: https://stackoverflow.com/questions/9845292/a-tool-to-convert-matlab-code-to-python

## • PyVISA
PyVISA package enables you to control all kinds of measurement devices independently of the interface (ex. GPIB, RS232, USB, Ethernet, VXI, PXI etc...)

Example code with a Keithley Multimeter with GPIB number 12, only needing three lines of code
`import visa` <br />
`rm = visa.ReasourceManager()` <br />
`rm.list_resources()` <br />
`    ('ASRL1::INSTR', 'ASRL2::INSTR', 'GPIB0::12::INSTR')` <br />
`inst = rm.open_resource('GPIB0::12::INSTR')` <br />
`print(inst.query("*IDN?"))` <br />

Works on Window's Linux, and Mac. <br />
Works with arbitrary adapters like National Instruments, Agilent, Tektronix, Stanford Research Systems. <br />
Here is a good read about this,
 - article: http://pyvisa.readthedocs.io/en/stable/

## • SWIG, PyFort, ctypes, Cython, f2py and other glue librarys
You may learn that Python is a great glueing language.  Instead of reinventing the wheel or trying to be the best at everything, it can wrap around and interface with about any major language.

If you need speed of fast C, C++, or Fortran code, just use it from Python! <br />
Here is about 5 different way you can do it, <br />
 - doc: https://docs.scipy.org/doc/numpy-1.10.0/user/c-info.python-as-glue.html



# FEM
Some selected FEM softwares you can script and code with Python.

## • FEniCS Project
COMSOL cannot take Python code, how it takes Matlab code.  There is a forum, on the COMSOL website, talking about how COMSOL and Python.

 - forum: https://www.comsol.com/forum/thread/107812/python-for-comsol

I personally don't think COMSOL will ever make an API to interface with Python.  Not because Python can't, but because COMSOL probably has an agreement with Matlab.  There are more forum post talking about how people are stuck on Matlab, just because they want/need to use COMSOL.  It's just my reasoning for why based on what I have read online, and I want to make sure you don't get any false hopes.

That said, it's not all doom and gloom.  In the open-source community, if something is needed, people make it.  There are other widely known alternatives to COMSOL, Ansys, and Seimens NX.  They sometimes require computer savviness (or time spent, as it is really investment).

Meet FEniCS Project, an open-source computing platform for solive partial differential equations.  It allows you to translate engineering and scientific models into finite element code.  Written in C and C++, you can use Python or C++ to interface with FEniCS, compute, than plot/analyze the results.

 - Official site: https://fenicsproject.org/

## • Elmer
Elmer is a Muliphysics Simulation Software that competes against COMSOL.

 - Official site: https://www.csc.fi/web/elmer/elmer

It does have an accoustics module.  Here is a youtube video showing it, <br />
 - youtube: https://www.youtube.com/watch?v=dfLHVUcvnDo

Unlike COMSOL, Elmer does allow Python code to run.  You can actually choose to run you Python code as C code, or as TCL code. <br />
This wiki goes into more details, <br />
 - wiki: https://wiki.python.org/moin/elmer

A forum discussing a simulation comparison between Elmer and COMSOL, by a user,

 - forum: http://www.elmerfem.org/forum/viewtopic.php?t=4306

## • Coding COMSOL with Python
This contradicts what was said in the the past two FEM Softwares, Elmer and FEniCS Project, but you can code COMSOL with Python.  This however is a little weird to think about.  COMSOL has two API's, one for Matlab and one for Java.  You essentually use the Java API with Python, as this individual did for there thesis.

 - github: https://github.com/dilzeem/thesis/blob/master/thesis.org
  
## Others
Many other FEM softwares that can be coded with Python can be found here,

 - site: https://alternativeto.net/software/comsol/?license=opensource
 
