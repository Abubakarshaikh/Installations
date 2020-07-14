# jupyter notebook download for ubuntu


### 1. In your browser, download the [Anaconda installer for Linux](https://www.anaconda.com/download/#linux)

### 2. Enter the following to install Anaconda for Python 3.7:
```
bash ~/Downloads/Anaconda3-2020.02-Linux-x86_64.sh
```

### 3. Scroll to the bottom of the license terms and enter “Yes” to agree.

### 4. The installer prompts you to click Enter to accept the default install location, CTRL-C to cancel the installation, or specify an alternate installation directory. If you accept the default install location, the installer displays “PREFIX=/home/<user>/anaconda<2 or 3>” and continues the installation. It may take a few minutes to complete.
> NOTE: We recommend you accept the default install location. Do not choose the path as /usr for the Anaconda/Miniconda installation.
  
### 5. The installer prompts “Do you wish the installer to initialize Anaconda3 by running conda init?” We recommend “yes”.

### 6. to launch jupyter notebook open Anaconda-navigator

### 7. To control whether or not each shell session has the base environment activated or not, run conda config --set auto_activate_base False or True. To run conda from anywhere without having the base environment activated by default, use conda config --set auto_activate_base False. This only works if you have run conda init first.
> NOTE: conda init is available in conda versions 4.6.12 and later.
