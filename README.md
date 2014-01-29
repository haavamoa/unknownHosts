unknownHosts
============

A Raspberry Pi project : emails you unknown hosts connected to your LAN.

The script uses a safehosts.txt file to read any already known hosts on the LAN, and does a crosscheck with nmap. If any unknown host pops up, it will contact you with the date and mac address of the host.
It also paces the unknown host in a .txt file called unknownhosts.txt.


#### safehosts.txt
The script reads each line in safehosts.txt, so the files structure naturally has to be like this:

> 62:L9:34:21:AB

> AB:21:34:L9:62

### Usage
>git clone https://github.com/haavamoa/unknownHosts.git

> cd checkClients

>chmod -x checkClients

>./checkClients safehosts.txt myemail@mydomain.com

or 

> ./checkClients safehosts.txt myemail@mydomain.com &

to run as a background process

### Requirements

* nmap

* mailutils

* mail

* smtp

* a safehosts.txt file with the mac addresses of the known hosts.

### Future plans

* A host will only be logged as unknown for 24 hours, after 24 hours and the host gets picked up it will send another email about its connection
