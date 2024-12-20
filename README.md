# Mathematica Installation on Jupyter
This document shows istallation steps for WolframEngine anf WolframScript for using Mathematica on Jupyter Notebook.

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

Visual Studio Code (Optional)
========================
To launch Jupyter Notebook, you can use its built-in GUI; however, this can be inconvenient when frequently switching between the notebook and the terminal. I recommend using Visual Studio Code (VS Code) for primary editing and code execution. This code editor is lightweight, high-performance, supports numerous extensions, and is free to use.

Click on this link and follow the installation instructions specific to your machine's operating system.\
[Visual Studio Code](https://code.visualstudio.com/) 
<p align="center">  
<img src="https://github.com/user-attachments/assets/786e642f-bbb6-4f22-900a-f2e96e0804ee" width="760px" height="400px"  align="center" >
</p>
For Windows, you can download from Microsoft Store.
<p align="center">  
<img src="https://github.com/user-attachments/assets/40b9b9ec-d236-46a3-8e72-85cd59c02fc5" width="600px" height="460px"  align="center" >
</p>

For all OS, you need to set up for connecting VS Code with WSL.\
[Developing in WSL](https://code.visualstudio.com/docs/remote/wsl)


