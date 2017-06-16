## Database Management with SQLite

SQLite is a lightweight Relational Database Management System - it stores data in a specified format and uses the SQL language to work with the data.
SQL style database management systems are a great way of storing data - particularly if your data is "big" because it will not be stored in RAM as you work with it.

We chose SQLite because it involves the least set up and assumes no knowledge of server management.

## Installation Guide

### For Windows Users

We will install SQLite so that it plays nicely within CygWin.
Its time to go back to the **setup-x86_64.exe** we told you not to delete. We will use it to install sqlite.
Proceed as follows:

* Click through the installation until you arrive at the page "Select packages."
* Type sqlite into the search function and wait for the results to be filtered.
* Click the '+' next to "Database" and then find the following lines:
    * libsqlite3_0
    * sqlite3
 and then click on the word 'Skip.' located next to each of these. 'Skip' should then be replaced with some numbers (the version which we will install)
* Click the '+' next to "Ruby" and then click on 'Skip' next to:
    * ruby-sqlite3
    * ruby-sqlite-doc
so that version numbers again appear.
* Now click on "Next" in the bottom right corner and continue accepting all options until the installation is complete.

**Note:** Clicking through all the pages before "Select Packages" will *not* install or modify anything you have done previously - so don't fret along the way.

### For Mac Users

Open up a terminal and enter the following (followed by hitting the return key)

    brew install sqlite3

### For Linux Users

SQLite should already be installed on your system.

## Verifying the Installation

To check, open a terminal and then type (followed by hitting the return key):

    sqlite3 --version

If it is installed, you should see something similar to the follwoing returned:

    3.15.2 2016-11-28 19:13:37

This is the version number that you have installed. Ensure that the version you have installed is `3.15.1` or higher.
