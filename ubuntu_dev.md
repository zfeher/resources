## Latest Chrome
- [install 1](http://askubuntu.com/questions/510056/how-to-install-google-chrome)
- [install 2](http://tecadmin.net/install-google-chrome-in-ubuntu/#)


## Unix
- [bash-guide](https://github.com/Idnan/bash-guide)
- [What are the shell's control and redirection operators?](http://unix.stackexchange.com/questions/159513/what-are-the-shells-control-and-redirection-operators)


## Check encoding for sed
- [sed-and-utf-8-encoding](https://stackoverflow.com/questions/27072558/sed-and-utf-8-encoding)
- `Bash printf à | wc -c` must say 2, not 1
- `Bash locale` should list "UTF-8" or "utf8" in the LC_CTYPE line


## Using sed with multiple files

```Bash
find app/scripts -type f -name "*.js" | xargs sed -b -i -- '/\/\* eslint max-len: \["error", 160\] \*\//d'
find app/scripts -type f -name "*.js" | xargs sed -b -i -- 's/, max-len: \["error", 160\]//g'
```

## Find files where first line includes pattern
```Bash
head -n1 -v app/scripts/components/base-input/basic/index.js | egrep -B1 "\/* eslint" | egrep "==>"
```

## Prepend header and append footer with sed

```Bash
find app/scripts/components/ -name "template.html" | xargs - L 1 sed -b -i -e $'1i<template>' -e $'$a</template>'
```

## Remove first and last line with sed

```Bash
find app/scripts/components/ -name "template.html" | xargs -p -L 1 sed -b -i '1d;$d'
```

[more info](https://unix.stackexchange.com/questions/209068/how-do-i-delete-the-first-n-lines-and-last-line-of-a-file-using-shell-commands)

## Find directories recursively

```Bash
find /path/ -type d -print
```

## Find files which contains text

```Bash
egrep --include=\*.js --exclude=\*.spec.js -Rnwl './app/scripts/components' -e '@vue/component'
```

## xargs multiple commands / input arg usage
```
# -I can give a name to input arg to be used in commands
cat foo.txt | xargs -I % sh -c 'echo %; mkdir %' 
```

## Run script in the current shell
```Bash
. ./somescript.sh
```


## Git
```Bash
sudo add-apt-repository ppa:git-core/ppa
sudo apt-get update
sudo apt-get install git
```
- [Bash completion](https://github.com/petervanderdoes/git-flow-completion/wiki/Install-Bash-git-completion)


## Git Flow
- [Using git-flow to automate your git branching workflow](http://jeffkreeftmeijer.com/2010/why-arent-you-using-git-flow/)
- [Bash ZSH completion AVH edition](https://github.com/petervanderdoes/git-flow-completion)
- [Install AVH edition](https://github.com/petervanderdoes/gitflow-avh)
- [Install AVH edition](https://github.com/petervanderdoes/gitflow-avh)
- [Bash, ZSH completion](https://github.com/bobthecow/git-flow-completion)
- [Install](https://github.com/nvie/gitflow/wiki/Installation)
- [Git Flow](https://github.com/nvie/gitflow)


## Python 2.7
```Bash
# refreshing the repositories
sudo apt update
# its wise to keep the system up to date!
# you can skip the following line if you not
# want to update all your software
sudo apt upgrade
# installing python 2.7 and pip for it
sudo apt install python2.7 python-pip
# installing python-pip for 3.6
sudo apt install python3-pip
```
**NOTE: Do not try to remove python 3.6 as it will screw up your system**
```Bash
# for python 2.7
pip2 install <package>

# for python 3.6
pip install <package>
```

### Resources
- [Correct way to install python 2.7 on Ubuntu 17.10?](https://askubuntu.com/questions/981118/correct-way-to-install-python-2-7-on-ubuntu-17-10)
- [How to Install Python 2.7.14 on Ubuntu & LinuxMint](https://tecadmin.net/install-python-2-7-on-ubuntu-and-linuxmint/)

## Diff and merge tools

### [DiffMerge](https://sourcegear.com/diffmerge)

### [KDiff3](http://kdiff3.sourceforge.net)
- [install 1](https://www.howtoinstall.co/en/ubuntu/xenial/kdiff3)
- [install 2](http://opensourceforgeeks.blogspot.hu/2014/07/how-to-install-kdiff3-on-ubuntu.html)
- [install 3](http://uniqueminds.co/2013/08/14/how-to-install-kdiff3-on-ubuntu.html)


## Node JS + NPM
- [install 1](https://github.com/nodesource/distributions)
- [install 2](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-16-04)


## [NVM](https://github.com/creationix/nvm) - Node Version Manager


## [n](https://github.com/tj/n) - node version manager

```Bash
cd somewhere
git clone https://github.com/tj/n.git
cd n
PREFIX=$HOME make install  # will install to $home/bin/n
```

Add the following to the end of $HOME/.bashrc
```Bash
export N_PREFIX="$HOME"  # node versions will be installed under $HOME/n/versions
```

note: something happens with npm when switching between versions eg if you installed the latest npm in 6.x then switch to 7.x and back the version of npm will be reset to 3.x

npm fix if needed (won't fix the problem above)
```Bash
$ curl -0 -L https://npmjs.org/install.sh | sudo sh
```

## Pomodoro
- [PomoDone](https://pomodoneapp.com/)
- [Pomodoro Indicator](https://github.com/atareao/pomodoro-indicator)
- [Tomighty](https://launchpad.net/~pwr22/+archive/ubuntu/tomighty)
- [Tomate](https://github.com/eliostvs/tomate-gtk)
- Pomodoro Chrome/Opera extensions ?


## OpenConnect
```Bash
sudo apt-get install network-manager-openconnect-gnome # will be visible in GUI as well
sudo openconnect vpn.acme.com
```

- [install 1](http://askubuntu.com/questions/154699/how-do-i-install-the-cisco-anyconnect-vpn-client)
- [install 2](https://support.onevpn.com/knowledgebase/linux-ubuntu-anyconnect/)
- [install 3](https://technicalsanctuary.wordpress.com/2016/05/28/installing-cisco-anyconnect-vpn-on-ubuntu-16-04/)
- [install 4](http://ubuntuhandbook.org/index.php/2014/11/connect-cisco-anyconnect-vpn-ubuntu/)
- [install 5](http://askubuntu.com/questions/627638/cisco-anyconnect-compatible-vpn-openconnect-in-ubuntu-15-04)


## VirtualBox
- [How to install open-vm-tools-desktop On Ubuntu 16.04 Lts? ](https://www.devmanuals.net/install/ubuntu/ubuntu-16-04-LTS-Xenial-Xerus/how-to-install-open-vm-tools-desktop.html)
- [How to Access Folders on Your Host Machine from an Ubuntu Virtual Machine in VirtualBox](http://www.howtogeek.com/187703/how-to-access-folders-on-your-host-machine-from-an-ubuntu-virtual-machine-in-virtualbox/)
- [Resizing Virtual drive](http://askubuntu.com/questions/101715/resizing-virtual-drive/558215#558215)
- [IE virtual machines](https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/)
