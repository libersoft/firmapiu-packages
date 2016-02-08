## FirmaPiù Packages
This project keeps together all repositories needed to build firmapiu software suite. 
Every repo contains a branch named _master_ and one called _debian_ .

In the _master_ repo lives the source code, this is the place where the
developpement happens and where you can find the last developped code.
In the _debian_ branch  are stored the debian folder containing the
instructions to build the .deb package and the source code relative to the last
release.
The packages built should be compatible both with Debian and Ubuntu as well as
their\ derivates.

## How to build .deb package
In order to build the debian package you'll need:
* git
* debuild
    sudo apt-get install git debuild

1. git clone https://github.com/libersoft/firmapiu-packages.git
2. cd firmapiu-packages
3. git submodules init
4. git submodules update
5. cd <package folder>
6. debuild -uc -us 

Now you should have your .deb package located in the parent folder (..)
