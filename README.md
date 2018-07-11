# Python-with-Mac
Omnibus tutorial walk through setting up Python with macOS.  I'm calling this an omnibus tutorial because I am combinding links to other tutorials that do a great job at explaining certain topics already.  (So why reinvent the wheel?)  Anything I type up is to:
    - Fill in gaps inbetween tutorials and/or articles
    - Explain why/what you should read in a particular turtorial or atricle
    - Give digested information, expecially if the article or tutorial is really long and wordy for what it is explaining 
      (_no point in wasting time_).
    - Give quick reference to go back to, to advoid of having to reopen the article.

##Nomenclature I use (To avoid confusion)
1. Keystrokes:
    * If I say: `SHIFT + CTRL + c`, that means press at the same time shift, control, and the letter c.
    * If I say: `SHIFT - CTRL - c`, that means press sequentually shift, control, and the letter c.
2. Directories
    * In a directory if I use ( ) like: `/home/(user_name)/Documents/(youe_folder)`, they refer to something unique to what you named them.

#Installing Python3
Python2 comes default with OSx.  However, I recommend upgrading to seperate Python3 installation, because a seperate installation will avoid conflicts between your normal computer programs and your coding endevours.

##Python.org macOS installer (not recommended)
This method does not involve terminal and is here if you wish.  I do not recommend this because it does not expose you to terminal (something needed for PIP), you can only upgrade or revert to previous versions of python through installers, and does have the automatic tools of the **Terminal Installation Method** which ultimatly save you time.
Link to download the Latest Python 3 Release https://www.python.org/downloads/mac-osx/

##Teminal instalation Method (recommended)
**How to open terminal** section - Need to know
**Using Terminal** - can just reference
**Installing Python3 using Homebrew** - can just follow along

Yes, you can install python3 straight from python.org.  However, we are going to do a different route.  When it comes to installing and updating things on Unix like machines (like macOS), your about to be blown away how EASY it is to do with a package manager.  They are SUPPER useful ensemble of tools to automate installing, updating, configuring, and removing programs and modules.  It's helpful, but you don't need to _know_ terminal, but I do recommend becoming familiar with the couple of commands that are listed in 

###How to open Terminal
I. Quick shortcut to open terminal:
      1. type: `CMD +  SPACE` (_opens spotlight search_)
      2. type: `terminal - RETURN` (_opens terminal_)
II. GUI
      1. Open Applictions folder
      2. Open Utilities folder
      3. Open Terminal Application (you can add this to your dock)
      
###Using Termianl
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


###Installing Python3 using Homebrew
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
