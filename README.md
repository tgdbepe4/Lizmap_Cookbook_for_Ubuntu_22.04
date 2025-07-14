# Lizmap_Cookbook_for_Ubuntu

This documentation has the aim to enable Lizmap installers to get a properly running Lizmap installation which easy can extend and re configured. And this as simple as possible.

These scripts are foreseen for Ubuntu 22.04 and 24.04
- Using differnet versions of Ubuntu require different ways to bing it alive. The main difference is that the qgis-plugins cannot installed with the normal python pip installer and instead pipx has to be used.
- Lizmap is now on version 3.9. This require by default using the py-qgisserver. The script here are still based on Apache and a single qgis-server. If you install you have to made a post installation configuration:
- Eigentlich wird der py-qgis-server erst ab version 3.9.0 “default” - du kannst aber in der lizmap/var/config/localconfig.ini.php
Den Block aktiv schalten, und ändern zu:
[qgisWrapper]
; If off, FCGI is not allowed, only Py-QGIS-Server or QJazz
; Py-QGIS-Server
; Welcome to py-qgis-server’s documentation! — py-qgis-server 1.8 documentation
; GitHub - 3liz/qjazz: A suite of QGIS based services
allowFcgi=on
Dann kannst du die 3.9.X version auch ohne py-qgis-server nutzen.

Lizmap installation is always tricky and a lot of people have much problems. Often so much that they giving up.

Reasons for this are that so many differnet instances must interwork. 
- apache2 with all the necessary addons and configurations
- the missing installation libapache2-mod-fcgid module
- the Fcgid* parameters in the apache config file
- php version and the apache integration
- the apache and the php modules
- python version python3 in our case
- the desired qgis and qgis-server version
- the lizmap version and the installing

## Pre requites and limitations:
- The installer has to use ONLY Ubuntu 22.04 LTS server with it. 
- Running an initial installation of Ubuntu 22.04 LTS server.
- Understanding basic Linux command line usage.

## Performing the script commands
- Copy and paste the full or part by part of the script into a terminal window and run it as root user.
- Answer potentially occurring pop up questions with yes. Use the TAB key in this case to select or confirm.

## At the end you will have:
- A full updated Ubuntu 22.04 LTS
- The ubuntu-gnome-desktop GUI
- A running remote desktop server, RDP.
- Apache 2 running with all for qgis-server and lizmap necessary additions.
- **The last QGIS and QGIS server versions are installed. At the moment version 3.34**
- **A running Lizmap installation with the demo projects as well.**

## The 000-default.conf apache2 configuration file for Ubuntu 22.04.
Consist of all necessary parameters to properly run qgis-server on apache2.

## Install_QGIS-Server_3.34_Lizmap_3.8.1_Ubuntu_22_04_V1.txt
Installation script to run an installation with QGIS und QGIS-Server 3.34

## Install_QGIS-Server_3.34_Lizmap_3.8.1_Ubuntu_22_04_V1.txt
Installation script to run an installation with QGIS und QGIS-Server 3.34


## Adaption
Enhanced linux users should be able to adapt the script for any other Ubuntu oder Debian version. Important is the OS is fresh and native which mean that python3 or php an so is not already installed.


