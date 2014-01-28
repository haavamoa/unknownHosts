unknownHosts
============

A Raspberry Pi project : emails you unknown hosts connected to your LAN.
The script uses a safehosts.txt file to read any already known hosts on the LAN, and does a crosscheck with nmap. If any unknown host pops up, it will contact you with the date and mac address of the host.
It also paces the unknown host in a .txt file called unknownhosts.txt.

### Pre-requisits:

* nmap

* mailutils

* mail

* smtp

* a safehosts.txt file with the mac addresses of the known hosts.

Example:

> 62:L9:34:21:AB

> AB:21:34:L9:62

### Usage
>git clone https://github.com/haavamoa/unknownHosts.git

> cd checkClients

>chmod -x checkClients

>./checkClients safehosts.txt myemail@mydomain.com


