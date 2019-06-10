# Brains on Board hackathon
Hello BoBers!

This repository contains installation instructions for the various bits and pieces you'll need to install on your laptop if you'd like to use it for the hackathon (we can share machines, so not everyone needs to do this -- but the more the better!). It also contains git submodules for the various in-house programs we'll be using.

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
