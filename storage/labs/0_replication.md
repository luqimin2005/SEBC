Choose a partner in class
```
xiaohu-liu
```

Name a source directory after your GitHub handle
Name a target directory after your partner's GitHub handle
```
[root@ip-172-31-35-195 ~]# hadoop fs -ls /test
Found 2 items
drwxr-xr-x   - root supergroup          0 2017-05-09 03:41 /test/luqimin2005
drwxr-xr-x   - root supergroup          0 2017-05-09 03:41 /test/xiaohu-liu
```

Use teragen to create a 500 MB file
```
[root@ip-172-31-35-195 ~]# sudo -u hdfs hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar  teragen -Dmapreduce.job.maps=1  5242880 /test/luqimin2005/source

[root@ip-172-31-35-195 ~]# hadoop fs -ls /test/luqimin2005/source
Found 2 items
-rw-r--r--   3 hdfs supergroup          0 2017-05-09 03:50 /test/luqimin2005/source/_SUCCESS
-rw-r--r--   3 hdfs supergroup  524288000 2017-05-09 03:50 /test/luqimin2005/source/part-m-00000
```

My source fsck
```
[root@ip-172-31-35-195 ~]# sudo -u hdfs hdfs fsck /test/luqimin2005/source -files -blocks
Connecting to namenode via http://ip-172-31-35-75:50070
FSCK started by hdfs (auth:SIMPLE) from /172.31.35.195 for path /test/luqimin2005/source at Tue May 09 12:39:13 UTC 2017
/test/luqimin2005/source <dir>
/test/luqimin2005/source/_SUCCESS 0 bytes, 0 block(s):  OK

/test/luqimin2005/source/part-m-00000 524288000 bytes, 4 block(s):  OK
0. BP-1132382126-172.31.35.195-1494244091384:blk_1073743500_2676 len=134217728 Live_repl=3
1. BP-1132382126-172.31.35.195-1494244091384:blk_1073743501_2677 len=134217728 Live_repl=3
2. BP-1132382126-172.31.35.195-1494244091384:blk_1073743502_2678 len=134217728 Live_repl=3
3. BP-1132382126-172.31.35.195-1494244091384:blk_1073743503_2679 len=121634816 Live_repl=3

Status: HEALTHY
 Total size:	524288000 B
 Total dirs:	1
 Total files:	2
 Total symlinks:		0
 Total blocks (validated):	4 (avg. block size 131072000 B)
 Minimally replicated blocks:	4 (100.0 %)
 Over-replicated blocks:	0 (0.0 %)
 Under-replicated blocks:	0 (0.0 %)
 Mis-replicated blocks:		0 (0.0 %)
 Default replication factor:	3
 Average block replication:	3.0
 Corrupt blocks:		0
 Missing replicas:		0 (0.0 %)
 Number of data-nodes:		5
 Number of racks:		1
FSCK ended at Tue May 09 12:39:13 UTC 2017 in 2 milliseconds


The filesystem under path '/test/luqimin2005/source' is HEALTHY

```

My target fsck
```
[root@ip-172-31-35-195 ~]# sudo -u hdfs hdfs fsck /test/xiaohu-liu -files -blocks
Connecting to namenode via http://ip-172-31-35-75:50070
FSCK started by hdfs (auth:SIMPLE) from /172.31.35.195 for path /test/xiaohu-liu at Tue May 09 12:39:28 UTC 2017
/test/xiaohu-liu <dir>
/test/xiaohu-liu/source <dir>
/test/xiaohu-liu/source/_SUCCESS 0 bytes, 0 block(s):  OK

/test/xiaohu-liu/source/part-m-00000 524288000 bytes, 4 block(s):  OK
0. BP-1132382126-172.31.35.195-1494244091384:blk_1073746375_5551 len=134217728 Live_repl=3
1. BP-1132382126-172.31.35.195-1494244091384:blk_1073746376_5552 len=134217728 Live_repl=3
2. BP-1132382126-172.31.35.195-1494244091384:blk_1073746377_5553 len=134217728 Live_repl=3
3. BP-1132382126-172.31.35.195-1494244091384:blk_1073746378_5554 len=121634816 Live_repl=3

Status: HEALTHY
 Total size:	524288000 B
 Total dirs:	2
 Total files:	2
 Total symlinks:		0
 Total blocks (validated):	4 (avg. block size 131072000 B)
 Minimally replicated blocks:	4 (100.0 %)
 Over-replicated blocks:	0 (0.0 %)
 Under-replicated blocks:	0 (0.0 %)
 Mis-replicated blocks:		0 (0.0 %)
 Default replication factor:	3
 Average block replication:	3.0
 Corrupt blocks:		0
 Missing replicas:		0 (0.0 %)
 Number of data-nodes:		5
 Number of racks:		1
FSCK ended at Tue May 09 12:39:28 UTC 2017 in 1 milliseconds


The filesystem under path '/test/xiaohu-liu' is HEALTHY

```
