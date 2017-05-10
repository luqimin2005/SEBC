
Hive Stop:
```
[root@ip-172-31-35-195 ~]# curl -X POST -u luqimin2005:cloudera 'http://172.31.35.195:7180/api/v1/clusters/luqimin2005/services/hive/commands/stop'
{
  "id" : 835,
  "name" : "Stop",
  "startTime" : "2017-05-10T03:45:11.850Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }

```

Hive Start:
```
[root@ip-172-31-35-195 ~]# curl -X POST -u luqimin2005:cloudera 'http://172.31.35.195:7180/api/v1/clusters/luqimin2005/services/hive/commands/start'
{
  "id" : 840,
  "name" : "Start",
  "startTime" : "2017-05-10T03:46:06.801Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }

```

Hive Status:
```

```
