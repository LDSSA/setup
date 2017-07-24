## Configure Anaconda3's Python distribution

## Target audience
This tutorial is for you if, like me:
- You are using Windows 10 with Python to develop Data Science contents.
- You want to use Anaconda3 as default, <b> currently </b> regarded as one of the best Data Science Python Distributions (and non Python :) ).

## Description of the Problem
When some users install Anaconda3 in their windows environment, the install recommends not to add Anaconda3 to %PATH% (Windows environment variable). Users often will follow the given suggestion.
After installation, some Pythpn power users like to use their "old" but also "fast" workflows and tools, like "Sublime Text 3" and have access to Command Prompt Python.
Since it wasn't added anything to %PATH% these tools will not recognize Anconda3 Python as their default Python interpreter.
The simple solution, which can be obvious for any experienced user, may be a bit complicated and time consuming to find out for the beginner.

## Solution
i) Verify if there is already a python.exe in %PATH% from other Python distributions you already have installed, that can obfuscate Anaconda3's.
- So press "Windows key + S" to open windows search;
- Type cmd for locating DOS like windows shell;
- Right-click with mouse and choose "Run as Administrator";
- type in cmd GUI: "echo %PATH%" which will output all the Windows Environment Variable %PATH% folders;
- type after: "where python" it will display any folder that gives direct access to Python;

ii) If any folder was found the options are to either:
- uninstall the competing distribution;
OR
- rename the Python.exe to Python3.exe or Python2.exe;

iii) Now configure Anaconda3's Python in windows as default:
- open windows explorer
- right-click the "This PC" folder (not the shortcut) and select Properties
- go to "Advanced System Settings"
- now select "Environment Variables"
- Select Path Variable in either User Environment (only affects current user) or Windows (will change for all users)
- Click Edit button, then new, and browse to Anaconda3's installation folder then add it into %PATH%
- Click ok.

iv) In sublime text you have to uninstall any Package that compiles Python with the name "Python" build, which is the name that is used by default system.

Done Enjoy!



make sure no other python.exe is available (type in cmd: echo %PATH% then type: where python) if there is you must rename or uninstall that distribution. 
ii) Now add Anaconda3 folder to %PATH%, and voilá.
























## IMPORTANT

Once you have completed the setup, mark yourself as such on [this spreadsheet](https://docs.google.com/spreadsheets/d/1SYn38h_DNzdyrZsDH4y50U32eDMdoi00cNDdn2MHAsE/edit?usp=sharing).

If you know what you're doing in terms of python, there's a `requirements.txt` that you can
use as you would like. Alternatively if you like Docker, there's [install instructions](https://github.com/LDSSA/setup/wiki/Alternate-install-methods)
for it in the wiki. If that's the case the only thing you really need to do is make sure
you can run the `Verify great success.ipynb` notebook in this repo and you are good.

## How to use this repo

This repository is the one that you will use to make sure you can execute
all of the critical tasks required to make the most of your learning
experience. In particular, after following this readme, you should:

1. Have a GitHub acount
1. Be able to clone a git repository
1. Be able to start a jupyter notebook with python 3
1. Run code within a jupyter notebook to (among other things) render some plots.

## Prerequisites

Please note that these are conservative estimates. If you
are not 100% on any of these (except for the last), you should still be okay.

- ~1GB of free memory on your computer
- Some hundreds of megabytes free on your computer
- 64-bit processor
- The ability to read a README and follow the instructions in it

## Setup

### GitHub account

[Sign up](https://github.com/join) for a GitHub account if you don't already have one.
Really, it's quite useful.

### Step 1 - Install dependencies

Follow each of the links to download and install.

- [git](https://git-scm.com/)
  - If you're on Windows or OS X and don't know what git is, [GitHub Desktop](https://desktop.github.com/) is probably easiest.
- [anaconda](https://www.continuum.io/downloads)

### Step 2 - Clone an LDSSA repo

In the future, you will clone other repositories so take note of these
steps, you will indeed use them again. If you don't already know where
you will want to clone the repo to on your machine, create a directory
in your user's home directory called "repos" and clone everything to
that.

#### Using GitHub Desktop

From the green "Clone or Download" button on the github.com repo page,
select "clone using github desktop" as shown below:

![clone](http://i.imgur.com/i8pZmhD.png)

#### From the command line

```
git clone git@github.com:LDSSA/setup.git
```
  
Take a note of the filepath on which you cloned the repo!

Note that if you choose this option, you will need to have your
[ssh keys set up](https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/).
  
### Step 3 - Start your environment

Open up anaconda and launch the jupyter notebook

![launch jupyter notebook](https://i.imgur.com/SFeVsT6.png)

### Step 4

#### Make sure that jupyter notebook is running

In the freshly opened notebook, navigate to the root of this repository and open and run
the `Verify great success.ipynb` notebook (you run cells by clicking on them and then pressing shift+enter).
If you get a couple of pretty graphs, you are all good to go!

### Final notes

#### Before the day

On the thursday before the academy, we will be asking you to clone another repository.
With the new repo, you will do everything the same as in step 4 but nagivate to a
different repository.

#### On git usage

- If you are trying to sync a notebook and you get a conflicts error,
  navigate to the directory and execute `git stash` before you sync again.
