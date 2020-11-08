# Linux command line 
### For unzip 
```
unzip -q filename.zip
```
### For zip file 
```
zip -r filename.zip filename
```
### For remove file 
```
rm -rf dirname
```
### For move file through ssh connection
```
scp /path/to/file username@IDaddress:/path/to/destination
```
### Script for settting font in vscode
```
#LINK FOR SEETING ZSH
https://viblo.asia/p/customize-terminal-mac-dinh-nham-chan-cua-ubuntu-vscode-rubymine-voi-zsh-XL6lAyo4lek
#Font for vscode
sudo apt install fonts-firacode
```
### Link for down gcc version
```
https://linuxconfig.org/how-to-switch-between-multiple-gcc-and-g-compiler-versions-on-ubuntu-20-04-lts-focal-fossa
```
### Screen command 
```
#for create a screen session
screen -S <sessionname>

#for show list of session 
screen -ls

#for resume your session
screen -r <session ID>

#for kill a session
screen -X -S [session # you want to kill] quit
# for exit scree
Crtl + A + D
```
### Check weblcam list
```
ls -ltrh /dev/video*
```
# Python
### Install requirement 
```
pip install -r requirements.txt
```
### jupyter on ssh
```
jupyter notebook --ip 192.168.1.232 --NotebookApp.token='' --NotebookApp.password=''
```
### conda command
```
#for remove a env
conda remove --name <envname> --all



