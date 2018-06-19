<<<<<<< HEAD
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
$ cd src/project/nemesis/18.x/etc/plugins # or to installation etc/ subdirectory
$ ./ConnectPlugins.sh all
$ ./ConnectPlugins.sh
``` 

## Dependencies
* qt5
* OpenGL
* libglewmx-dev
* libfreetype6-dev
=======
# NEMESIS - Molecular Modelling Environment
Nemesis is an advanced molecular structure builder. It is able to build a
molecule from predefined 3D fragments. Molecules can be visualized in
monoscopic and stereoscopic representations. The geometry of the built
molecule can be easily measured and manipulated.

## Documentation
The documentation is available [here](https://nemesis.ncbr.muni.cz).

## Building Package
The building and installation procedure can be found in the
[nemesis-build](https://github.com/kulhanek/nemesis-build) repository.
>>>>>>> 0f87275c365dc8eb7d0790295a9b9ca1dc22196b

