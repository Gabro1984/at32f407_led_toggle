# Simple LEDs blinking
======================================

The project forked from original"led_toggle" example from  Arterytek  Firmware Library <br />
[Download Arterytek at32f407 Firmware Library](https://github.com/ArteryTek/AT32F403A_407_Firmware_Library.git) <br />
but based on open source solutions to build and debug application. <br />
You can use this project as a template to create more complex applications for Arterytek MCUs. <br />

To build project cmake with a GNU toolchain are used.  <br />
[Download GNU toolchain](https://developer.arm.com/downloads/-/gnu-rm) <br />

To debug Arterytek openocd is used.  <br />
[Download Arterytek openocd](https://github.com/ArteryTek/openocd.git) <br />

To debug using VS Code editor openocd configuration is attached at .vscode folder.  <br />

## Preparing

   1. Install cmake. <br />
   2. Download an arm-none-eabi toolchain and add path to toolchain to the PATH enviroment variable. <br />
   3. Download Arterytek openocd and build it by following instructions from README file. <br />

## Building
   1. Create and go to build directory  <br />
      `mkdir build && cd build`  <br />
   2. Run cmake  <br />
      `cmake ..`  <br />
   3. Build  <br />
      `make -j8`  <br />

## Debugging  <br />
   Just run VS code and start debug.  <br />

   Note: if path to openocd configs was changed during openocd installation  <br />
   you need to edit ".vscode/launch.json".  <br />