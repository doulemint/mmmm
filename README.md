# SSSSSSSSSSS
-rw-r----- 1 root adm 13207068947 Jun  9 13:19 /var/log/cups/error_log
root@stone-W65KJ1-KK1:~# logrotate -vf /etc/logrotate.d/admin
reading config file /etc/logrotate.d/admin

Handling 1 logs

rotating pattern: /var/log/admin.log  forced from command line (5 rotations)
empty log files are rotated, old logs are removed
switching euid to 0 and egid to 38
considering log /var/log/admin.log
  log needs rotating
rotating log /var/log/admin.log, log->rotateCount is 5
dateext suffix '-20180609'
glob pattern '-[0-9][0-9][0-9][0-9][0-9][0-9][0-9][0-9]'
renaming /var/log/admin.log.5.gz to /var/log/admin.log.6.gz (rotatecount 5, logstart 1, i 5), 
old log /var/log/admin.log.5.gz does not exist
renaming /var/log/admin.log.4.gz to /var/log/admin.log.5.gz (rotatecount 5, logstart 1, i 4), 
old log /var/log/admin.log.4.gz does not exist
renaming /var/log/admin.log.3.gz to /var/log/admin.log.4.gz (rotatecount 5, logstart 1, i 3), 
old log /var/log/admin.log.3.gz does not exist
renaming /var/log/admin.log.2.gz to /var/log/admin.log.3.gz (rotatecount 5, logstart 1, i 2), 
old log /var/log/admin.log.2.gz does not exist
renaming /var/log/admin.log.1.gz to /var/log/admin.log.2.gz (rotatecount 5, logstart 1, i 1), 
old log /var/log/admin.log.1.gz does not exist
renaming /var/log/admin.log.0.gz to /var/log/admin.log.1.gz (rotatecount 5, logstart 1, i 0), 
old log /var/log/admin.log.0.gz does not exist
log /var/log/admin.log.6.gz doesn't exist -- won't try to dispose of it
running prerotate script
switching euid to 0 and egid to 0
renaming /var/log/admin.log to /var/log/admin.log.1
running postrotate script
switching euid to 0 and egid to 0
syslogd: no process found
/usr/bin/chattr: No such file or directory while trying to stat /var/log/admin.log
error: error running shared postrotate script for '/var/log/admin.log '
switching euid to 0 and egid to 0
 
 
 suck ! I have tried to commit many time but the network is suck

/
### Hello! continue my study record 18/6/12 today we still meet numerous problems
first one: When I start my bit-32 firefox ,this error occured
{XPCOMGlueLoad error for file /opt/firefox/libmozgtk.so:
libgtk-3.so.0: wrong ELF class: ELFCLASS64
Couldn't load XPCOM.}

By google for answer,I need to reinstall all package with 32-bite
BTW,never forget reading the original question commited on stack overflow before copying command line to your terminal
Then,I just simplely give up.

Next I head to downgrade gcc verison so I am able to match my kernal compiler to install nvidia driver..
I have heard that update-alternatives is a good tool on ubuntu to change some sofeware version.
Thing becomes more wir I have already install gcc but since I have typed this commond
update-alternatives --list gcc 
gcc link is broken and need install gcc again
BUT,when I apt install gcc ,It ture out that I have the newest version!WTF

