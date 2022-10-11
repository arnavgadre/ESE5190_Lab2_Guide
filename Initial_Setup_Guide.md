# Guide to Setup your Environment


## 1. Installing Windows Subsystem for Linux (WSL) - Ubuntu:
- WSL can be downloaded from the documentation offered by Microsoft, which is available online: https://learn.microsoft.com/en-us/windows/wsl/install
- My system already had WSL installed. I downloaded Ubuntu from the Microsoft store (this can also be done through Powershell).
- My Ubuntu was not running because I was missing the updated version of the WSL2 Kernel Package.
- Install that package from the link given here: [WSL2 Linux kernel update package for x64 machines](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi). 
- Follow the Microsoft documentation for setting up and running Ubuntu on your PC. 


## 2. Installing Terminal on the Laptop:
- I have used the pre-existing ‘Terminal’ program present on Windows. You can download any terminal application available as open source.
- Create a text file. You will navigate to this file using the Terminal program.
- Navigate to your folder using the ‘cd’ function. The folder where you have stored your text file.
- Print the contents of the directory using the ‘dir’ command, as shown below.
- Print contents of the word file file using the ‘cat’ command, as shown below.
<br>

![image](https://user-images.githubusercontent.com/52575718/194972032-9432a405-866f-46bd-8159-3e1ff7c2e827.png)

<br>

## 3. Installing and Running Vim and NeoVim:
- Download and install the latest version of NeoVim (stable release) from here: https://neovim.io/
- Add it as an Environment variable to open it using Terminal (Go to the ‘Edit the SYstem Environment Variables’ tab → Environment Variables → Click on PATH → Click on ‘New’ → Paste the Path of the NeoVim application on your machine → Press ‘Okay’ to save and exit).
- Open Neovim from the terminal using the ‘nvim’ command.
<br> 

![image](https://user-images.githubusercontent.com/52575718/194972300-736ce09c-28d9-40d3-9020-edb8e79451b1.png)

<br>

- The ‘VimTutor’ is not available on NeoVim. So I downloaded the Vim release.
- Downloaded the 64-bit release of Vim (gvim) from here: https://github.com/vim/vim-win32-installer/releases
- Download the most suitable version for your machine specs. (64-bit in my case).
- Open Vim using the terminal (‘vim’ command). Open VimTutor using the terminal itself (‘vimtutor’ command)
- Follow the steps given in the VimTutor and incorporate them on NeoVim, because it is an advanced version of Vim, and much better to use overall. This will get you well acquainted with using NeoVim.
<br>

![image](https://user-images.githubusercontent.com/52575718/194972567-b40bbcbf-a561-4678-8c7a-a883dfc7eaef.png)

<br>

## 4. Installing and Running PuTTy:
- Download and installed PuTTy from the given online resources: https://learn.adafruit.com/welcome-to-circuitpython/advanced-serial-console-on-windows
- Run the exe file. 
- In our case the details to be entered are as follows: Connection Type --> Serial | Speed --> 115200 | Serial Line --> COM7 (Check your COM port using Device Manager).
- Enter and save the required specs in a file (Embedded_1 in my case) to load it anytime in the future.
- Click ‘Open’ to open the PuTTy program terminal.
- You are all set to use PuTTy.
<br>

![image](https://user-images.githubusercontent.com/52575718/194973133-d6f26507-dd4f-4540-bf5b-1575a4eaa2c5.png)

<br>

![image](https://user-images.githubusercontent.com/52575718/194973157-10f55196-bb66-4b09-8936-f810f4d60c0f.png)








