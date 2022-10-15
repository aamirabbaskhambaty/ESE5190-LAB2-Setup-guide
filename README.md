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
<img src="" width="700" height="700">
