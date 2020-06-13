# debianize_karfa

The files I added to make a debian package of Karka, 2.50

Download the binary tgz distrbution from Apache
Then copy this directory over the top.

You can then build a debian package with a normal looking:

```
debuild -us -uc 
```

Installs ok despite the non debian layout

```
root@frank:~# dpkg -i kafka_2.50_all.deb 
Selecting previously unselected package kafka.
(Reading database ... 33047 files and directories currently installed.)
Preparing to unpack kafka_2.50_all.deb ...
Unpacking kafka (2.50) ...
Setting up kafka (2.50) ...
Warning: The home dir /usr/local/kafka you specified already exists.
Adding system user `kafka' (UID 106) ...
Adding new user `kafka' (UID 106) with group `nogroup' ...
The home directory `/usr/local/kafka' already exists.  Not copying from `/etc/skel'.
```
