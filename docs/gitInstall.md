# Installing Git and Setting Up Accounts

Git is a Version Control System (VCS) that has gained a lot of traction among the programming community.
We will want to use version control to keep track of the files we write, and the changes we make to them.

## Account Creation

During the course we will show you how to use [GitHub](https://www.github.com) to host some of your work and do code related project management. You will need to set up an account:

<!-- During the course we will show you how to host some of your work on GitHub and the Economics Department's internal GitLab server.
You will need to setup accounts for each of these: -->

*   Please [register](https://github.com/join) for a [GitHub](https://github.com/) account
<!-- *   Sign into the [Economics Department's GitLab server](https://econgit.uzh.ch/). Use your UZH shortname and your web-access password (same as for OLAT). You will need to access "Econ Git" while on-site at UZH or whilst using a UZH VPN if you are off-site. -->

<!-- !!! danger "Non-UZH Economics Students"
    The UZH Department of Economics has a internal Git server that may be hard for you to access.
    It looks and behaves almost identically to [GitLab](https://about.gitlab.com/).
    We recommend that you register for an account here, so you can follow along in class. -->

## Mac Users

On MacOS, download and install Git from [here](http://git-scm.com/download/mac).
Also install the command-line auto-completion script, as described [here](https://git-scm.com/book/en/v1/Git-Basics-Tips-and-Tricks#Auto-Completion).


## Linux Users

Follow the steps documented [here](https://git-scm.com/download/linux) to install on Linux from the terminal.

## Windows Users

Download and install the latest versions of:

*   [msysgit](http://msysgit.github.io), and
*   [TortoiseGit](http://code.google.com/p/tortoisegit/wiki/Download)

After installing these programs use Windows Explorer to go to a folder that contains some documents (any folder) and right click on it.
You should see some additional items - "GitBash" and "TortoiseGit" appear in the context menu upon right-clicking.


!!! danger "Windows PATH Setting Redux"
    We also want Git from the command line, so we again need to update our PATH settings.

    Right-click on Computer. Then go to "Properties" and select the tab "Advanced System settings". Choose "Environment Variables" and select `Path` from the list of system variables.

    Choose `Edit`.

    **On Windows 7 or 8 machines:**
    If you accepted all defaults during your installation, and didn't have any other non-default setting prior to starting this guide, modifying the following string, copy and paste the following string without spaces at the start or end:

           ;C:\Program Files\Git\bin

    **On Windows 10 machines:**
    Click `New` and paste the following string:

            C:\Program Files\Git\bin

    Click on `OK` as often as needed.


## Verifying your install

<!-- We will need to make Git accessible from the command line. Windows and Mac users will need to follow the steps on the page "Modifying Path Settings." Linux users will already have git accessible from the command line. -->

To verify your installation, type the following command in a terminal and press the return key:

       git --version

You should get an output that looks like:

        git version 2.7.4

Ensure that you have a version greater than `2.7.1` installed.
