# Virtual Gens v0.1

Sega Gensis "Gens KMod" emulator running inside Unity in a virtual room.

This project is an attempt at implementing Sega's "SEGA Genesis Classics" VR room.

## Installation

1. Download the "VirtualGens" folder and copy it into a Unity project folder.
2. Import the prefab into the editor.
3. Build for Windows 32-bit; DLL was compiled in a 32-bit system. Mac and Linux are not supported.
4. Place a Sega Genesis ROM in the root folder where the application executable is. The ROM file should be named "rom.bin".

## Use

Run "VirtualGens.exe". The application will start in fullscreen and the Sega Genesis ROM will be executed immediately.

Controls:
* **Esc**: close the application.
* **Mouse**: look around.
* **W**: move forwards.
* **S**: move backwards.
* **A**: strafe left.
* **D**: strafe right.
* **Z: press A button on the controller.
* **X**: press B button on the controller.
* **C**: press C button on the controller.
* **B**: press X button on the controller.
* **N**: press Y button on the controller.
* **M**: press Z button on the controller.
* **V**: press Start button on the controller.

## Description

The Sega Gensis [Gens KMod](https://segaretro.org/Gens_KMod) source code was compiled as a 32-bit DLL with a new interface to allow communication with an application. The DLL code is run on a separate thread, and receives input from Unity. After each frame is rendered, the DLL sends it as an array to Unity to be drawn on a texture. Since audio is handeled directly by Gens, there is no 3D audio as of yet.

A virtual room was created with a TV where the execution of the emulator can be seen. The user can move and look around. The player carries a wireless Sega Genesis controller, animated when the user presses any button.

## Legal

I do not condone the use of ilegally obtained roms.

## Authors

* *Virtual Gens*: Federico Garcia
* *Gens KMod*: [Kaneda](https://segaretro.org/Gens_KMod)
* *Furbished Cabin asset*: [Johnny Kasapi] (https://assetstore.unity.com/packages/3d/environments/urban/furnished-cabin-71426)