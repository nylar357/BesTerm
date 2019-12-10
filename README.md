# BesTerm
Productive, Great Looking, Terminal configuration.  Made of multiple tools, and here you'll get a short description of the tools needed.  How to install them and pics of the final product.


A complete guide to setup a reliable, good looking, and highly productive terminal environment.

Tools: (basic installation unless otherwise stated apt,pacman,xbpc,ect.)

Zsh
Oh-My-Zsh
Terminal Multiplexor (Tmux)
Customized Tmux Configuration
PowerLevel9k - Highly Specialized Zsh Prompt

Prerequisites:
*curl or wget
*git

# a basic apt installation
sudo apt-get install git & apt-get install (your choice of wget or curl)

*powerline fonts (https://github.com/powerline/fonts)

# clone
git clone https://github.com/powerline/fonts.git --depth=1
# install
cd fonts
./install.sh
# clean-up a bit
cd ..
rm -rf fonts

*Oh-My-Zsh (https://github.com/nylar357/oh-my-zsh)

via curl
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
via wget
sh -c "$(wget -O- https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

*Customized Tmux Configuation (https://github.com/nylar357/mytmux)

git clone https://github.com/samoshkin/tmux-config.git
sudo bash ./tmux-config/install.sh

install.sh script does following:

copies files to ~/.tmux directory
symlink tmux config file at ~/.tmux.conf, existing ~/.tmux.conf will be backed up
Tmux Plugin Manager will be installed at default location ~/.tmux/plugins/tpm, unless already presemt
required tmux plugins will be installed
Finally, you can jump into a new tmux session:

tmux new

Finally You should end up with something along there lines.


