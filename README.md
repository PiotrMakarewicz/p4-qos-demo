# p4-switch-ml-poc

## Environment setup

This guide assumes you are working on Windows 11.

Install VirtualBox 7.0 from this site: https://www.virtualbox.org/wiki/Downloads. Choose the full setup:

![obraz](https://github.com/PiotrMakarewicz/p4-switch-ml-poc/assets/54529536/3e106c2b-3896-4d41-ad07-c551a13ce891)

**(BEGIN UNNECESSARY PART?)**

(Not sure you actually need to install this.)
You will need to have python and pywin32 on your machine. If you are missing these dependencies, get Python 3.11 from Microsoft Store and then use pip to install pywin32.

```cmd
pip install pywin32
```
**(END UNNECESSARY PART?)**

Download a virtual machine image of Ubuntu with P4 and mininet from here: https://github.com/jafingerhut/p4-guide/blob/master/bin/README-install-troubleshooting.md. Choose 2023-Jun-01 version.

Import and run this virtual machine in Virtualbox. Log in as user `p4` with password `p4`.

To make life easier for yourself, install Mozilla Firefox and open this guide in virtual machine.

```bash
sudo apt-get update
sudo apt install firefox
```

From now on, you should be working from the inside of your virtual machine. Go to the home directory and download p4-switchML.

```bash
cd ~
git clone https://github.com/p4lang/p4app-switchML.git
```

