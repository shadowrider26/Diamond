Diamond (DMD)

Instructions for compiling in Linux.

Update ubuntu
   
   sudo apt-get update

*install git to download the source code

    sudo apt-get install git

*install the other necessary components

    sudo apt-get install build-essential libboost1.55-all-dev libcurl4-openssl-dev libdb5.1-dev libdb5.1++-dev

*navigate to the home directory

    cd ~ *download the diamond source code

    git clone https://github.com/DMDcoin/Diamond.git

*navigate to the downloaded files

    cd ~ *navigate to the src file in the source code
    cd diamond/src

*create obj folder

    mkdir obj

*build diamondd !This will take a while!

    make -f makefile.unix USE_UPNP=-
