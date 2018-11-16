# cisco-anyconnect-ubuntu
This is a short guide on using cisco anyconnect vpn on ubuntu. This is especially for NYU students who use a Ubuntu linux machine and want to use VPN outside campus, or connect to VPN at other NYU global site (NYU Shanghai VPN for example). This guide is tested on Ubuntu 18.04 LTS, but should also work on Ubuntu 16. 

## First Install necessary system packages, use sudo apt-get install to install the following packages.
- openconnect
- network-manager-openconnect
- network-manager-openconnect-gnome 

reference: https://gist.github.com/marshki/bd9aae8384f02aaca1eb5772d63969dc

## Then set up VPN for a particular global site. 

Now open Ubuntu network settings, click the + symbol on the VPN panel. You will see an option saying "Cisco Anyconnect Compatible VPN (openconnect)" (this option will not show up if you haven't installed the 3 packages mentioned above.)

Click on it, it will open a "Add VPN" window. Now in "Gateway", enter the correct NYU site gateway. For instance, enter "vpn.nyu.edu" if you are trying to connect to the VPN site in NYC. Here is a list of NYU site gateway names, the reference is actually for Mac, since NYU doesn't yet have good support page for Ubuntu. You can look at the official guide for MAC/Windows to get a basic idea. 
reference: https://nyu.service-now.com/servicelink/kb_search.do?id=KB0011175

After that you can give your vpn whatever name you want, and click "Add".

Now try to connect to this VPN, and enter your NYU netid and password (and also DUO authentication method, just look at the instructions on that new window.)
