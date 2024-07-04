# to Install chsh
yum install util-linux-user

# To make zsh default shell
chsh -s /bin/zsh root

# To pull OH MY Zsh!
wget https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh -O - | zsh

# T0 copy the frame work
cp ~/.oh-my-zsh/templates/zshrc.zsh-template ~/.zshrc

# TO Refresh shell
source ~/.zshrc


# Install brew
sudo passwd ec2-user
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"


# To remove password for installing 
sudo visudo

Add ec2-user ALL=(ALL) NOPASSWD: ALL 

* Press Ctrl+X to exit the editor.
* Press Y to confirm that you want to save the changes.
* Press Enter to confirm the file name to write to (which should be the default sudoers file).


brew install starship
# ~/.bashrc

eval "$(starship init bash)"


# Fzf
