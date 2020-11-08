# Install Blue UI and Custom Terminal

## Install zsh
* Install zsh
```
sudo apt-get install zsh
```
* Set zsh become default shell
```
chsh -s $(which zsh)
```
### NOTE: You should log out after above step
## Install Oh-my-zsh
* Install oh-my-zsh!
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```
### NOTE: After install zsh-shell you should transfer paths from bashrc to zshrc by delete:
```
export PATH=$HOME/bin:/usr/local/bin:$PATH in  ~./zshrc 
```
