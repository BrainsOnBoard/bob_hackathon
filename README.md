# Brains on Board hackathon
Hello BoBers!

(**NOTE**: This repository is currently a work in progress while we finish up our hacking, so you won't be able to build the program for the hackathon yet. You should be able to install the dependencies though.)

This repository contains installation instructions for the various bits and pieces you'll need to install on your laptop if you'd like to use it for the hackathon (we can share machines, so not everyone needs to do this -- but the more the better!). It also contains git submodules for the various in-house programs we'll be using. The submodules are included for convenience so you don't have to download all the source code manually and to ensure you get the right versions.

So first things first...

## Installing git
If you haven't used git before, now is a good opportunity to learn :-).

If you're on Windows, you can download the git tools [here](https://gitforwindows.org). Linux users can install it from their package managers and Mac users can either get it [here](https://git-scm.com/download/mac) or (I guess) use Homebrew.

There are lots of good options for git GUI programs, but my personal fave is [Gitkraken](https://www.gitkraken.com) (it's free for academics).

## Cloning this repository and the submodules
If you're using a GUI, there should be a button labelled "clone" or something. To do it via the command line, run:
```
git clone https://github.com/BrainsOnBoard/bob_hackathon --recursive
```

The ``--recursive`` is needed so you get the submodules too, which otherwise won't be downloaded by default.

If you do find yourself without the submodules (i.e. the subfolders in the ``submodules`` directory are empty), you can download them by running:
```
git submodule update --init --recursive .
```

## Building the needed programs from source
If you followed the steps above you should have all the source code you need in the ``submodules`` directory, so you don't need to download these programs again.

Installation instructions for the various programs are available online:
* [Instructions for GeNN](https://github.com/genn-team/genn/blob/master/README.md)
* [Instructions for Spine Creator](https://spineml.github.io/spinecreator)

## Other dependencies
We will use a program called Gazebo for the robot simulation, which can be downloaded [here](http://gazebosim.org). If you're using Ubuntu you can install it with your package manager.

