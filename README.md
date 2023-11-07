# Mathematica Installation on Jupyter
This document shows istallation steps for WolframEngine anf WolframScript for using Mathematica on Jupyter Notebook.

Install WolframEngine and WolframScript
========================
Download WolframEngine installer via [WolframEngine Download Page](https://www.wolfram.com/engine/) for your OS and get your WolframEngine ID license from the page. 
- For Linux
  ```Linux
  cd Downloads
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
