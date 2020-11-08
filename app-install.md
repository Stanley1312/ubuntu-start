# Install VS Code 
* First, update the packages index and install the dependencies by typing
```
$ sudo apt install software-properties-common apt-transport-https wget
```
* Next, import the Microsoft GPG key using the following wget 
```
$ wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -
```
And enable the Visual Studio Code repository by typing
```
$ sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"
```
* Once the apt repository is enabled , install the latest version of Visual Studio Code with
```
$ sudo apt update
$ sudo apt install code 
```
# REF 
[How to Install Visual Studio Code on Ubuntu 18.04](https://linuxize.com/post/how-to-install-visual-studio-code-on-ubuntu-18-04/)
