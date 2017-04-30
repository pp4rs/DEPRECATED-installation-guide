# Command Line Tools

A command-line interface or command language interpreter (CLI), also known as command-line user interface, is a means of interacting with a computer program where the user issues commands to the program in the form of successive lines of text (command lines).

Throughout the course we will emphasize use of the terminal and executing commands within it as our modus operandi.

## Installation Guide

### Windows Users

So that we can work as closely as possible to the Mac and Linux users we will install [Cygwin](https://www.cygwin.com/).
Download it [here](https://cygwin.com/install.html) and use the graphical installer. Accept all the default options.

**Do not delete the setup-x86_64.exe file.** It needs to be kept so that we can add on some additional packages throughout the course.


### Mac Users

A command line interface comes already installed on Mac OSX.

But you will need to install some other software from the terminal thoughout the course, so it will be useful to install some additional "command line tools" now:

First we want to install X-code command line tools. Open a terminal and then copy and paste the following

    xcode-select --install

Second,  install Homebrew by opening a terminal and pasting the following command:

    ruby -e “$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)”

To verify that Homebrew installed correctly, enter the following into your terminal

    brew doctor

And you should see the following output

    Your system is ready to brew

### Linux Users

Nothing needs to be done.
