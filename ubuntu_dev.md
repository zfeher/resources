## Latest Chrome
- [install 1](http://askubuntu.com/questions/510056/how-to-install-google-chrome)
- [install 2](http://tecadmin.net/install-google-chrome-in-ubuntu/#)


## Latest Git
```Bash
sudo add-apt-repository ppa:git-core/ppa
sudo apt-get update
sudo apt-get install git
```

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
