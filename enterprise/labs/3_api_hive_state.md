
Hive Stop:
```
[root@ip-172-31-35-195 ~]# curl -X POST -u luqimin2005:cloudera 'http://172.31.35.195:7180/api/v12/clusters/luqimin2005/services/hive/commands/stop'
{
  "id" : 869,
  "name" : "Stop",
  "startTime" : "2017-05-10T04:02:00.246Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}[root@ip-172-31-35-195 ~]# 

```
Hive Stoped State:
```
[root@ip-172-31-35-195 ~]# curl -u luqimin2005:cloudera 'http://172.31.35.195:7180/api/v12/commands/869'
{
  "id" : 869,
  "name" : "Stop",
  "startTime" : "2017-05-10T04:02:00.246Z",
  "endTime" : "2017-05-10T04:02:05.285Z",
  "active" : false,
  "success" : true,
  "resultMessage" : "Successfully stopped service.",
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  },
  "children" : {
    "items" : [ {
      "id" : 872,
      "name" : "Stop",
      "startTime" : "2017-05-10T04:02:00.252Z",
      "endTime" : "2017-05-10T04:02:05.284Z",
      "active" : false,
      "success" : true,
      "resultMessage" : "Successfully stopped process.",
      "serviceRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive"
      },
      "roleRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive",
        "roleName" : "hive-HIVEMETASTORE-88eb5a727a793b685a4135df95eca5f0"
      }
    }, {
      "id" : 870,
      "name" : "Stop",
      "startTime" : "2017-05-10T04:02:00.248Z",
      "endTime" : "2017-05-10T04:02:05.284Z",
      "active" : false,
      "success" : true,
      "resultMessage" : "Successfully stopped process.",
      "serviceRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive"
      },
      "roleRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive",
        "roleName" : "hive-WEBHCAT-88eb5a727a793b685a4135df95eca5f0"
      }
    }, {
      "id" : 871,
      "name" : "Stop",
      "startTime" : "2017-05-10T04:02:00.251Z",
      "endTime" : "2017-05-10T04:02:05.260Z",
      "active" : false,
      "success" : true,
      "resultMessage" : "Successfully stopped process.",
      "serviceRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive"
      },
      "roleRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive",
        "roleName" : "hive-HIVESERVER2-88eb5a727a793b685a4135df95eca5f0"
      }
    } ]
  },
  "canRetry" : false
}[root@ip-172-31-35-195 ~]# 

```

Hive Start:
```
[root@ip-172-31-35-195 ~]# curl -X POST -u luqimin2005:cloudera 'http://172.31.35.195:7180/api/v12/clusters/luqimin2005/services/hive/commands/start'
{
  "id" : 874,
  "name" : "Start",
  "startTime" : "2017-05-10T04:02:31.551Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}[root@ip-172-31-35-195 ~]# 

```

Hive Started State:
```
[root@ip-172-31-35-195 ~]# curl -u luqimin2005:cloudera 'http://172.31.35.195:7180/api/v12/clusters/luqimin2005/services/hive'
{
  "name" : "hive",
  "type" : "HIVE",
  "clusterRef" : {
    "clusterName" : "cluster"
  },
  "serviceUrl" : "http://ip-172-31-35-195:7180/cmf/serviceRedirect/hive",
  "roleInstancesUrl" : "http://ip-172-31-35-195:7180/cmf/serviceRedirect/hive/instances",
  "serviceState" : "STARTED",
  "healthSummary" : "GOOD",
  "healthChecks" : [ {
    "name" : "HIVE_HIVEMETASTORES_HEALTHY",
    "summary" : "GOOD",
    "suppressed" : false
  }, {
    "name" : "HIVE_HIVESERVER2S_HEALTHY",
    "summary" : "GOOD",
    "suppressed" : false
  }, {
    "name" : "HIVE_WEBHCATS_HEALTHY",
    "summary" : "GOOD",
    "suppressed" : false
  } ],
  "configStalenessStatus" : "FRESH",
  "clientConfigStalenessStatus" : "FRESH",
  "maintenanceMode" : false,
  "maintenanceOwners" : [ ],
  "displayName" : "Hive",
  "entityStatus" : "GOOD_HEALTH"
}[root@ip-172-31-35-195 ~]# 

```
