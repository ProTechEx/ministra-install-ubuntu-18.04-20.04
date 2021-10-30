# ministra-install-ubuntu-20.04
Ministra Portal auto install script

[![Donate](https://img.shields.io/badge/Donate-PayPal-blue.svg)](https://www.paypal.com/donate?hosted_button_id=4H8VAGMLW5RMA) - You can make one-time donations via PayPal.

##### Runs on
[![Ubuntu](https://user-images.githubusercontent.com/12951085/139525842-ce8999f2-bae2-4306-94a8-fac83aba7e41.png)](https://www.ubuntu.com)

This script work only on Clean Ubuntu 20.04

Ministra auto install script
  * Version of Ministra 5.6.5

## Installation
```bash
apt-get install git
git clone https://github.com/madzharov/ministra-install-ubuntu-20.04.git
cd ministra-install-ubuntu-20.04/
```

Open minister_install_ubuntu.20.04.sh with your favorite text editor and change on line 17
```bash
mysql_root_pass="test123456"
```
- This is the root password for MySQL that will be set during the installation, you can change it with yours if you wish.


And on line 14 change
```bash
TIME_ZONE="Europe/Sofia"
```
- This is the time zone that will be set during the installation, you can change it with yours if you wish

The installation itself is as follows:
```bash
chmod +x ministra_install_ubuntu.20.04.sh
./ministra_install_ubuntu.20.04.sh
```

- Accordingly, during the installation, when executing the last command, phing will ask you for the root password for MySQL, enter the password you set on line 17



You can access your stalker portal at: http://ipadres/stalker_portal The username and password to login to the portal are your default
```
Login: admin
pass: 1
```

Remove all channels from the database through the terminal
```bash
mysql -u root -p stalker_db
truncate ch_links;
truncate itv;
```

## Video

[![Click to Watch](https://img.youtube.com/vi/6b2vlc-jPPQ/hq720.jpg)](https://www.youtube.com/watch?v=6b2vlc-jPPQ "Click to Watch")


[![Donate](https://img.shields.io/badge/Donate-PayPal-blue.svg)](https://www.paypal.com/donate?hosted_button_id=4H8VAGMLW5RMA) - You can make one-time donations via PayPal.
