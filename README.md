# Python-with-Mac
Omnibus tutorial walk through setting up Python with macOS.  I'm calling this an omnibus tutorial because I am combinding links to other tutorials, documation, and articles that already do a great job at explaining certain topics already.  (So why reinvent the wheel?)  Anything I type up is to:
    - Fill in gaps inbetween tutorials and/or articles
    - Explain why/what you should read in a particular turtorial or atricle
    - Give digested information, expecially if the article or tutorial is really long and wordy for what it is explaining 
      (_no point in wasting time_).
    - Give quick reference to go back to, to advoid of having to reopen the article.

## Nomenclature I use (To avoid confusion)
1. Keystrokes:
    * If I say: `SHIFT + CTRL + c`, that means press at the same time shift, control, and the letter c.
    * If I say: `SHIFT - CTRL - c`, that means press sequentually shift, control, and the letter c.
2. Directories
    * In a directory if I use ( ) like: `/home/(user_name)/Documents/(youe_folder)`, they refer to something unique to what you named them.

# Installing Python3
Python2 comes default with OSx.  However, I recommend upgrading to seperate Python3 installation, because a seperate installation will avoid conflicts between your normal computer programs and your coding endevours.  This is important because even though you can use Python2 that comes with macOS, the Python Software Fondation does not recommend changing, altering, or deleteing these file associated with it, as this installation of python is used by Apple and third-party software. A good source for Macintosh can be found in the python's documentation, which provides a good source of documentation about using Python on macOS.
sauce: https://docs.python.org/3.7/using/mac.html

There is also the MacPython wiki
sauce: https://wiki.python.org/moin/MacPython

Lastly, here a walk through of two methods to walk you through doing an installation of Python3, one of which I recommend over the other (the **Terminal Installation Method**).  It's less involved as it sounds, and often when you install modules it vastly easier using pip in terminal.

## Python.org macOS installer (not recommended)
This method does not involve terminal and is here if you wish.  I do not recommend this because it does not expose you to terminal (something needed for PIP), you upgrading or reverting to previous versions of python is harder, does have the automatic tools of the **Terminal Installation Method** which ultimatly save you time, and I am not sure as to how seperate it keeps Python2 (macOS) and Python3 from each other.
Link to download the Latest Python 3 Release https://www.python.org/downloads/mac-osx/

## Teminal instalation Method (recommended)
General Guide
**How to open terminal** section - Need to know
**Using Terminal** - can just reference
**Installing Python3 using Homebrew** - can just follow along

When it comes to installing and updating things on Unix like machines (like macOS), your about to be blown away how EASY it is to do with a package manager.  They are SUPPER useful ensemble of tools to automate installing, updating, configuring, and removing programs and modules.  It's helpful, but you don't need to _know_ terminal, but I do recommend becoming familiar with the couple of commands that are listed in the table under **Using Terminal**.  Lastly, Homebrew will install Python in a directory that macOS will never touch, and make it the default Python for you.  This keeps you happy, macOS happy, and it's third-party applications happy.

### How to open Terminal
I. Quick shortcut to open terminal:
      1. type: `CMD +  SPACE` (_opens spotlight search_)
      2. type: `terminal - RETURN` (_opens terminal_)
II. GUI
      1. Open Applictions folder
      2. Open Utilities folder
      3. Open Terminal Application (you can add this to your dock)
      
### Using Termianl
Command | Name | Laymen Terms 
--- | --- | ---
`pwd` | Print Working Directory | Tells you which folder you are in
`ls` | List Stuff | Shows you everything in the folder you are in
`cd` | Change Directory | Lets you move in and out of folders
`cd (folder_names)` | | Like double clicking a folder to open it
`cd ..` | | Backs out of the folder your in
`cd ~` | | ~ is short hand for homefolder

Sauce: Introduction to the Mac OS X Command Line (Jim Hoskins)
http://docs.python-guide.org/en/latest/dev/virtualenvs/#virtualenvironments-ref


### Installing Python3 using Homebrew
1. Open Terminal
2. Install Homebrew package manager
    `ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
3. Insert Homebrew directory at the top of your PATH enviroment variable 
    `export PATH=/usr/local/bin:/usr/local/sbin:$PATH`
4. Install Python3 using Homebrew
    `brew install python`
**Done!**

sauce: Installing Python3 on Mac OS X (Kenneth Reitz)
http://docs.python-guide.org/en/latest/starting/install3/osx/


So lets introduce you to pip 

# Quick intro to PIP
When you installed Python3 it came with pip by default.  Pip stand for (stands for PIP installs Python); it is another wonderful package manager that comes with python!  So once you installed it yourself, either though Homebrew or through the Installer, you'll have pip. \^-^/

To use PIP, generally do this
1. open termianl
2. type `pip install (module_you_want)`
**Done!**

Let's try installing matplotlib!
`pip install matplotlib`

Go have lunch because that's it.  Realistically, the only legwork you'll need to do is just know the name of what you want, but you'll eventually get to know them because you use them so often, google search, website, forum post, or you hear about them from a friend.Here are some sources for places where you can discover more modules:


# Open IDLE (Interactive Development Enviroment)
The Python's IDLE is where you will code in python.  You can open in one of two methods.

##Applications Folder (recommended)
In your Applications folder, you should see:
IDLE - the Developement Enviroment
PythonLauncher - Handle what happens when you double click on python scrpits (I recommend for when you are starting out, having it open the IDLE)
Build Applet - A tool too package Python scripts as standalone applications

##Terminal
Type in termianl `IDLE`
note: _This is not the preffered method..._

#Learning Python

#Start Learning Python
From here, watch this Python Programming tutorial series on youtube from thenewboston
https://www.youtube.com/watch?v=HBxCHonP6Ro&list=PL6gx4Cwl9DGAcbMi1sH6oAMk4JHw91mC_
##Basics
Even if you have a higher version like 3.7, as he used 3.4 in the tutorial, it will work just fine at showing you all the basics in python.  I recommend watching videos (these are what I used to learn python).  Python is extremely powerful and has LOTS of features, data types, and high level abstracts.  However, one might not be interest in *everything* python has to offer, and you are prolly going to become bord after a while learning the basics.  So there's no point learning it all at once by watching these video as your not going to remeber it all.  Therefore, I recommend binging these at first (like your binging a Netflix series) and than only watching 2-3 vids a week after that.  That way you can explore cooler things like the libraries past this point.

Basic | Comprehensive
--- | ---
2 | 2 _to_ 5
7 _to_ 16 _and_ 21 | 7 _to_ 21
23 | 23
29 _to_ 33 _and_ 40 | 28 _to_ 41
| 50
| 53 _to_ 56
18 Total | 


##Matplotlib
Ploting library that can generate plots with few lines of code
_If you have not already_, to install: `pip install matplotlib`

A youtube series that you can pick out what exactly your interested in, by sentdex:
https://www.youtube.com/watch?v=q7Bo_J8x_dw&list=PLQVvvaa0QuDfefDfXb9Yf0la1fPDKluPF

Another comprehensive series can be found here, by Fluidic Colours:
https://www.youtube.com/watch?v=b3lK639ymu4&list=PLNmACol6lYY5aGQtxghQTq0bHXYoIMORy
(**note**: _polar plots are video number 24_)

Offical website for Matplotlib
sauce: https://matplotlib.org/
It also has some notes for Matlab Users

##Numpy

http://www.numpy.org/

Here is a link for Matlab users.



##Pandas 
Library providing high-performance, easy-to-use data structures and data analysis tools for the Python programming language. 
It's good for relational data.

sauce: https://pandas.pydata.org/

