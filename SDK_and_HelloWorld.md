# Guide for SDK Setup and Hello World program



## 1. SDK Setup:
### 1.1. RPi Documentation and Datasheets:
- Open the RP2040 documentation from this link: https://www.raspberrypi.com/products/rp2040/
https://www.raspberrypi.com/products/rp2040/specifications/
- Read all the given documentation such as Datasheets, specifications, SDK, examples, etc.
- Download all these PDFs for future reference.
<br>

![image](https://user-images.githubusercontent.com/52575718/194973666-19c1aa3e-2e7e-42f2-b355-569141604ef3.png)

<br>

### 1.2. Install Log:
- Set-up an ‘install log’ on Notes or Google Docs for your future reference, and for getting good grades :P

### 1.3. Getting started with PICO, SDK Download:
- Download the ‘Getting Started with PICO’ guide from here: https://datasheets.raspberrypi.com/pico/getting-started-with-pico.pdf
- We need to install the SDK using WSL on the Terminal on the Windows PC.
- Open Terminal, select Ubuntu in the drop down menu at the top of the screen.
- Open the PICO setup guide mentioned above and skip to Chapter 2 of the guide (Chapter 1 contains setup instructions for Raspberry Pi, which we don’t need in our case).
- Start by creating directories for all pico related stuff. Then, clone the git repositories for the example applications which are written using ‘pico-sdk’.
<br>

![image](https://user-images.githubusercontent.com/52575718/194973977-e8bcc9ff-6f2e-41be-912f-184a362ac1f0.png)

<br>

- Now, using the ‘apt’ command we need to install ‘CMake’ and the ‘ARM GNU Embedded Toolchain’ to build our applications in pico-examples.
- The ‘apt’ command will ignore the already present applications. 
- We are using Ubuntu, so we also need to install ‘ibstdc++-arm-none-eabi-newlib’ through the command line. 
<br>

![image](https://user-images.githubusercontent.com/52575718/194974060-9ee08925-4147-4c93-a5ff-72c2de68e5e5.png)

<br>

![image](https://user-images.githubusercontent.com/52575718/194974089-308554a0-5b19-4ef4-b97b-67fce5014414.png)

<br>

- Use the updating commands given in the documentation to update to the latest version of the SDK.
- Navigate to the pico-sdk folder before doing so. 
- Create a build directory in the already existing ‘pico-examples’ directory. 
- We have cloned the ‘pico-sdk’ and ‘pico-examples’ repos in the same directories side by side. We now need to set the PICO_SDK_PATH.
- We can do that using the command given in the documentation.
<br>

![image](https://user-images.githubusercontent.com/52575718/194974237-9bcc67e0-bc2d-4514-984f-6ba04a7723ac.png)

<br>

![image](https://user-images.githubusercontent.com/52575718/194974273-e428ab30-f602-4bd8-8516-674532f6ed88.png)

<br>

## Hello World Code Implementation:

- Navigate to the ‘hello_world’ directory in pico → pico-examples → build → hello_world → usb.
- Enter the ‘make -j4’ command. This command tells us how many cores are required to run a specific task. This step is optional and can be skipped.
<br>

![image](https://user-images.githubusercontent.com/52575718/194974441-3ec02845-b6ef-45d5-988c-5b074052c2e3.png)

<br>

![image](https://user-images.githubusercontent.com/52575718/194974477-25c417f9-1cff-49ef-bb04-46dc13a9d3b8.png)

<br>

- Now, hold down the ‘BOOT’ and ‘RST’ (Reset) pins on the RP2040 board. This will erase the pre-existing Micro-Python from our board. This is required to run our new code using RP2040. 
- Now, open the File Explorer. Access the WSL file system and find the UF2 binary which will be dragged and dropped into the RP2040, appearing as a USB mass storage after the rebooting process.
- This PC → Linux → Ubuntu → home → username.
- The RP2040 reboots itself and unmounts itself as a Mass Storage Device.
- Now the RP2040 starts running the flashed code.
- We cannot see the running code yet, for that we need to open an stdio interface. This is where PuTTY comes into picture.
- Open PuTTY, enter all the specifications of the board (as mentioned above in this documentation) and press the ‘Open’ button.
- You will see your code running in the PuTTY window. The text ‘Hello_World!’ will be displayed on your screen.
<br>

![image](https://user-images.githubusercontent.com/52575718/194974566-f56621a9-5260-4d20-b4e3-ab2ba769be43.png)

<br>

- Bravo! You have successfully completed one part of the lab. Now go have fun over the Fall Break :D



