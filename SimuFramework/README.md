# Computer Animation 2022 - Exercise

## Overview

Code framework for course exercise.

## Installation

Install **Git** and build system **Cmake**. For windows user, MSVC need to be installed.

### Note for linux users

Many linux distributions do not include `gcc` and the basic development tools in their default installation. On Ubuntu, you need to install the following packages:

```
sudo apt-get install build-essential libx11-dev mesa-common-dev libgl1-mesa-dev libglu1-mesa-dev libxrandr-dev libxi-dev libxmu-dev libblas-dev libxinerama-dev libxcursor-dev
```

### Build

Clone this repo (together with the submodule `libigl`):
```
git clone --recursive http://dalab.se.sjtu.edu.cn/gitlab/courses/ca-framework-2022.git
# if you forget clone submodule at first place
git submodule update --init --recursive
``` 

Run the following commands inside the relevant subfolder to setup the build folder:
```
mkdir build
cd build
cmake ..
```

Compile and run the executable, e.g. Ubuntu:
```
make && ./0_dummy/0_dummy
```

### For Windows

Cmake will generate Microsft visual studio project. Click the `*.sln` file to open the project and build.
