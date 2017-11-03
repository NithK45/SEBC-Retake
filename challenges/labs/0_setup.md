Cloud provider AWS

Instance IPS
```
172.31.44.20
172.31.38.243
172.31.43.3
172.31.42.120
172.31.33.170
```

DNS
```
ip-172-31-44-20.us-west-2.compute.internal
ip-172-31-38-243.us-west-2.compute.internal
ip-172-31-43-3.us-west-2.compute.internal
ip-172-31-42-120.us-west-2.compute.internal
ip-172-31-33-170.us-west-2.compute.internal
```

linux release
```
[root@ip-172-31-33-170 ~]# cat /etc/centos-release
CentOS release 6.5 (Final)
```

file system capacity
```
[root@ip-172-31-44-20 ~]# df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvde        30G  806M   28G   3% /
tmpfs           7.4G     0  7.4G   0% /dev/shm
```

yum repolist enabled output
```
[root@ip-172-31-44-20 ~]# yum repolist enabled
Loaded plugins: fastestmirror, presto
Loading mirror speeds from cached hostfile
 * base: mirror.pac-12.org
 * extras: mirrors.unifiedlayer.com
 * updates: mirror.sfo12.us.leaseweb.net
repo id                        repo name                                  status
base                           CentOS-6 - Base                            6,706
extras                         CentOS-6 - Extras                             46
updates                        CentOS-6 - Updates                           756
repolist: 7,508

```

output of /etc/passwd
```
reilly:x:2800:501::/home/reilly:/bin/bash
frankola:x:2900:500::/home/frankola:/bin/bash

```
output of /etc/group
````
paloalto:x:500:
sanfrancisco:x:501:

```