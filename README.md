# Mathematica-Tutorial
This document shows istallation steps for WolframEngine anf WolframScript for using Mathematica on Jupyter Notebook.

Install WolframEngine and WolframScript
========================
Download WolframEngine installer via [WolframEngine Download Page](https://www.wolfram.com/engine/) for your OS and get your WolframEngine ID license from the page. 
- For Linux
  ```Linux
  cd Downloads
  sudo bash WolframEngine-installer.sh
  ```
  Download WolframScript installer via (WolframScript Download Page)[https://www.wolfram.com/wolframscript/] for your Linux version.
  ```Linux
  sudo dpkg -i WolframScript-installer.deb
  ```

  Activate WolframEngine ID.
  ```Linux
  wolframscript --activate
  ```
  If you have any questions, you can refer to the page below.
  
  [How do I set up the Wolfram Engine on Linux?](https://support.wolfram.com/46072)
  
  [Install WolframScript](https://reference.wolfram.com/language/workflow/InstallWolframScript.html)

- For MacOS

  After downloading the WolframEngine installer, click on the installer to begin the installation. Then, drag and drop to install WolframScript. Finally, activate the WolframEngine ID.
  ```Linux
  wolframscript --activate
  ```

Install Jupyter Notebook and Wolfram Langunge For Jupyter
========================
[WolframLanguageForJupyter](https://github.com/WolframResearch/WolframLanguageForJupyter)
