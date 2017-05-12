List the cloud provider you are using 
```
AWS
```

List your instances by their IP address and DNS name
```
172.31.36.237	ip-172-31-36-237
172.31.38.5	ip-172-31-38-5
172.31.41.1	ip-172-31-41-1
172.31.44.121	ip-172-31-44-121
172.31.46.221	ip-172-31-46-221
```

List the Linux release you are using
```
CentOS release 6.5 (Final)
```

List the file system capacity for the first node
```
[root@ip-172-31-36-237 ~]# df -hT
Filesystem     Type   Size  Used Avail Use% Mounted on
/dev/xvde      ext4    30G  749M   28G   3% /
tmpfs          tmpfs  7.4G     0  7.4G   0% /dev/shm
```

List the command and output for yum repolist enabled
```
[root@ip-172-31-36-237 ~]# yum repolist enabled
Loaded plugins: fastestmirror, presto
Loading mirror speeds from cached hostfile
 * base: mirror.pac-12.org
 * extras: mirror.chpc.utah.edu
 * updates: repos.lax.quadranet.com
base                                                                                                | 3.7 kB     00:00     
extras                                                                                              | 3.4 kB     00:00     
updates                                                                                             | 3.4 kB     00:00     
repo id                                              repo name                                                       status
base                                                 CentOS-6 - Base                                                 6,706
extras                                               CentOS-6 - Extras                                                  64
updates                                              CentOS-6 - Updates                                                270
repolist: 7,040
```

List the /etc/passwd entries for zhou and chen
```
[root@ip-172-31-36-237 ~]# cat /etc/passwd | grep zhou
zhou:x:2800:2800::/home/zhou:/bin/bash
[root@ip-172-31-36-237 ~]# cat /etc/passwd | grep chen
chen:x:2900:2900::/home/chen:/bin/bash
```

List the /etc/group entries for shanghai and beijing
```
[root@ip-172-31-36-237 ~]# cat /etc/group | grep shanghai
shanghai:x:2901:chen
[root@ip-172-31-36-237 ~]# cat /etc/group | grep beijing
beijing:x:2902:zhou
```

