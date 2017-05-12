List the command and output for ls /etc/yum.repos.d
```
[root@ip-172-31-38-5 ~]# ls /etc/yum.repos.d/
CentOS-Base.repo       CentOS-Media.repo  cloudera-manager.repo  mysql-community-source.repo
CentOS-Debuginfo.repo  CentOS-Vault.repo  mysql-community.repo

```

Use the scm_prepare_database.sh script to create the db.properties file
```
[root@ip-172-31-38-5 ~]# /usr/share/cmf/schema/scm_prepare_database.sh mysql -hip-172-31-36-237 -utemp -ptemp --scm-host ip-172-31-38-5 scm scm scm
JAVA_HOME=/usr/java/jdk1.7.0_67-cloudera
Verifying that we can write to /etc/cloudera-scm-server
Creating SCM configuration file in /etc/cloudera-scm-server
Executing:  /usr/java/jdk1.7.0_67-cloudera/bin/java -cp /usr/share/java/mysql-connector-java.jar:/usr/share/java/oracle-connector-java.jar:/usr/share/cmf/schema/../lib/* com.cloudera.enterprise.dbutil.DbCommandExecutor /etc/cloudera-scm-server/db.properties com.cloudera.cmf.db.
[                          main] DbCommandExecutor              INFO  Successfully connected to database.
All done, your SCM database is configured correctly!

```
