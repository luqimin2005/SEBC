
http://ec2-52-88-204-134.us-west-2.compute.amazonaws.com:7180/api/v2/cm/deployment
```
{
  "timestamp" : "2017-05-10T03:30:23.309Z",
  "clusters" : [ {
    "name" : "luqimin2005",
    "version" : "CDH5",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "HIVEMETASTORE",
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "1548746752"
          }, {
            "name" : "hive_metastore_server_max_message_size",
            "value" : "154874675"
          } ]
        }, {
          "roleType" : "HIVESERVER2",
          "items" : [ {
            "name" : "hiveserver2_java_heapsize",
            "value" : "1548746752"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "912680550"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "153"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "ip-172-31-35-195"
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "hive_password"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-167b7a52e7ddae9bd0c2f5bb0e28e7cc",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-09fc91b9cc4e540fa"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-1bfc054487e550097c6e893d8040d77f",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-04ec6151b4c8d8f43"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-5b006429c0621ab32c2ee8c9b16e00b4",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-00961cda4e7247e97"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-88eb5a727a793b685a4135df95eca5f0",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-02f2e32e68a6e8387"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-8c20160685cc7943f1289549045e7ec7",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-079a7953bcff585e1"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-88eb5a727a793b685a4135df95eca5f0",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "i-02f2e32e68a6e8387"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5d8nap7ndvbcrwc4rrq09jbm5"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-88eb5a727a793b685a4135df95eca5f0",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "i-02f2e32e68a6e8387"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7mlxzli7wgz2kvduw093k01uu"
          } ]
        }
      }, {
        "name" : "hive-WEBHCAT-88eb5a727a793b685a4135df95eca5f0",
        "type" : "WEBHCAT",
        "hostRef" : {
          "hostId" : "i-02f2e32e68a6e8387"
        },
        "config" : {
          "items" : [ {
            "name" : "hive_webhcat_secret_key",
            "value" : "dTL4bHuiCund9UcLcFzbZL3RfQ6Hc0"
          }, {
            "name" : "role_jceks_password",
            "value" : "6urox30xgddimgoaqdmm8me1"
          } ]
        }
      } ],
      "displayName" : "Hive"
    }, {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-167b7a52e7ddae9bd0c2f5bb0e28e7cc",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-09fc91b9cc4e540fa"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "a9m6p17w6l4wngp1n3re1bz64"
          }, {
            "name" : "serverId",
            "value" : "1"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-88eb5a727a793b685a4135df95eca5f0",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-02f2e32e68a6e8387"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "pb55hfgj5dayai9egnk9olx7"
          }, {
            "name" : "serverId",
            "value" : "3"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-8c20160685cc7943f1289549045e7ec7",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-079a7953bcff585e1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "gfrd2a9d6wwwqrlawgygipu6"
          }, {
            "name" : "serverId",
            "value" : "2"
          } ]
        }
      } ],
      "displayName" : "ZooKeeper"
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ {
          "name" : "database_host",
          "value" : "ip-172-31-35-195"
        }, {
          "name" : "database_password",
          "value" : "hue"
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-HTTPFS-5b006429c0621ab32c2ee8c9b16e00b4"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-5b006429c0621ab32c2ee8c9b16e00b4",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "i-00961cda4e7247e97"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "71yp5xmy4ukzgzjxmvjm04oq1"
          }, {
            "name" : "secret_key",
            "value" : "H5GuDBisdvRtKQpk9OoGnCNbjns4et"
          } ]
        }
      } ],
      "displayName" : "Hue"
    }, {
      "name" : "oozie",
      "type" : "OOZIE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "OOZIE_SERVER",
          "items" : [ {
            "name" : "oozie_database_host",
            "value" : "ip-172-31-34-57"
          }, {
            "name" : "oozie_database_password",
            "value" : "oozie"
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie"
          }, {
            "name" : "oozie_java_heapsize",
            "value" : "713031680"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-5b006429c0621ab32c2ee8c9b16e00b4",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "i-00961cda4e7247e97"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6zi587rdgcyia7yqdc4x0bk6b"
          } ]
        }
      } ],
      "displayName" : "Oozie"
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "mapred_reduce_tasks",
            "value" : "10"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "2"
          } ]
        }, {
          "roleType" : "NODEMANAGER",
          "items" : [ {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100"
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm"
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs"
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "4"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "5250"
          } ]
        }, {
          "roleType" : "RESOURCEMANAGER",
          "items" : [ {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "5250"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "3"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "80"
        }, {
          "name" : "yarn_service_cgroups",
          "value" : "false"
        }, {
          "name" : "yarn_service_lce_always",
          "value" : "false"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "w6BKICHgNj5GmNxc5F67FMo3qNwC2Q"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-8c20160685cc7943f1289549045e7ec7",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "i-079a7953bcff585e1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "zkvjlvkhy4qlsj5ickz58w44"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-167b7a52e7ddae9bd0c2f5bb0e28e7cc",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-09fc91b9cc4e540fa"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6fs08a98159n1rqdos2v0hfz5"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-1bfc054487e550097c6e893d8040d77f",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-04ec6151b4c8d8f43"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2z6qhz10bswynr1gf9v6e5w55"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-5b006429c0621ab32c2ee8c9b16e00b4",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-00961cda4e7247e97"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "af0t9rimh6es8u4dgcw065w5u"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-88eb5a727a793b685a4135df95eca5f0",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-02f2e32e68a6e8387"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7ank9fa162agfem6ld83zckoo"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-8c20160685cc7943f1289549045e7ec7",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-079a7953bcff585e1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "cg9f927d2ljrilluw7q9ah2yz"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-8c20160685cc7943f1289549045e7ec7",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "i-079a7953bcff585e1"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "62"
          }, {
            "name" : "role_jceks_password",
            "value" : "5hekk9udyfrd3zssyi6uoly0z"
          } ]
        }
      } ],
      "displayName" : "YARN (MR2 Included)"
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "DATANODE",
          "items" : [ {
            "name" : "datanode_java_heapsize",
            "value" : "1073741824"
          }, {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "3170683699"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "4294967296"
          } ]
        }, {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true"
          } ]
        }, {
          "roleType" : "JOURNALNODE",
          "items" : [ {
            "name" : "dfs_journalnode_edits_dir",
            "value" : "/jn"
          } ]
        }, {
          "roleType" : "NAMENODE",
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/dfs/nn"
          }, {
            "name" : "dfs_namenode_handler_count",
            "value" : "32"
          }, {
            "name" : "dfs_namenode_service_handler_count",
            "value" : "32"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          }, {
            "name" : "namenode_java_heapsize",
            "value" : "1073741824"
          }, {
            "name" : "role_config_suppression_namenode_java_heapsize_minimum_validator",
            "value" : "true"
          } ]
        }, {
          "roleType" : "SECONDARYNAMENODE",
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/dfs/snn"
          }, {
            "name" : "secondary_namenode_java_heapsize",
            "value" : "1073741824"
          } ]
        } ],
        "items" : [ {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "E3ljgGH2jeRmHt4gZXeMlw5ZisLJ80"
        }, {
          "name" : "dfs_ha_fencing_methods",
          "value" : "shell(true)"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "M7mytlGliQP4qOGyPgGT21D1eeSmk8"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "1BUdTkIl7ym2wUnO887LecaBNgNZLh"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "20"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-8c20160685cc7943f1289549045e7ec7",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "i-079a7953bcff585e1"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-167b7a52e7ddae9bd0c2f5bb0e28e7cc",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-09fc91b9cc4e540fa"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6y1dkrvmtndt1iv0w9s2s9f0y"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-1bfc054487e550097c6e893d8040d77f",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-04ec6151b4c8d8f43"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dr84hyw3sxtdrgbmf3dbvaowx"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-5b006429c0621ab32c2ee8c9b16e00b4",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-00961cda4e7247e97"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "cywh20vwmyqg6sl8mpo4injvl"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-88eb5a727a793b685a4135df95eca5f0",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-02f2e32e68a6e8387"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1pd0dy9vu4d1lextsprpgkzmf"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-8c20160685cc7943f1289549045e7ec7",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-079a7953bcff585e1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1lkgscfavmoyjoxqa03g1u85p"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-88eb5a727a793b685a4135df95eca5f0",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "i-02f2e32e68a6e8387"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "abzzuoin9po9mrkajjkc7kc2b"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-8c20160685cc7943f1289549045e7ec7",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "i-079a7953bcff585e1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "e5fvijxxs2u66def3wu4kjcyc"
          } ]
        }
      }, {
        "name" : "hdfs-HTTPFS-5b006429c0621ab32c2ee8c9b16e00b4",
        "type" : "HTTPFS",
        "hostRef" : {
          "hostId" : "i-00961cda4e7247e97"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8gm85oq1m5l9ten4ejjswhdpd"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-167b7a52e7ddae9bd0c2f5bb0e28e7cc",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "i-09fc91b9cc4e540fa"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_journalnode_edits_dir",
            "value" : "/dfs/jn"
          }, {
            "name" : "role_jceks_password",
            "value" : "5cbrfkmhi0np08ihhjjb1chb9"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-88eb5a727a793b685a4135df95eca5f0",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "i-02f2e32e68a6e8387"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_journalnode_edits_dir",
            "value" : "/dfs/jn"
          }, {
            "name" : "role_jceks_password",
            "value" : "b8trpfccvz3ke2bo0wj4a5gm1"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-8c20160685cc7943f1289549045e7ec7",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "i-079a7953bcff585e1"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_journalnode_edits_dir",
            "value" : "/dfs/jn"
          }, {
            "name" : "role_jceks_password",
            "value" : "am27dvozrw5pjrt29n58ew5et"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-88eb5a727a793b685a4135df95eca5f0",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "i-02f2e32e68a6e8387"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "luqimin2005"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "luqimin2005"
          }, {
            "name" : "namenode_id",
            "value" : "80"
          }, {
            "name" : "role_jceks_password",
            "value" : "doek16gu0bpjy2bv816g1gspk"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-8c20160685cc7943f1289549045e7ec7",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "i-079a7953bcff585e1"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "luqimin2005"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "luqimin2005"
          }, {
            "name" : "namenode_id",
            "value" : "66"
          }, {
            "name" : "role_jceks_password",
            "value" : "e0bur1hxkyphuu7fl47j4bcfs"
          } ]
        }
      } ],
      "displayName" : "HDFS"
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "i-00961cda4e7247e97",
    "ipAddress" : "172.31.34.57",
    "hostname" : "ip-172-31-34-57",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-079a7953bcff585e1",
    "ipAddress" : "172.31.35.195",
    "hostname" : "ip-172-31-35-195",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-02f2e32e68a6e8387",
    "ipAddress" : "172.31.35.75",
    "hostname" : "ip-172-31-35-75",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-09fc91b9cc4e540fa",
    "ipAddress" : "172.31.38.142",
    "hostname" : "ip-172-31-38-142",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-04ec6151b4c8d8f43",
    "ipAddress" : "172.31.47.179",
    "hostname" : "ip-172-31-47-179",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__54cd4e1d-3f27-4b8c-9972-536185f597b3",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "d57e58dfe0531a1c57efece7162080ff87879448e2717b194a0adb6e20cc3d3c",
    "pwSalt" : -8651375003884873630,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__e43b0ec2-c912-4182-813a-795a9ceed1c9",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "c604106f2add8be80b9a0008bc588cebd64b551c0cfd693266046403effd1ed8",
    "pwSalt" : -4379491772074245104,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-ACTIVITYMONITOR-5b006429c0621ab32c2ee8c9b16e00b4",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "70b3dc29410cae26fd3216beb973dfca54fad2945d7d57bc1637d8374c998238",
    "pwSalt" : -4783284258844570701,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-5b006429c0621ab32c2ee8c9b16e00b4",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "880ccb7bab334232f973f2bcf02a1697b5e6a852960a2b478fd7b7a9fd30d58f",
    "pwSalt" : 5250202085628076078,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-5b006429c0621ab32c2ee8c9b16e00b4",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "47833c77da310d0db83b3d5abda414914061061cc1f81f6ad49047868cd848b1",
    "pwSalt" : 3907698489560562979,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-5b006429c0621ab32c2ee8c9b16e00b4",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "97d1fb38c700e60654fa86bd8b01a6f4681372df20b1c0cc2119a45b8a372f13",
    "pwSalt" : 1928304433345572579,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-5b006429c0621ab32c2ee8c9b16e00b4",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "6ecda49390dac1797d022e239bffdadc3bc1e7b0e8eed7e4db04d4d68f5c5a6c",
    "pwSalt" : -128290007073775417,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ],
    "pwHash" : "f8cd8fcc4c83ed1fcf6854f19c87859edd421d84f6a016114eca066e4b7f5efc",
    "pwSalt" : 399700203967354088,
    "pwLogin" : true
  }, {
    "name" : "luqimin2005",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "2adab192f07fc9f23dacd3315e16803ce76ee419abf1f52cfc8e3272b689cc1a",
    "pwSalt" : 6519572533304686886,
    "pwLogin" : true
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ],
    "pwHash" : "5d83f5468e9c90da79599b9b430b973b7b92a1672c57875bb7f3f1de2e4eec69",
    "pwSalt" : -4269551325870171447,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.9.2",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20170330-1814",
    "gitHash" : "822da28bff818f57fc1bfc3eafe3a550300ef1b0",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "roleTypeConfigs" : [ {
        "roleType" : "ACTIVITYMONITOR",
        "items" : [ {
          "name" : "firehose_database_host",
          "value" : "ip-172-31-35-195"
        }, {
          "name" : "firehose_database_name",
          "value" : "amon"
        }, {
          "name" : "firehose_database_password",
          "value" : "amon_password"
        }, {
          "name" : "firehose_database_user",
          "value" : "amon"
        }, {
          "name" : "firehose_heapsize",
          "value" : "713031680"
        } ]
      }, {
        "roleType" : "EVENTSERVER",
        "items" : [ {
          "name" : "event_server_heapsize",
          "value" : "713031680"
        } ]
      }, {
        "roleType" : "HOSTMONITOR",
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "713031680"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "926941184"
        }, {
          "name" : "role_config_suppression_firehose_heap_size_validator",
          "value" : "true"
        }, {
          "name" : "role_config_suppression_firehose_non_java_memory_validator",
          "value" : "true"
        } ]
      }, {
        "roleType" : "REPORTSMANAGER",
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "ip-172-31-35-195"
        }, {
          "name" : "headlamp_database_name",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_password",
          "value" : "rman_password"
        }, {
          "name" : "headlamp_database_user",
          "value" : "rman"
        }, {
          "name" : "headlamp_heapsize",
          "value" : "713031680"
        } ]
      }, {
        "roleType" : "SERVICEMONITOR",
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "713031680"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "926941184"
        }, {
          "name" : "role_config_suppression_firehose_heap_size_validator",
          "value" : "true"
        }, {
          "name" : "role_config_suppression_firehose_non_java_memory_validator",
          "value" : "true"
        } ]
      } ],
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ACTIVITYMONITOR-5b006429c0621ab32c2ee8c9b16e00b4",
      "type" : "ACTIVITYMONITOR",
      "hostRef" : {
        "hostId" : "i-00961cda4e7247e97"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "efs0kyj0j2o8v7xr6shzegcnj"
        } ]
      }
    }, {
      "name" : "mgmt-ALERTPUBLISHER-5b006429c0621ab32c2ee8c9b16e00b4",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "i-00961cda4e7247e97"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "eh6y0kg8v7w9sxtm30h8298o1"
        } ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-5b006429c0621ab32c2ee8c9b16e00b4",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "i-00961cda4e7247e97"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "e3nphj8b5eketfp43m2w95or6"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-5b006429c0621ab32c2ee8c9b16e00b4",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "i-00961cda4e7247e97"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "17z0m0t776az44ormopsp217v"
        } ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-5b006429c0621ab32c2ee8c9b16e00b4",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "i-00961cda4e7247e97"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "a3xpkct1qqpozmartxtkaxpq7"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-5b006429c0621ab32c2ee8c9b16e00b4",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "i-00961cda4e7247e97"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "dqnck48fyxnops7qtnowje21o"
        } ]
      }
    } ],
    "displayName" : "Cloudera Management Service"
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/25/2012 10:00"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/,http://172.31.47.179/cdh5.11,http://172.31.47.179/cdh5.8.4"
    } ]
  }
}

```
