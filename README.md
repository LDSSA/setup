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
    - If you are on windows:
      - Make sure that there are no non-english characters in your username or on the path and that you have qt installed. [Here is a reference](https://github.com/ContinuumIO/anaconda-issues/issues/1270) on how to address these issues.

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

#### From the command line the easy way

```
git clone https://github.com/LDSSA/setup.git
```

#### From the command line the ssh way

Make sure that you have your [ssh keys set up](https://help.github.com/articles/connecting-to-github-with-ssh/).
Once they are you use *almost* the same clone command as above in 
"the easy way"

```
git clone git@github.com:LDSSA/setup.git
```
  
Take a note of the filepath on which you cloned the repo!

Note that if you choose this option, you will need to have your
[ssh keys set up](https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/).
  
### Step 3 - Start your environment

Open up anaconda and create a new python 3.5 environment with
1. Click on "environments"
1. Click on "Create"
1. Select 3.5 and give it a name "ldsa"
1. Click create

![Create a new environment](https://i.imgur.com/9YdLYTv.png | width=100)


**NOTE** that every time you start anaconda navigator, you will need to choose the ldsa environment! If you forget to do
this, you will be missing some key things!

### Step 4 - Install extra dependencies

Open a terminal with 

1. Click on Environments
1. Click on the green arrow next to the ldsa environment name
1. Click open terminal

![open terminal](https://i.imgur.com/R60Eavh.png | width=100)

Now copy-paste the following line into the terminal

```
conda config --add channels conda-forge
conda install Cython==0.28.2 jupyter==1.0.0 matplotlib==2.2.2 mlxtend==0.11.0 numpy==1.14.2 pandas==0.22.0 scikit-learn==0.19.1 seaborn==0.8.1
```

### Step 5 - Verify Success

Click on home and then run (install if needed) the jupyter notebook

![Launch the notebook](https://i.imgur.com/HSkFRpy.png | width=100)

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
