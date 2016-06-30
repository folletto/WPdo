WPdo - Simple Make WordPress in Bash
====================================

**Simple command line tool to install WordPress TRUNK and patches from make.wordpress.com**  
<https://make.wordpress.org/>


WHAT IS WPDO
------------

Starting from scratch in contributing to Make WordPress is challenging, expecially for non-developers.
This tool, while still a command line tool, is meant to simplify how people can interact with the technical side of things, from setup to patches.


WHAT DOES IT DO
---------------

* Helps setting up a Mac OSX dev environment (sorry, just OSX for now, collaborations welcome)
* Helps updating a local WordPress TRUNK setup via SVN
* Helps applying and clearing patches easily


INSTALLATION
------------

1. Download `wpdo`
2. Install it in `bin` so it's globally available, or put it in the directory you're going to work
3. Make it executable
4. Run it from Terminal: `./wpdo`


USAGE
-----

* `wpdo start`  
  This command checks if everything is installed correctly and helps with setup.  
  Also installs WordPress TRUNK to _wordpress-trunk_ subdirectory.
* `wpdo patch [number]`  
  Just type the patch number or URL and it applies the patch to the WordPress in the current directory.
* `wpdo revert`  
  Restores the local WordPress folder you're in to its original state.
* `wpdo update`  
  Updates the local WordPress folder you're in to the latest revision.
* `wpdo kill`  
  Removes the WordPress sub-folder named _wordpress-trunk_.


CHANGELOG
---------

* **0.1** (26/06/2016)
  * First version.
  * Made at WordCamp Europe Contributors Day 2016


LICENSE
-------

  _Copyright (C) 2016, Davide Casali_  
  _Licensed under **GPLv3 License**_

> _I've got some gift for languages.  
  You follow your gift.  
  But Latin's not easy._  
  – Ursula K. Le Guin
