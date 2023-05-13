# Remove pre-installed
`sudo apt purge libreoffice-* hexchat celluloid redshift rhythmbox hypnotix timeshift warpinator transmission-* thunderbird sticky simple-scan pix rclone`

# Install essentials
`sudo apt install vim htop vlc bc module-assistant build-essential dkms`

# Lines to be add to ~/.bashrc
```
export PS1="\[\e]0;\u@\h: \w\a\]${debian_chroot:+($debian_chroot)}\[\033[01;32m\]\u@\h\[\033[00m\]:\[\033[01;34m\]\w\[\033[00m\]\n$ "
alias of="xdg-open $1"
alias nvrun="__NV_PRIME_RENDER_OFFLOAD=1 __GLX_VENDOR_LIBRARY_NAME=nvidia $1"
alias gb="git branch -vv"
```
