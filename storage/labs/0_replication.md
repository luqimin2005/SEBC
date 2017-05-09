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
[root@ip-172-31-35-195 ~]# hadoop fs -ls /test/luqimin2005/source
Found 2 items
-rw-r--r--   3 hdfs supergroup          0 2017-05-09 03:50 /test/luqimin2005/source/_SUCCESS
-rw-r--r--   3 hdfs supergroup  524288000 2017-05-09 03:50 /test/luqimin2005/source/part-m-00000
```


