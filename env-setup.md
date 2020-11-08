# Install Conda virtualenv 
## 1. In your browser, download [the Anaconda installer for Linux.](https://www.anaconda.com/products/individual#linux)
## 2. CHECK IT on linux terminal
```
sha256sum /path/filename
```
## 3. Enter the following to install Anaconda for Python 3.7
```
bash ~/Downloads/Anaconda3-2020.02-Linux-x86_64.sh
```
### NOTE: Include the bash command regardless of whether or not you are using Bash shel
## 4. The installer prompts you to click Enter to accept the default install location, CTRL-C to cancel the installation, 
or specify an alternate installation directory. If you accept the default install location, the installer displays “PREFIX=/home/<user>/anaconda<2 or 3>” 
and continues the installation. It may take a few minutes to complete.
## 5. To control whether or not each shell session has the base environment activated or not, run conda config --set auto_activate_base False or True. To run conda from anywhere without having the base environment activated by default, use conda config --set auto_activate_base False. 
This only works if you have run conda init first.
