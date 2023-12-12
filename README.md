# Mathematica Installation on Jupyter
This document shows istallation steps for WolframEngine anf WolframScript for using Mathematica on Jupyter Notebook.

Install Ubuntu on Windows
========================
First, dowload `Windows Subsystem for Linux` from Microsoft Store.

<p align="center">  
<img src="https://github.com/CraverBoyyy/Mathematica-Installation/assets/109847168/561f59c4-e73b-40a1-ae29-6fde23ffa87a" width="700px" height="450px"  align="center" >
</p>

Turn on the windows feature of `Windows Subsystem for Linux`. Search `Turn Windows features on or off` and tick on `Windows Subsystem for Linux` to allow the permission. 

<p align="center">  
<img src="https://github.com/CraverBoyyy/Mathematica-Installation/assets/109847168/c8d18143-35b0-4778-8f4e-0d277852f8e4" width="300px" height="300px"  align="center" >
</p>

You need to download the `Windows Terminal` software from Microsoft Store. After installing windows terminal, script the following commands on `Command Prompt`.
```Linux
wsl --set-default-version 1
wsl --install Ubuntu
```
The Ubuntu terminal have been displayed and you need to set username and password for Ubuntu account. And then script the following commands for fisrt setting on Ubuntu.
  ```Linux
  sudo apt update && sudo apt upgrade
  sudo apt-get install libegl1
  sudo apt-get install libasound2
  ```
For more infomation: [https://ubuntu.com/tutorials/install-ubuntu-on-wsl2-on-windows-10#1-overview](https://ubuntu.com/tutorials/install-ubuntu-on-wsl2-on-windows-10#1-overview)

  Install Python Languge and Jupyter.
  ========================
  - For Linux Ubuntu
  ```Linux
  sudo apt install python3
  sudo apt install python3-pip
  pip3 install numpy
  pip3 install scipy
  pip3 install matplotlib
  pip3 install getdist
  pip3 install jupyter
  ```
 - For MacOS
   - Install HomeBrew
```Linux
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
  ```Linux
brew install python3
python3 -m pip install --upgrade pip
pip3 install numpy
pip3 install scipy
pip3 install matplotlib
pip3 install getdist
pip3 install jupyter
  ```
 
Install WolframEngine and WolframScript
========================
Download WolframEngine installer via [WolframEngine Download Page](https://www.wolfram.com/engine/) for your OS and get your WolframEngine ID license from the page. 
- For Linux Ubuntu
  ```Linux
  sudo bash WolframEngine-installer.sh
  ```
  Activate WolframEngine ID.
  ```Linux
  wolframscript --activate
  ```
  If you have any questions, you can refer to the page below.
  
  [How do I set up the Wolfram Engine on Linux?](https://support.wolfram.com/46072)
  
  [Install WolframScript](https://reference.wolfram.com/language/workflow/InstallWolframScript.html)

  [WolframScript Download Page](https://www.wolfram.com/wolframscript/) 

- For MacOS

  After downloading the WolframEngine installer, click on the installer to begin the installation. Then, drag and drop to install WolframScript. Finally, activate the WolframEngine ID.
  ```Linux
  wolframscript --activate
  ```

Install Wolfram Langunge For Jupyter
========================
Clone the WolframLanguageForJupyter repository
```Linux
git clone https://github.com/WolframResearch/WolframLanguageForJupyter.git
cd WolframLanguageForJupyter
```
Run the following command in your shell to make the Wolfram Language engine available to Jupyter:
```Linux
./configure-jupyter.wls add
```
Check Wolfram Languge kernel on Jupyter
```Linux
jupyter kernelspec list
```
The out put should include `wolframlanguage13    ..\jupyter\kernels\wolframlanguage13`.

Run Jupyter Notebook and select Wolfram Language from the drop down menu to start Wolfram kernel on your notebok.
```Linux
jupyter notebook
```

<p align="center">  
<img src="https://github.com/CraverBoyyy/CosmoMC-Installation/assets/109847168/11febab3-4bac-4791-ba63-f1e5701f0d01" width="600px" height="300px"  align="center" >
</p>

For more information: [WolframLanguageForJupyter](https://github.com/WolframResearch/WolframLanguageForJupyter)
