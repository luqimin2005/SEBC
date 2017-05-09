
Create a precious directory in HDFS; copy the ZIP course file into it
```
[root@ip-172-31-35-195 ~]# hadoop fs -ls /precious
Found 1 items
-rw-r--r--   3 hdfs supergroup     474957 2017-05-09 06:53 /precious/SEBC-Shanghai.zip
```

Enable snapshots for precious
```
[root@ip-172-31-35-195 ~]# sudo -u hdfs hdfs dfsadmin -allowSnapshot /precious
Allowing snaphot on /precious succeeded
```

Create a snapshot called sebc-hdfs-test
```
[root@ip-172-31-35-195 ~]# sudo -u hdfs hdfs dfs -createSnapshot /precious sebc-hdfs-test
Created snapshot /precious/.snapshot/sebc-hdfs-test
```

Delete the directory
```
[root@ip-172-31-35-195 ~]# sudo -u hdfs hdfs dfs -rm -r -skipTrash /precious
rm: The directory /precious cannot be deleted since /precious is snapshottable and already has snapshots
```

Delete the ZIP file
```
[root@ip-172-31-35-195 ~]# sudo -u hdfs hdfs dfs -rm -r -skipTrash /precious/SEBC-Shanghai.zip
Deleted /precious/SEBC-Shanghai.zip
```

Restore the deleted file
```
[root@ip-172-31-35-195 ~]# sudo -u hdfs hdfs dfs -cp /precious/.snapshot/sebc-hdfs-test/SEBC-Shanghai.zip /precious/SEBC-Shanghai.zip
[root@ip-172-31-35-195 ~]# hdfs dfs -ls /precious
Found 1 items
-rw-r--r--   3 hdfs supergroup     474957 2017-05-09 07:07 /precious/SEBC-Shanghai.zip
```
