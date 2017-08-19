# Pandoc

Pandoc is an extremely useful 'swiss army knife' for converting between different types of markup languages from the command line.
For example, it readily builds PDFs with latex, and markdown - both of which are heavily used in academic research.

We do not actively teach how to use Pandoc in the course - but we will utilize it in some lessons where we produce PDF, Word or HTML output from plain text files.

## Installation

*   Go to the [Pandoc Homepage](https://pandoc.org/) and follow the installation instructions for your operating system.

## Verify Your Install

Verify your install by typing the following into a command line:
```bash
pandoc --version
```
The expected output starts with the following information:
```bash
pandoc 1.17.2
```
Ensure you have at least version 1.15.1 installed.

!!! danger " Windows PATH Setting redux"
    If you want R available from the command line (it is by default for Mac and Linux), we again need to update our PATH settings.

    Right-click on Computer. Then go to "Properties" and select the tab "Advanced System Settings". Choose "Environment Variables" and select "Path" from the list of system variables.

    If you accepted all defaults during your installation, and didn't have any other non-default setting prior to starting this guide, copy and paste the following string without spaces at the start or end:

            ;C:\Program Files (x86)\Pandoc\

    After you have done this, open a **new** terminal and try and verify your install.
