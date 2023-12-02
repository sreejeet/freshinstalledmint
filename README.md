# FreshInstalledMint
### A few commands and notes for my fresh [Linux Mint](https://linuxmint.com/) installation.
### This should work fine with Ubuntu and Debian based LinuxMint.

# Remove pre-installed
```
sudo apt purge -y libreoffice-* hexchat hexchat-common celluloid redshift rhythmbox hypnotix timeshift warpinator transmission-* thunderbird sticky simple-scan pix
```

# Install essentials
```
sudo apt install -y vim htop vlc bc module-assistant build-essential dkms rclone libreoffice-calc libreoffice-writer
```

# Keyboard shortcuts
```
gsettings set org.cinnamon.desktop.keybindings.wm close "['<Alt>F4', '<Super>q']"
gsettings set org.cinnamon.desktop.keybindings.media-keys volume-up "['XF86AudioRaiseVolume', '<Alt>period']"
gsettings set org.cinnamon.desktop.keybindings.media-keys volume-down "['XF86AudioLowerVolume', '<Alt>comma']"
gsettings set org.cinnamon.desktop.keybindings.media-keys volume-mute "['XF86AudioMute', '<Alt>slash']"
gsettings set org.cinnamon.desktop.keybindings.media-keys terminal "['<Primary><Alt>t', '<Super>Return']"
```

# Lines to be add to ~/.bashrc
```
echo '
export PS1="\[\e]0;\u@\h: \w\a\]${debian_chroot:+($debian_chroot)}\[\033[01;32m\]\u@\h\[\033[00m\]:\[\033[01;34m\]\w\[\033[00m\]\n$ "
alias of="xdg-open $1"
alias nvrun="__NV_PRIME_RENDER_OFFLOAD=1 __GLX_VENDOR_LIBRARY_NAME=nvidia $1"
alias gb="git branch -vv"
' >> ~/.bashrc
```
