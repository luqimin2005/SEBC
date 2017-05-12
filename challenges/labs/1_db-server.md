The hostname of your database server
```
[root@ip-172-31-36-237 ~]# hostname 
ip-172-31-36-237
```

The command and output for showing the database server version
```
[root@ip-172-31-36-237 ~]# mysql -V
mysql  Ver 14.14 Distrib 5.6.36, for Linux (x86_64) using  EditLine wrapper
```

The command and output for listing the databases created above
```
[root@ip-172-31-36-237 ~]# mysql -uroot -p -e "show databases"
Enter password: 
+--------------------+
| Database           |
+--------------------+
| information_schema |
| hive               |
| hue                |
| mysql              |
| oozie              |
| performance_schema |
| rman               |
| scm                |
| sentry             |
+--------------------+

```
