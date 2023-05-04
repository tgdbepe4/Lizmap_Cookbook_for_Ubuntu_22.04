# Lizmap_Cookbook_for_Ubuntu_22.04

This documentation has the aim to enable Lizmap installers to get a properly running Lizmap installation which easy can extend and re configured. And this as simple as possible.

**The only constraint is the willing to use Ubuntu 22.04 LTS as OS.**

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
Must accept to use ONLY Ubuntu 22.04 LTS server with it. 
- Running an initial installation of Ubuntu 22.04 LTS server.
- Understanding basic Linux command line usage.

## Performing_
- Copy and paste the full or part by part of the script into a terminal window and run it as root.
- Answer potentially occurring pop up questions with yes. Use the TAB key in this case to select or confirm.

## At the end you will have:
- A full updated Ubuntu 22.04 LTS
- The ubuntu-gnome-desktop GUI
- A running remote desktop server, RDP.
- Apache 2 running with all for qgis-server and lizmap necessary additions.
- The last QGIS and QGIS server versions are installed. At the moment version 3.30.
- A running Lizmap installation with the demo projects as well.

## The 000-default.conf apache2 configuration file
Consist of all necessary parameters to properly run qgis-server on apache2

## Install_QGIS-Server_3_28_Lizmap_3_6_3_auf_Ubuntu_22_04_V1.txt
Installation script to run an installation with QGIS und QGIS-Server 3.28

## Install_QGIS-Server_3_30_Lizmap_3_6_3_auf_Ubuntu_22_04_V1.txt
Installation script to run an installation with QGIS und QGIS-Server 3.30

## Adaption
Enhanced linux users should be able to adapt the script for any other Ubuntu oder Debian version. Important is the OS is fresh and native which mean that python3 or php an so is not already installed.


