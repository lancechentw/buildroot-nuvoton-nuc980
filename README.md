The Buildroot external tree for Nuvoton NUC980 boards
=====================================================

This repo is originated from https://github.com/OpenNuvoton/NUC970_Buildroot. The specific configurations for Nuvoton NUC980 boards are extracted from the Buildroot tree to make it easier to work with latest Buildroot version.

Get started
-----------

```sh
# Clone this repo
git clone https://github.com/lancechentw/buildroot-nuvoton-nuc980

# Clone the Buildroot repo
git clone https://github.com/buildroot/buildroot

# We will be building inside the buildroot directory
cd buildroot

# Load the config for Nuvoton NUC980 IIoT board
make BR2_EXTERNAL=../buildroot-nuvoton-nuc980 nuvoton_nuc980_iot_defconfig

# Modify the configuration if needed
make menuconfig

# Start building
make

# Checkout the built artifacts
ls output/
```
