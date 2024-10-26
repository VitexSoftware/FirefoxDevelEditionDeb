Firefox Developer Edition package for Debian / Ubuntu
=====================================================

![FirefoxDeveloperEdition](https://raw.githubusercontent.com/VitexSoftware/FirefoxDevelEditionDeb/master/mozicon300.png "DeveloperEdition logo")

A version of Firefox that's tailored for web developers.

Building package
----------------

```shell
    apt-get -y install devscripts dpkg-dev
    git clone https://github.com/VitexSoftware/FirefoxDevelEditionDeb.git
    debuild -i -us -uc -b
```


Installation
------------

Download from https://www.vitexsoftware.cz/pool/main/f/firefox-devedition/firefox-devedition_1.0.0_all.deb or Build package. Then install:

```shell
    gdebi firefox-devedition_1.0.0_all.deb
```


Or you can use repo:

```shell
sudo apt install lsb-release wget apt-transport-https bzip2
sudo wget -O /usr/share/keyrings/vitexsoftware.gpg https://repo.vitexsoftware.cz/keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/vitexsoftware.gpg]  https://repo.vitexsoftware.cz  $(lsb_release -sc) main" | sudo tee /etc/apt/sources.list.d/vitexsoftware.list
sudo apt update
sudo apt install firefox-devedition
```

Testing
-------

    vagrant up
    vagrant ssh
    sudo apt install xfce4
    startxfce4


![Vagrant Test](https://raw.githubusercontent.com/VitexSoftware/FirefoxDevelEditionDeb/master/vagrantubuntu.png "DeveloperEdition in Ubuntu")


See also: https://github.com/Vitexus/ThunderbirdDailyDeb https://github.com/Vitexus/FirefoxNightlyDeb
