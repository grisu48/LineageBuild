# LineageBuild

My LineageOS build script. Usage:

    ## First setup the repository
    # ./build --inst-dep            # Install dependencies (Ubuntu 18.04)
    # ./build --init
    
    ## Trigger build
    $ ./build DEVICE

I used it to build for hammerhead (Google Nexus 5)

## System requirements

This script is developed for Ubuntu 18.04. It worked well on Ubuntu 16.04, older version may need to setup the toolchain manually.

See the LineageOS wiki for instructions (e.g. for the [Samsung Galaxy S7](https://wiki.lineageos.org/devices/herolte/build) or the [Nexus 5](https://wiki.lineageos.org/devices/hammerhead/build))

The build script is hardcoded to only work for 14.1. You can try other versions by changing the FLAVOUR variable in the script.

## Usage / Build recipe

**Dependencies install**

First you need to setup the repository. Type the following to install them directly

    ./build --inst-dep

or the following to list the required dependencies.

    ./build --dependencies

**Repository initialisation**

To initialize the repository use the --init command.

    ./build --init

This step should only be done once and the script warns you if you are trying to initialize it again.

**Build for a device (e.g. hammerhead)**

To synchronize the repositories and build for hammerhead

    ./build hammerhead

You can replace hammerhead by your device.

The files are placed in the android/system/out/target/product/ subfolder

### In a nutshell

    ./build --inst-dep			# Dependency install (Once)
    ./build --init			# Initialize repository (Once)
    ./build hammerhead			# Build for hammerhead

# Disclaimer

You are free to use, share, modify or even print this script without any restrictions but keep in mind that it comes with ABSOLUTELY NO WARRANTY. Use at own risk. Have fun.

If you find it useful, please share!


