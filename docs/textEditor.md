# Text Editors

A good text editor lies at the heart of any serious programmer's toolkit: It can do almost anything and makes you much more productive. The editors built into each program are generally are not an option (we will find certain cases where you may want to use them).

This year we are encouraging all participants to use the text editor [Atom](https://atom.io/).

Please download, install it alng with the necessary packages and stick with it for at least the duration of the course and assignment to get a feel for how it works.
There is a slight learning curve, but soon you hopefully be wondering why no-one forced you to do this before!
We should get you past the steepest part of the learning curve during the course itself, so we don't anticipate you struggling on your own.

*Note:* None of the skills we learn in the course are tied to Atom, so if you do decide to move away to another editor, nothing will be lost.

<!-- ## Installing Sublime Text

Go to the [downloads page](https://www.sublimetext.com/3) and download the live installer for your operating system. -->

## Installing Atom

Go to the [downloads page](https://github.com/atom/atom/releases/tag/v1.9.9) and download the live installer for your operating system.

## Additional Packages for Atom

One of the advantages of atom is that there are many *packages* that make your life easier, ranging from simple syntax highlighting to environments that can mimic a complete graphical user interface.

For this course, we will install the minimum number of packages necessary to make your coding life easier.

## Installing Additional Packages for Atom

Atom's package manager is built in to the program itself and is relatively esay to interact with.
To access Atom's settings press `Ctrl + ,` on your keyboard then click on the `Install +` tab which is visible on the left hand side.

On the Installation page there is a prompt where you can type in a package name and then press `Enter/Return` and Atom will search for that package for you and return results with similar names. When you find the package that you need, you click the blue Install button and the package will be installed.

For this course, please install the following packages (not a complete list yet):

* autocomplete-r
* autocomplete-python
* autoflow
* hydrogen (?)
* language-r
* linter
* tablr

If you decide to stick with Atom after this course, you may find the following packages useful in your day to day work:

* language-latex
* language-markdown
* language-make
* language-sql
* markdown-writer
* markdown-preview-plus
* whitepace

<!-- ## Additional Package for Sublime Text

For those who want to use Sublime Text as their editor, you will need to add an additional package, "Package Control" to it so that we can customize it a little throughout the course. Proceed as follows:

Open the Sublime Text console via the using the ctrl+` shortcut or the View > Show Console menu.
Once open, paste the code below into the console (and press return):

        import urllib.request,os,hashlib; h = '2915d1851351e5ee549c20394736b442' + '8bc59f460fa1548d1514676163dafc88'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)

We will show you how to use Package Control during the course. -->
