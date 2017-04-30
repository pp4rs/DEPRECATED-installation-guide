# Text Editors

A good text editor lies at the heart of any serious programmer's toolkit: It can do almost anything and makes you much more productive. The editors built into each program are generally are not an option (we will find certain cases where you may want to use them).

We recommend two editors:

* [Sublime Text](https://www.sublimetext.com)
* [Atom](https://atom.io/)

Please download an install (at least) one of these editors and stick with it for at least the duration of the course and assignment to get a feel for how they work.
There is a slight learning curve, but soon you will wonder why no-one forced you to do this before!

## Installing Sublime Text

Go to the [downloads page](https://www.sublimetext.com/3) and download the live installer for your operating system.

## Installing Atom

Go to the [downloads page](https://github.com/atom/atom/releases/tag/v1.9.9) and download the live installer for your operating system.

## Additional Package for Sublime Text

For those who want to use Sublime Text as their editor, you will need to add an additional package, "Package Control" to it so that we can customize it a little throughout the course. Proceed as follows:

Open the Sublime Text console via the using the ctrl+` shortcut or the View > Show Console menu.
Once open, paste the code below into the console (and press return):

        import urllib.request,os,hashlib; h = '2915d1851351e5ee549c20394736b442' + '8bc59f460fa1548d1514676163dafc88'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)

We will show you how to use Package Control during the course.
