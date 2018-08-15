# Installing Anaconda Python

Anaconda is a pre-packaged Python distribution for scientific users.

Direct your browser to [Anaconda download page](https://www.continuum.io/downloads) and download the Python 3.6 Graphical Installer for your machine.
Follow the steps provided on the website. If you are on a windows machine, check the tips for a smoot install below.

During the installation you will be asked whether you want Anaconda Python to be added to your PATH. **Click yes!** Even if the installation window gives a warning about adding it to your PATH, please still check that box.

To verify that the correct version of Python has been installed and was made available in your PATH settings, close your terminal and open a **new** terminal interface and enter:

```bash
python --version
```
followed by hitting the `Return` key.

You should see the following information returned:

##   Windows users:

Notes on Anaconda installation:  

*   When asked if you want single or multiple user installation, choose single user  
*   Accept all defaults that are set in the installation window  
*   Check the box for adding Anaconda to your PATH  
*   In the last step, you are asked if you want Visual Studio. **Click yes!**  


```bash
Python 3.6.5 :: Anaconda, Inc.
```
##  Linux/Ubuntu users:
```bash
Python 3.6.2 :: Anaconda custom (64-bit)
```
##  Mac users:
you may get this:
```bash
Python 3.6.1 |  Anaconda 4.4.0 (x86_64)
```
or this:
```bash
Python 3.6.1 ::  Anaconda 4.4.0 (x86_64)
```

!!! tip "Python 2 vs Python 3"
    Python 2 and 3 are incompatible in syntax. If you had Python 2 previously installed on your machine, you have seen `Python 2.x.x` above, try typing

    ```python3 --version```

    instead. Now you should see a message like the one above and are good to go for the course.
