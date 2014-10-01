doc-scripts
===========

Setup, Installation and Initialization scripts


# VM Setup

```bash
sudo apt-get update && sudo apt-get install build-essential linux-headers-$(uname -r)
sudo ln -s /usr/src/linux-headers-$(uname -r)/include/generated/uapi/linux/version.h /usr/src/linux-headers-$(uname -r)/include/linux/version.h
sudo ./vmware-install.pl

mkdir -p .ssh
cd ~/.ssh

ssh-keygen -t rsa -C "john.fragkoulis@gmail.com"
ssh-add id_rsa

cat id_rsa.pub

cd ..

sudo apt-get install git

git config --global user.email "john.fragkoulis@gmail.com"
git config --global user.name "John Fragkoulis"
git config --global push.default simple

sudo add-apt-repository ppa:webupd8team/sublime-text-2
sudo add-apt-repository ppa:webupd8team/sublime-text-3
sudo apt-get update

sudo apt-get install sublime-text
# sudo apt-get install sublime-text-installer
```
