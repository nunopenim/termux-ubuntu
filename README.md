# termux-ubuntu

Set of scripts to install Ubuntu variants chroot images in Termux.

## Preparation

You need to install wget and proot in Termux before using this script.

```
pkg install wget proot
```

The script will make its files in the current directory. So if you want your Ubuntu-filesystem at a particular location switch to that folder first and then call the script with it's relative path.

## Instalation

These will install it in a folder named "ubuntu" in your home directory

For the current LTS version:

```
mkdir -p ~/ubuntu
cd ~/ubuntu
wget https://raw.githubusercontent.com/nunopenim/termux-ubuntu/master/lts_release.sh
mv lts_release.sh ubuntu.sh
bash ubuntu.sh
```

For the latest release:

```
mkdir -p ~/ubuntu
cd ~/ubuntu
wget https://raw.githubusercontent.com/nunopenim/termux-ubuntu/master/latest_release.sh
mv latest_release.sh ubuntu.sh
bash ubuntu.sh
```

For any version available:

```
mkdir -p ~/ubuntu
cd ~/ubuntu
wget https://raw.githubusercontent.com/nunopenim/termux-ubuntu/master/distros/<distro_name>.sh
mv <distro_name>.sh ubuntu.sh
bash ubuntu.sh
```

After installation, you can run "start-ubuntu.sh" (./start-ubuntu.sh) to switch into your ubuntu installation.

## Special thanks

These scripts are adaptations of [Neo-Oli's](https://github.com/Neo-Oli) termux-ubuntu script.
