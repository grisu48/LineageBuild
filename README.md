# LineageBuild

My LineageOS build script. Usage:
    ./build DEVICE

I use it to build for hammerhead (Google Nexus 5)

## System requirements

This script is developed for Ubuntu 16.04 (and later). Older versions may work, but you may need to setup the toolchain manually.

See the LineageOS wiki for instructions (e.g. for the Nexus 5 device: https://wiki.lineageos.org/devices/hammerhead/build)

## Usage

* Dependencies install

First you need to setup the repository. Type the following to install them directly
    ./build --inst-dep
or the following to list the required dependencies.
    ./build --dependencies

* Repository initialisation

To setup the repository use the --init command
    ./build --init

To synchronize the repositories and build for hammerhead
    ./build hammerhead

You can replace hammerhead by your device.

The files are placed in the android/system/out/target/product/ subfolder

### In a nutshell

Dependencies install
    ./build --inst-dep
Initialize repository
    ./build --init
Build for hammerhead
    ./build hammerhead


