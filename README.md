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

> XX:XX:XX:XX:XX
> ZZ:ZZ:ZZ:ZZ:ZZ

### Usage
>chmod -x checkClients
>./checkClients safehosts.txt myemail@mydomain.com


