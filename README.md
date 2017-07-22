# IMPORTANT

Once you have completed the setup, mark yourself as such on [this spreadsheet](https://docs.google.com/spreadsheets/d/1SYn38h_DNzdyrZsDH4y50U32eDMdoi00cNDdn2MHAsE/edit?usp=sharing)

# How to use this repo

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
- [docker](https://docs.docker.com/engine/installation/)
  - [OSX](https://store.docker.com/editions/community/docker-ce-desktop-mac)
  - [Windows](https://store.docker.com/editions/community/docker-ce-desktop-windows)
  - [Browse here](https://www.docker.com/community-edition#/download) if you use another platform


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

#### Make sure that docker is running!

Before you start your environment, you must make sure that docker
is running. Otherwise when you try to run it, you will get an error
that say something about not being able to find the docker daemon.

#### Navigate on the command line to the root of the repo

##### Command line on windows

If you installed GitHub Desktop, it comes with a program called "git bash" that
you should be able to find in your applications. Any time you must do something
on your command line, it's recommended to use this.

#### Navigate to the repo on the command line

Assuming you've cloned the repo into your repos on OS X or linux, the command would look something like

- `cd ~/repos/data-science-101`

#### Start the docker image and jupyter notebook

  - `bash run-jupyter-notebook.sh`
  
Note that the first time you run this, it will take a LONG time because it has to download
basically an entire operating system.
  
### Step 4

#### Make sure that jupyter notebook is running

Open [http://localhost:8888](http://localhost:8888) in your browser and you should see
an `examples` directory. Navigate into it and run the example notebook
to make sure that you don't get any errors.

### Final notes

- You don't need to have docker running all the time. Feel free to shut it down
  when you aren't using your notebooks.
- If you have troubles or errors with running your notebook, check the
  terminal where you started it from to see if there are any hints.
- If something doesn't work, always remember to give it the ol'
  turn it off and turn it on trick.

