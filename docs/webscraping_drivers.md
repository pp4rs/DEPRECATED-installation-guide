# Web Scraping inside a Browser

Sometimes when we scrape the web, we need to automate our computer to open a web browser to gather information from each page.
This is especially true when the site we want to scrape has content that is loaded dynamically with javascript.

We will install two packages to help us here:

1.  Chromedriver
2.  Phantomjs

Installing most of this stuff is operating system specific.

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
