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

## Dependencies
* qt5
* OpenGL
* libglewmx-dev
* libfreetype6-dev

