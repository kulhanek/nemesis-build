# nemesis-build
Utilities for testing and building of the [NEMESIS - Molecular Modelling Environment](https://github.com/kulhanek/nemesis) package.

## Building and Installation

### Testing Mode
```bash
$ git clone --recursive https://github.com/kulhanek/nemesis-build.git
$ cd nemesis-build
$ ./build-utils/00.init-links.sh
$ ./01.pull-code.sh
$ ./04.build-inline.sh   # build the code inline in src/
```

### Production Build into the Infinity software repository
```bash
$ git clone --recursive https://github.com/kulhanek/nemesis-build.git
$ cd nemesis-build
$ ./build-utils/00.init-links.sh
$ ./01.pull-code.sh
$ ./10.build-final.sh
```

### Production Build into Custom Directory
```bash
$ git clone --recursive https://github.com/kulhanek/nemesis-build.git
$ cd nemesis-build
$ ./build-utils/00.init-links.sh
$ ./01.pull-code.sh
$ cmake -DCMAKE_INSTALL_PREFIX=/path/to/nemesis/installation/directory
$ make
$ make install
```

### Activation of Plugins
```bash
$ cd src/projects/nemesis/18.x/etc/plugins # or to installation etc/ subdirectory
$ ./ConnectPlugins.sh all
$ ./ConnectPlugins.sh
``` 

## Dependencies
* Ubuntu 18.04 LTS (Desktop)
```bash
$ sudo apt-get install git cmake g++ gfortran libfreetype6-dev libgl1-mesa-dev libglu1-mesa-dev libqt5opengl5-dev qtscript5-dev libqt5svg5-dev qtwebengine5-dev
```
