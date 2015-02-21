Diamond (DMD)
===

Fork Information
===

This branch is an unofficial offshoot that allows building for armv7l
architecture CPUs. It was made for the convenience of people that either 
use an ARM desktop or run an ARM server and who want to keep their 
wallet open to mint coins via POS or want to run an energy-efficient 
node for solo mining.

This fork really only adds a few lines of changes to the Makefile and 
Qt's version of a makefile. It might even be a drop-in solution for the 
future, if neither have significant changes made to them. (Either that
or the Diamond team will merge it.)

Information for building is located in:
[doc/build-unix-arm.txt](doc/build-unix-arm.txt) for headless and
[doc/readme-qt-arm.rst](doc/readme-qt-arm.rst) for the Qt GUI.


Instructions for compiling in Linux for armv7l.
---

Update ubuntu
```   
sudo apt-get update
```
*install git to download the source code
```
sudo apt-get install git
```
*install the other necessary components
```
sudo apt-get install build-essential libboost1.55-all-dev libcurl4-openssl-dev libdb5.1-dev libdb5.1++-dev
```
*navigate to the home directory
```
cd ~ *download the diamond source code
git clone https://github.com/DMDcoin/Diamond.git
```
*navigate to the downloaded files
```
cd ~ *navigate to the src file in the source code
cd diamond/src
```
*create obj folder
```
mkdir obj
```
*build diamondd !This will take a while!
```
make -f makefile.unix xCPUARCH=armv7l
```