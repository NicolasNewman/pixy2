Pixy2 README

This directory contains:

/releases - this directory contains binaries for various releases 

/scripts - this directory contains scripts for building pixy software modules.

/src/device - this directory contains code (firmware) that runs on the Pixy2 device.

/src/host - this directory contains code that runs on the host computer.
(Windows PC, Linux PC, Mac)

# Installation

```sh
// Install the repository to the directory of your desire
cd /directory/you/want/to/install/to
git clone https://github.com/NicolasNewman/pixy2.git

// Build the python bindings
cd pixy2/scripts
./build_python_demos.sh

// Run a test script to verify instilation
cd ../build/python_demos
python3 get_blocks_python_demo.py

// Make a syslink from the _pixy.so bindings to the python site-packages directory
ln -s _pixy.*.so /path/to/site-packages/_pixy.so
```

