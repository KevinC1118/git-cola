# git-cola: The highly caffeinated git GUI

    git-cola is a powerful git GUI with a slick and intuitive user interface.

    Copyright (C) 2007, 2008, 2009, 2010, 2011, 2012, 2013
    David Aguilar and contributors

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 2 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.

## SCREENSHOTS

Screenshots are available on the
[git-cola screenshots page](http://git-cola.github.io/screenshots.html).

## DOWNLOAD

    apt-get install git-cola python-pyinotify

New releases are available on the
[git-cola download page](http://git-cola.github.io/downloads.html).

## FORK

    git clone git://github.com/git-cola/git-cola.git cola

[git-cola on github](https://github.com/git-cola/git-cola)

[git-cola google group](http://groups.google.com/group/git-cola/)


# NUTRITIONAL FACTS


## ACTIVE INGREDIENTS

* [git](http://git-scm.com/) 1.6.3 or newer

* [Python](http://python.org/) 2.5 through 2.7

* [PyQt4](http://www.riverbankcomputing.co.uk/software/pyqt/download) 4.4 or newer

## INOTIFY

[pyinotify](https://github.com/seb-m/pyinotify) 0.7.1 or newer
enables inotify support on Linux.

# BREWING INSTRUCTIONS

Normally you can just do "make install" to install *git-cola*
in your `$HOME` directory (`$HOME/bin`, `$HOME/share`, etc).
If you want to do a global install you can do

    make prefix=/usr install

You don't need to `make` to run it, though.
*git-cola* is designed to run directly out of its source tree.

    git clone git://github.com/git-cola/git-cola.git
    git-cola/bin/git-cola
    git-cola/bin/git-dag

## MAC OS X

Whether you install cola yourself with `make install` or
use the `git-cola.app` bundle, you will need to install
*Qt4* and *PyQt4*.

The easiest way to do this is to [install homebrew](http://mxcl.github.com/homebrew/)
and use it to install git-cola.

    brew install git-cola

Once brew has installed git-cola (and its dependencies) you either use
`git-cola.app`, run from source, or install from source via `make install`.
You can build `git-cola.app` by running `make git-cola.app`.

Installing these packages also gives you a PyQt development
environment which can be used for building your own applications
or hacking on cola itself.


## WINDOWS INSTALLATION

Download the latest stable Git, Python 2.x, and Py2x-PyQt4 installers

* [msysGit](http://msysgit.github.com/)

* [Python](http://python.org/download/)

* [PyQt](http://www.riverbankcomputing.co.uk/software/pyqt/download/)

* [git-cola Installer](https://github.com/git-cola/git-cola/downloads)

Once these are installed you can run *git-cola* from the Start menu or
by double-clicking on the `git-cola.pyw` script.

You can also use `python.exe` to invoke the `git-cola.pyw` script
directly from the command-line.

If you are developing *git-cola* on Windows you can run it from its
source tree by using `python.exe`.

    python.exe bin/git-cola

If you want to build the `git-cola Installer` yourself run the provided script

    win32/create-installer.sh

You have to make sure that the file

    /share/InnoSetup/ISCC.exe

exists. That is normally the case when you run the *msysGit bash* and
not the *Git for Windows bash* (look [here](http://msysgit.github.com/)
for the differences).
