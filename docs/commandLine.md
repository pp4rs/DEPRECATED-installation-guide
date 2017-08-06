# Command Line Tools

A command-line interface or command language interpreter (CLI), also known as a terminal, is a means of interacting with a computer program where the user issues commands to the program in the form of successive lines of text (command lines).

Throughout the course we will emphasize use of the terminal and executing commands within it as our modus operandi.

## Windows Users

So that we can work as closely as possible to the Mac and Linux users we will install [Cygwin](https://www.cygwin.com/).
Download it [here](https://cygwin.com/install.html) and use the graphical installer. Accept all the default options.

* Verify your installation by opening Cygwin, when it opens you should see a black box with some text that looks like:
```bash
userName@computerName: ~$
```
i.e. for Lachlan he sees:
```bash
lachlan@lachlan-ThinkPad-T460s: ~$
```
We will explain what all this means in the first day or so of the course.

* We will uses Cygwin as our command line tool, and unlike other Windows shells such as PowerShell it uses Unix syntax.
        * Anywhere throughout the remainder of the installation guide where we suggest you to enter a command into a terminal, enter the text-based command into your Cygwin terminal, for example:

```bash
userName@computerName: ~$ whoami
```

* **Do not delete the setup-x86_64.exe file.** It needs to be kept so that we can add on some additional packages to use in the course.


## Mac Users

A command line interface comes already installed with OSX.

You will need to install some other software from the terminal thoughout the course, so it will be useful to install some additional "command line tools" now:

* First we want to install X-code command line tools. Open a terminal by using the `Cmd + T` shortcut and then copy and paste the following

```bash
xcode-select --install
```

* Second,  install Homebrew by opening a terminal and pasting the following command:

```bash
ruby -e “$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)”
```

* To verify that Homebrew installed correctly, enter the following into your terminal
```bash
brew doctor
```
And you should see the following output
```bash
Your system is ready to brew
```

## Linux Users

Nothing needs to be done.
