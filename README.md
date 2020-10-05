# termux-ubuntu

A script to install Ubuntu chroot in Termux

It dose'nt work because that currupted link is https://partner-images.canonical.com/core/disco/current/ubuntu-disco-core-cloudimg-${archurl}-root.tar.gz

this is the new link 
https://partner-images.canonical.com/core/bionic/current/ubuntu-disco-core-cloudimg-${archurl}-root.tar.gz

You need to install wget and proot in Termux before using this script.

```
pkg install wget proot
```

The script will make its files in the current directory. So if you want your Ubuntu-filesystem at a particular location switch to that folder first and then call the script with it's relative path. Example:
```
mkdir -p ~/jails/ubuntu
cd ~/jails/ubuntu
wget https://raw.githubusercontent.com/asecginli/termux-ubuntu/main/ubuntu.sh
bash ubuntu.sh
```

After running it you can run "start-ubuntu.sh" to switch into your ubuntu

