What is ubertask optimization?
```
Whether to enable ubertask optimization, which runs "sufficiently small" jobs sequentially within a single JVM. 
"Small" is defined by the mapreduce.job.ubertask.maxmaps, mapreduce.job.ubertask.maxreduces, 
and mapreduce.job.ubertask.maxbytes settings.
```

Where in CM is the Kerberos Security Realm value displayed?
```
Administration ---> Settings ---> CATEGORY ---> Kerberos ---> Kerberos Security Realm 
```

Which CDH service(s) host a property for enabling Kerberos authentication?
```
Zookeeper , HDFS , YARN , HIVE , Oozie , Hue
```

How do you upgrade the CM agents?
```

```

Give the tsquery statement used to chart Hue's CPU utilization?
```
select cpu_system_rate + cpu_user_rate where category=ROLE and serviceName=hue
```

Name all the roles that make up the Hive service
```
Hive Gateway
Hive Metastore Server
HiveServer2
WebHCat Server
```

What steps must be completed before integrating Cloudera Manager with Kerberos?
```

```
