# dotfiles

I use [thoughtbot/dotfiles](https://github.com/thoughtbot/dotfiles) and manage it with [rcm](https://github.com/thoughtbot/rcm).

These are my  `.local` files that add to the base config.

## Set up a new machine

First, run Thoughtbot's [laptop setup script](https://github.com/thoughtbot/laptop) to set up a new machine with some basic development defaults.

Get Thoughtbot's dotfiles:

    git clone git://github.com/wilsonminer/dotfiles.git ~/Code/dotfiles

Then clone this repo:

    git clone git://github.com/wilsonminer/dotfiles-local.git ~/Code/dotfiles-local

And rcup to link:

    env RCRC=$HOME/Code/dotfiles-local/rcrc rcup

This will create symlinks for config files in your home directory from Thoughtbot's dotfiles with these local customizations.

After the initial setup, you can safely run `rcup` multiple times to update, without setting the environment variables:

    rcup

Next, run the [laptop setup script](https://github.com/thoughtbot/laptop) again, which will now include the extra scripts from this config.

## TODO

* Set OS X defaults
* iTerm colors
* VIM plugins and colors
* Install fonts
