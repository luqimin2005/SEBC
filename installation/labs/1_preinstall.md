 Check vm.swappiness on all your nodes
```
[root@ip-172-31-35-195 ~]# cat /proc/sys/vm/swappiness
1
```

Show the mount attributes of your volume(s)
```
[root@ip-172-31-35-195 ~]# cat /proc/mounts 
rootfs / rootfs rw 0 0
proc /proc proc rw,relatime 0 0
sysfs /sys sysfs rw,seclabel,relatime 0 0
devtmpfs /dev devtmpfs rw,seclabel,relatime,size=7674908k,nr_inodes=1918727,mode=755 0 0
devpts /dev/pts devpts rw,seclabel,relatime,gid=5,mode=620,ptmxmode=000 0 0
tmpfs /dev/shm tmpfs rw,seclabel,relatime 0 0
/dev/xvde / ext4 rw,seclabel,relatime,barrier=1,data=ordered 0 0
none /selinux selinuxfs rw,relatime 0 0
devtmpfs /dev devtmpfs rw,seclabel,relatime,size=7674908k,nr_inodes=1918727,mode=755 0 0
/proc/bus/usb /proc/bus/usb usbfs rw,relatime 0 0
none /proc/sys/fs/binfmt_misc binfmt_misc rw,relatime 0 0
```

If you have ext-based volumes, list the reserve space setting
```
[root@ip-172-31-35-195 ~]# cat /proc/mounts  | grep ext4
/dev/xvde / ext4 rw,seclabel,relatime,barrier=1,data=ordered 0 0
[root@ip-172-31-35-195 ~]# tune2fs -l /dev/xvde | grep "Reserved block count"
Reserved block count:     393145
```

Disable transparent hugepage support
```
[root@ip-172-31-35-195 ~]# cat /proc/meminfo | grep HugePages_Total
HugePages_Total:       0
```

List your network interface configuration
```
[root@ip-172-31-35-195 ~]# ifconfig
eth0      Link encap:Ethernet  HWaddr 06:1B:DF:D9:3D:02  
          inet addr:172.31.35.195  Bcast:172.31.47.255  Mask:255.255.240.0
          inet6 addr: fe80::41b:dfff:fed9:3d02/64 Scope:Link
          UP BROADCAST RUNNING MULTICAST  MTU:9001  Metric:1
          RX packets:28132 errors:0 dropped:0 overruns:0 frame:0
          TX packets:12733 errors:0 dropped:0 overruns:0 carrier:0
          collisions:0 txqueuelen:1000 
          RX bytes:28241816 (26.9 MiB)  TX bytes:1927173 (1.8 MiB)
          Interrupt:24 

lo        Link encap:Local Loopback  
          inet addr:127.0.0.1  Mask:255.0.0.0
          inet6 addr: ::1/128 Scope:Host
          UP LOOPBACK RUNNING  MTU:16436  Metric:1
          RX packets:0 errors:0 dropped:0 overruns:0 frame:0
          TX packets:0 errors:0 dropped:0 overruns:0 carrier:0
          collisions:0 txqueuelen:0 
          RX bytes:0 (0.0 b)  TX bytes:0 (0.0 b)
```

Show that forward and reverse host lookups are correctly resolved
```
[root@ip-172-31-35-195 ~]# getent hosts
127.0.0.1       localhost.localdomain localhost
127.0.0.1       localhost6.localdomain6 localhost6
172.31.35.195   ip-172-31-35-195
172.31.34.57    ip-172-31-34-57
172.31.35.75    ip-172-31-35-75
172.31.47.179   ip-172-31-47-179
172.31.38.142   ip-172-31-38-142
```

Show the nscd service is running
```
[root@ip-172-31-35-195 ~]# service nscd status
nscd (pid 6287) is running...
```

Show the ntpd service is running
```
[root@ip-172-31-35-195 ~]# service ntpd status
ntpd (pid  6315) is running...
```
