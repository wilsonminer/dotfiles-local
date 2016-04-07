my dotfiles
===================
I use a fork of Thoughtbot's [dotfiles](https://github.com/wilsonminer/dotfiles) as the
foundation of my personal configuration. These files are the `.local`
modifications that build on top of the foundation.

Requirements
------------

Install
-------

Install my fork of Thoughtbot's dotfiles:

    git clone git://github.com/wilsonminer/dotfiles.git ~/Code/dotfiles
    env RCRC=$HOME/Code/dotfiles/rcrc rcup

Then clone this repo:

    git clone git://github.com/wilsonminer/dotfiles-local.git ~/Code/dotfiles-local

And re-run rcup to link:

    rcup

This will create symlinks for config files in your home directory from
Thoughtbot's dotfiles and my local customizations.

You can safely run `rcup` multiple times to update:

    rcup

What's in it?
-------------

My custom additions to [thoughtbot's laptop setup script](https://github.com/thoughtbot/laptop)

* Generate SSH keys if they don't exist and prompt to add them to Github and Bitbucket
* Install basic software with Homebrew Cask
* Check out some git repositories to `~/Code`
* TODO: Personal gitconfig
* TODO: Install starred Atom packages

Credits
-------
Most of my configuration is small changes on top of thoughtbot's dotfiles.
They have a series of blog posts about dotfile configuration at their
[blog](http://robots.thoughtbot.com).

This software is free and distributable under the MIT license.
