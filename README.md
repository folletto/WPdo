WPdo - Simple Make WordPress in Bash
====================================

**Simple command line tool to install WordPress TRUNK and patches from make.wordpress.org**  
<https://make.wordpress.org/>


WHAT IS WPDO
------------

Starting from scratch in contributing to Make WordPress is challenging, expecially for non-developers.
This tool, while still a command line tool, is meant to simplify how people can interact with the technical side of things, from setup to patches.

If you just need support for patches and you're comfortable with Grunt, you might want to check [grunt-patch-wordpress](https://www.npmjs.com/package/grunt-patch-wordpress).

WHAT DOES IT DO
---------------

* Helps setting up a Mac OSX dev environment (sorry, just OSX for now, collaborations welcome)
* Helps updating a local WordPress TRUNK setup via SVN
* Helps applying and clearing patches easily


INSTALLATION
------------

Fast:

1. Open Terminal
2. Run `curl -s https://raw.githubusercontent.com/folletto/WPdo/master/wpdo -o wpdo.php && php wpdo.php install`
3. Done! Now you can use `wpdo` from Terminal.

Manual:

1. Download `wpdo`: https://raw.githubusercontent.com/folletto/WPdo/master/wpdo
2. Copy it in `/usr/local/bin` so it's globally available.
3. Make it executable: `chmod +x /usr/local/bin/wpdo`.
4. Done! Now you can use `wpdo` from Terminal.

Public WPdo website [here](https://folletto.github.io/WPdo/).

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

UPDATE
------

To update uninstall with `wpdo uninstall` then run the installation again.


CHANGELOG
---------

* **0.2.1** (2017-05-12)
  * Better URL detection for patches.
  * Detection of `src/` path to switch from `patch -p0` to `patch -p1`
  * Display of changed files after successful patch.
* **0.2** (2016-07-22)
  * Added install/uninstall commands.
  * Now remote installation with `curl` works.
* **0.1** (2016-06-26)
  * First version.
  * Made at WordCamp Europe Contributors Day 2016


LICENSE
-------

  _Copyright (C) 2016-2017, Davide Casali_  
  _Licensed under **GPLv3 License**_

> _I've got some gift for languages.  
  You follow your gift.  
  But Latin's not easy._  
  – Ursula K. Le Guin
