unknownHosts
============

A Raspberry Pi project : emails you unknown hosts connected to your LAN.

### Pre-requisits:

* nmap

* mailutils

* mail

* smtp

* a safehost.txt file with the mac addresses of the known hosts.

Example:

> 62:L9:34:21:AB

> AB:21:34:L9:62

### Usage
>git clone https://github.com/haavamoa/unknownHosts.git

> cd checkClients

>chmod -x checkClients

>./checkClients safehosts.txt myemail@mydomain.com


