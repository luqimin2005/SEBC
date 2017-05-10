Upgraded CM from 5.9.2 to 5.11.0
***

The latest available version of the API
```
[root@ip-172-31-35-195 ~]# curl -u luqimin2005:cloudera http://172.31.35.195:7180/api/version
v16
```

The CM version
```
[root@ip-172-31-35-195 ~]# curl -u luqimin2005:cloudera http://172.31.35.195:7180/api/v16/cm/version
{
  "version" : "5.11.0",
  "buildUser" : "jenkins",
  "buildTimestamp" : "20170412-1249",
  "gitHash" : "70cb1442626406432a6e7af5bdf206a384ca3f98",
  "snapshot" : false
}
```

List all CM users
```
[root@ip-172-31-35-195 ~]# curl -u luqimin2005:cloudera http://172.31.35.195:7180/api/v16/users
{
  "items" : [ {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ]
  }, {
    "name" : "luqimin2005",
    "roles" : [ "ROLE_ADMIN" ]
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ]
  } ]
}
```

The database server in use by CM
```
[root@ip-172-31-35-195 ~]# curl -X GET -u luqimin2005:cloudera http://172.31.35.195:7180/api/v16/cm/scmDbInfo
{
  "scmDbType" : "MYSQL",
  "embeddedDbUsed" : false
}
```
