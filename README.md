## IMPORTANT

Once you have completed the setup, mark yourself as such on [this spreadsheet](https://docs.google.com/spreadsheets/d/1SYn38h_DNzdyrZsDH4y50U32eDMdoi00cNDdn2MHAsE/edit?usp=sharing)

If you know what you're doing in terms of python, there's a requirements.txt that you can
use as you would like. If that's the case the only thing you really need to do is make sure
you can run the example notebook in this repo and you are good.

## How to use this repo

This repository is the one that you will use to make sure you can execute
all of the critical tasks required to make the most of your learning
experience. In particular, after following this readme, you should:

1. Have a GitHub acount
1. Be able to clone a git repository
1. Be able to start a jupyter notebook
1. Run code within a jupyter notebook to (among other things) render some plots.

## Prerequisites

Please note that these are conservative estimates. If you
are not 100% on than any of these, you should still be okay.

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
- [anaconda](https://www.continuum.io/downloads#windows)


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
  
### Step 3 - Start your environment

Open up anaconda and launch the jupyter notebook

![launch jupyter notebook](https://i.imgur.com/SFeVsT6.png)

#### Navigate to the repo on the command line

Assuming you've cloned the repo into your `repos` directory the command would look something like

### Step 4

#### Make sure that jupyter notebook is running

In the freshly opened notebook, navigate to the root of this repository and open and run
the notebook. If you get a couple of pretty graphs, you
are all good to go!

### Final notes

#### Before the day

On the thursday before the academy, we will be asking you to clone another repository.
With the new repo, you will do everything the same as in step 4 but nagivate to a
different repository.

#### On git usage

- If you are trying to sync a notebook and you get a conflicts error,
  navigate to the directory and execute `git stash` before you sync again.
