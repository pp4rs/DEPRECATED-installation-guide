# Web Scraping Using an Automated Browser

Sometimes when we scrape the web, we need to automate our computer to open a web browser to gather information from each page.
This is especially true when the site we want to scrape has content that is loaded dynamically with javascript.

We will install two packages to help us here:

1.  Chromedriver
2.  Phantomjs

Installing most of this stuff is operating system specific, hence so are the instructions below.

## Mac Users

Make sure your `homebrew` package is up-to-date. To do so, open a terminal and enter

```
brew update
```

### Chromedriver

*   Install via homebrew:
```
brew install chromedriver
```
*   Verify your install, by entering the following in your terminal. The expected output is `ChromeDriver 2.3X.X`
```
chromedriver --version
```

### Phantomjs

*   Install via homebrew:
```
brew install phantomjs
```
*   Verify your install, by entering the following in your terminal. The expected output is `2.1.1`
```
phantomjs --version
```

## Windows Users

### Chromedriver

*   Install Google Chrome from [here](https://www.google.com/chrome/browser/desktop/index.html)
*   Download the windows version of Chromedriver from [here](https://chromedriver.storage.googleapis.com/index.html?path=2.31/).
*   Extract the contents from the zip file, and place them in a new directory `C:\chromedriver`
*   Add the directory `C:\chromedriver` to your PATH.
*   If this went successfully, open a new Cygwin session, and enter `chromedriver --version`, you should get output that looks like `ChromeDriver 2.3X.XX`


### Phantomjs

*   Click [here](http://phantomjs.org/download.html) and go to the Windows download section. Download the zip file for version 2.1.1.
*   Right click on the downloaded phantomJs zip file to Extract All
*   Copy all the contents located in phantomjs-X.X.X-windows
*   Create a new directory `C:\PhantomJs\bin\phantomjs`
*   Paste the contents on the extracted phantomjs-X.X.X-windows directory here
*   Add the directory, `C:\PhantomJs\bin\phantomjs`, to your PATH like we have done before.
*   If this worked succesfully open a new Cygwin session, and enter `phantomjs --version` should return the version `2.1.1`


!!! tip "Hat-tip"
    We borrowed liberally from [Joe Coltantonio](https://www.joecolantonio.com/2014/10/14/how-to-install-phantomjs/) for instructions on installing Phantomjs.


## Linux Users

### Chromedriver

*   Open a terminal session
*   Install Google Chrome for Debian/Ubuntu by pasting the following and then pressing `Return`
```
sudo apt-get install libxss1 libappindicator1 libindicator7
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb

sudo dpkg -i google-chrome*.deb
sudo apt-get install -f
```
*   Install `xvfb` so chrom can run 'headless' by pasting the following and then pressing `Return`
```
sudo apt-get install xvfb
```
*   Install Chromedriver by pasting the following and then pressing `Return`:
```
sudo apt-get install unzip

wget -N http://chromedriver.storage.googleapis.com/2.31/chromedriver_linux64.zip
unzip chromedriver_linux64.zip
chmod +x chromedriver

sudo mv -f chromedriver /usr/local/share/chromedriver
sudo ln -s /usr/local/share/chromedriver /usr/local/bin/chromedriver
sudo ln -s /usr/local/share/chromedriver /usr/bin/chromedriver
```
*   Your install worked, you should get `ChromeDriver 2.31.488763` returned if the installation was successful
```
chromedriver --version
```

### Phantomjs

*   Open a terminal and paste the following:
```
sudo apt-get install build-essential chrpath libssl-dev libxft-dev \
libfreetype6-dev libfreetype6 libfontconfig1-dev libfontconfig1 -y
```
*   Download Phantomjs using your terminal:
```
sudo wget https://bitbucket.org/ariya/phantomjs/downloads/phantomjs-2.1.1-linux-x86_64.tar.bz2
```
*   Extract the archive:
```
sudo tar xvjf phantomjs-2.1.1-linux-x86_64.tar.bz2 -C /usr/local/share/
```
*   Create a symbolic link
```
sudo ln -s /usr/local/share/phantomjs-2.1.1-linux-x86_64/bin/phantomjs /usr/local/bin/
```
*   Verify the installation, and you should get `2.1.1` printed out
```
phantomjs --version
```

!!! tip "Hat-tip"
    We borrowed heavily from the guys and girls at Vultr to provide instructions for [Phantomjs](https://www.vultr.com/docs/how-to-install-phantomjs-on-ubuntu-16-04).
    We borrowed quite liberally from Christopher Su to for instructions on [installing Chrome and Chromedriver](https://christopher.su/2015/selenium-chromedriver-ubuntu/).
