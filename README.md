# ESE5190-LAB2-Setup-guide

### **System Specifications**
1. OS: Windows 11
2. CPU: Intel Core i7 10th Gen
3. Ram: 16GB
4. SSD: 256GB
5. LOG software used: Notepad
6. Code Editor : VS Code

### **Relavant Softwares Used**
The following tools need to be installed in order to run and compile the Pico C SDK:
1. [Arm GNU Toolchain](https://developer.arm.com/downloads/-/arm-gnu-toolchain-downloads)
2. [CMake](https://cmake.org/download/)
3. [Build Tools for Visual Studio 2022](https://visualstudio.microsoft.com/downloads/#build-tools-for-visual-studio-2022)
4. [PuTTy Serial Terminal](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)
5. [C/C++ MinGW Compiler](https://www.mingw-w64.org/downloads/)
6. [Pico SDK](https://github.com/raspberrypi/pico-sdk)
7.[Pico examples](https://github.com/raspberrypi/pico-examples)
### **Installation Guide**
1. First step is to install gitbash using the link mentioned above
2. Once installed refer to the [Raspberry Pi Pico Getting Started Guide](https://datasheets.raspberrypi.com/pico/getting-started-with-pico.pdf)to clone the Pico SDK and Pico Examples preferbaly into the same directory.
3. Download and install  GCC/G++ compiler
4. Downlaod an install CMake
5. Download and install the Arm GNU toolchain
6. You will now have to add the PICO_SDK_PATH to the environment variables. i was unable to do it through command line and therefore suggest go to the set environment variables in the start menu. The address of the PICO_SDK_PATH will be the directory where you have cloned the SDK and Examples.  

![image](https://user-images.githubusercontent.com/114267693/195966007-12b0df62-cd46-4a89-a7cb-17c5f0ac86fe.png)
7. In your pico examples folder, create a folder called "build"

Open a terminal inside build

Generate a cmake build system using the cmake command. Remember that CMAKE must be installed and make sure that it is added to the environment variables. In the terminal, type the following:  .
```
cmake .. -G "MinGW Makefiles"
```
8. After this if you check many folders will be uilt inside your build folder.
9. Now in the terminal change the directory to hello_world/usb directory:
```
cd hello_world/usb 
```
Now enter the following in the terminal to build the code:
```
mingw32-make -j6
```
10. once the build has been successfully completed you will find a .UF2 File in your build folder for Hello World.
11. Mount your RP2040. Make sure you press and hold the BOOTSEL button while mounting the usb and then release the button.
12. Once Done a RP1-RP2 folder shall open up.
13. Copy your .UF2 File into the folder, if succesfully done it will vanish.
14. Now open up 
