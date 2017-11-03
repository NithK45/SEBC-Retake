The command and output for hdfs dfs -ls /user

```
[root@ip-172-31-38-243 ~]# hdfs dfs -ls /user
Found 5 items
drwxrwxrwx   - mapred hadoop          0 2017-11-03 08:19 /user/history
drwxrwxr-t   - hive   hive            0 2017-11-03 08:21 /user/hive
drwxrwxr-x   - hue    hue             0 2017-11-03 08:21 /user/hue
drwxrwxr-x   - oozie  oozie           0 2017-11-03 08:22 /user/oozie
drwxr-x--x   - spark  spark           0 2017-11-03 08:20 /user/spark
[root@ip-172-31-38-243 ~]#
```
The command and output from the CM API call ../api/v5/hosts
```
[root@ip-172-31-38-243 ~]# curl -u admin:admin 'http://ec2-52-32-156-77.us-west-2.compute.amazonaws.com:7180/api/v5/hosts'
{
  "items" : [ {
    "hostId" : "i-038c81a93875d91cc",
    "ipAddress" : "172.31.33.170",
    "hostname" : "ip-172-31-33-170.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-38-243.us-west-2.compute.internal:7180/cmf/hostRedirect/i-038c81a93875d91cc",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "totalPhysMemBytes" : 15740305408
  }, {
    "hostId" : "i-0f0315f45e1d850f5",
    "ipAddress" : "172.31.38.243",
    "hostname" : "ip-172-31-38-243.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-38-243.us-west-2.compute.internal:7180/cmf/hostRedirect/i-0f0315f45e1d850f5",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "totalPhysMemBytes" : 15740305408
  }, {
    "hostId" : "i-08cf4470476efdce1",
    "ipAddress" : "172.31.42.120",
    "hostname" : "ip-172-31-42-120.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-38-243.us-west-2.compute.internal:7180/cmf/hostRedirect/i-08cf4470476efdce1",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "totalPhysMemBytes" : 15740305408
  }, {
    "hostId" : "i-0a765a424be73c151",
    "ipAddress" : "172.31.43.3",
    "hostname" : "ip-172-31-43-3.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-38-243.us-west-2.compute.internal:7180/cmf/hostRedirect/i-0a765a424be73c151",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "totalPhysMemBytes" : 15740305408
  }, {
    "hostId" : "i-0f236dc00314be139",
    "ipAddress" : "172.31.44.20",
    "hostname" : "ip-172-31-44-20.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-38-243.us-west-2.compute.internal:7180/cmf/hostRedirect/i-0f236dc00314be139",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "totalPhysMemBytes" : 15740305408
  } ]
}[root@ip-172-31-38-243 ~]#

```
The command and output from the CM API call ../api/v11/clusters/<githubName>/services
```
[root@ip-172-31-38-243 ~]# curl -u admin:admin 'http://ec2-52-32-156-77.us-west-2.compute.amazonaws.com:7180/api/v11/clusters/NithK45/services'
{
  "items" : [ {
    "name" : "hive",
    "type" : "HIVE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-38-243.us-west-2.compute.internal:7180/cmf/serviceRedirect/hive",
    "roleInstancesUrl" : "http://ip-172-31-38-243.us-west-2.compute.internal:7180/cmf/serviceRedirect/hive/instances",
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
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hive",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "zookeeper",
    "type" : "ZOOKEEPER",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-38-243.us-west-2.compute.internal:7180/cmf/serviceRedirect/zookeeper",
    "roleInstancesUrl" : "http://ip-172-31-38-243.us-west-2.compute.internal:7180/cmf/serviceRedirect/zookeeper/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "ZOOKEEPER_CANARY_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "ZOOKEEPER_SERVERS_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "ZooKeeper",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "hue",
    "type" : "HUE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-38-243.us-west-2.compute.internal:7180/cmf/serviceRedirect/hue",
    "roleInstancesUrl" : "http://ip-172-31-38-243.us-west-2.compute.internal:7180/cmf/serviceRedirect/hue/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HUE_HUE_SERVERS_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hue",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "oozie",
    "type" : "OOZIE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-38-243.us-west-2.compute.internal:7180/cmf/serviceRedirect/oozie",
    "roleInstancesUrl" : "http://ip-172-31-38-243.us-west-2.compute.internal:7180/cmf/serviceRedirect/oozie/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "OOZIE_OOZIE_SERVERS_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Oozie",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "yarn",
    "type" : "YARN",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-38-243.us-west-2.compute.internal:7180/cmf/serviceRedirect/yarn",
    "roleInstancesUrl" : "http://ip-172-31-38-243.us-west-2.compute.internal:7180/cmf/serviceRedirect/yarn/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "YARN_JOBHISTORY_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "YARN_NODE_MANAGERS_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "YARN_RESOURCEMANAGERS_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "YARN_USAGE_AGGREGATION_HEALTH",
      "summary" : "DISABLED",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "YARN (MR2 Included)",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "spark_on_yarn",
    "type" : "SPARK_ON_YARN",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-38-243.us-west-2.compute.internal:7180/cmf/serviceRedirect/spark_on_yarn",
    "roleInstancesUrl" : "http://ip-172-31-38-243.us-west-2.compute.internal:7180/cmf/serviceRedirect/spark_on_yarn/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Spark",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "hdfs",
    "type" : "HDFS",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-38-243.us-west-2.compute.internal:7180/cmf/serviceRedirect/hdfs",
    "roleInstancesUrl" : "http://ip-172-31-38-243.us-west-2.compute.internal:7180/cmf/serviceRedirect/hdfs/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HDFS_BLOCKS_WITH_CORRUPT_REPLICAS",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_CANARY_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_DATA_NODES_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_FREE_SPACE_REMAINING",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_HA_NAMENODE_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_MISSING_BLOCKS",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_UNDER_REPLICATED_BLOCKS",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "HDFS",
    "entityStatus" : "GOOD_HEALTH"
  } ]
}[root@ip-172-31-38-243 ~]#

```
The command and output for your CM deployment (yes, again)
```
[root@ip-172-31-38-243 ~]# curl -u admin:admin 'http://ec2-52-32-156-77.us-west-2.compute.amazonaws.com:7180/api/v2/cm/deployment'
{
  "timestamp" : "2017-11-03T08:26:53.789Z",
  "clusters" : [ {
    "name" : "NithK45",
    "version" : "CDH5",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "HIVEMETASTORE",
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "580911104"
          } ]
        }, {
          "roleType" : "HIVESERVER2",
          "items" : [ {
            "name" : "hiveserver2_java_heapsize",
            "value" : "580911104"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "4679270400"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "787"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "ip-172-31-44-20.us-west-2.compute.internal"
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "hive"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "spark_on_yarn_service",
          "value" : "spark_on_yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-577b123b289501485bbcd7f2c478cd49",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-08cf4470476efdce1"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-84605f78e0dcc198e7d36c1ae61e633c",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-0a765a424be73c151"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-8712269ceb5ae063a959f25111d67cfb",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-0f0315f45e1d850f5"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-aa6cac7c5ef2e1baee75c68b1412768c",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-0f236dc00314be139"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-ddb686fe5b3727b404abc759eeb81b32",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-038c81a93875d91cc"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-ddb686fe5b3727b404abc759eeb81b32",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "i-038c81a93875d91cc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "lgn2c0irbx3ylhxc28m1uphv"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-ddb686fe5b3727b404abc759eeb81b32",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "i-038c81a93875d91cc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "f47key0rlgnh0jxozmkkj88u9"
          } ]
        }
      } ],
      "displayName" : "Hive"
    }, {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "SERVER",
          "items" : [ {
            "name" : "zookeeper_server_java_heapsize",
            "value" : "580911104"
          } ]
        } ],
        "items" : [ ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-ddb686fe5b3727b404abc759eeb81b32",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-038c81a93875d91cc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1pl6gnyojuekswz96dk1ee76"
          }, {
            "name" : "serverId",
            "value" : "1"
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
          "value" : "ip-172-31-44-20.us-west-2.compute.internal"
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
          "value" : "hdfs-NAMENODE-ddb686fe5b3727b404abc759eeb81b32"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-ddb686fe5b3727b404abc759eeb81b32",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "i-038c81a93875d91cc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "290l3yuozrl3ftmwmmjeser1a"
          }, {
            "name" : "secret_key",
            "value" : "XKm63cl7dGvdW5xICMAhuVclbcyfwJ"
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
            "value" : "ip-172-31-44-20.us-west-2.compute.internal"
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
            "value" : "580911104"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "spark_on_yarn_service",
          "value" : "spark_on_yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-ddb686fe5b3727b404abc759eeb81b32",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "i-038c81a93875d91cc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "cjassvm5wi1d3kea42gksl7mr"
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
            "value" : "8"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "2"
          } ]
        }, {
          "roleType" : "JOBHISTORY",
          "items" : [ {
            "name" : "mr2_jobhistory_java_heapsize",
            "value" : "580911104"
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
            "name" : "resource_manager_java_heapsize",
            "value" : "580911104"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "5250"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "4"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "true"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "8YESmrQoxBShw9EVUi81Hp6CHjFEDb"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-ddb686fe5b3727b404abc759eeb81b32",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "i-038c81a93875d91cc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "b0go63ocpvqdzjf2rcnmseniu"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-577b123b289501485bbcd7f2c478cd49",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-08cf4470476efdce1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "18kwhxyth9mznc9hinox3so1j"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-84605f78e0dcc198e7d36c1ae61e633c",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-0a765a424be73c151"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ahd95l6x7a68gtkp1cvp3v2s9"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-8712269ceb5ae063a959f25111d67cfb",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-0f0315f45e1d850f5"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "is8yge1e4db1gn6mhk6cak02"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-aa6cac7c5ef2e1baee75c68b1412768c",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-0f236dc00314be139"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "aennq60zd35mayih6u06awcod"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-ddb686fe5b3727b404abc759eeb81b32",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "i-038c81a93875d91cc"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "55"
          }, {
            "name" : "role_jceks_password",
            "value" : "cwr2e99y12jz5nfggt1ptclf9"
          } ]
        }
      } ],
      "displayName" : "YARN (MR2 Included)"
    }, {
      "name" : "spark_on_yarn",
      "type" : "SPARK_ON_YARN",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ {
          "name" : "yarn_service",
          "value" : "yarn"
        } ]
      },
      "roles" : [ {
        "name" : "spar40365358-SPARK_YARN_HISTORY_SERVER-ddb686fe5b3727b404abc759e",
        "type" : "SPARK_YARN_HISTORY_SERVER",
        "hostRef" : {
          "hostId" : "i-038c81a93875d91cc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "cpuvu8ykkzwb3koepwb3heruu"
          } ]
        }
      }, {
        "name" : "spark_on_yarn-GATEWAY-577b123b289501485bbcd7f2c478cd49",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-08cf4470476efdce1"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "spark_on_yarn-GATEWAY-84605f78e0dcc198e7d36c1ae61e633c",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-0a765a424be73c151"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "spark_on_yarn-GATEWAY-8712269ceb5ae063a959f25111d67cfb",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-0f0315f45e1d850f5"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "spark_on_yarn-GATEWAY-aa6cac7c5ef2e1baee75c68b1412768c",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-0f236dc00314be139"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "spark_on_yarn-GATEWAY-ddb686fe5b3727b404abc759eeb81b32",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-038c81a93875d91cc"
        },
        "config" : {
          "items" : [ ]
        }
      } ],
      "displayName" : "Spark"
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "BALANCER",
          "items" : [ {
            "name" : "balancer_java_heapsize",
            "value" : "580911104"
          } ]
        }, {
          "roleType" : "DATANODE",
          "items" : [ {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "3170683699"
          } ]
        }, {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true"
          } ]
        }, {
          "roleType" : "NAMENODE",
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/dfs/nn"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          }, {
            "name" : "namenode_java_heapsize",
            "value" : "580911104"
          } ]
        }, {
          "roleType" : "SECONDARYNAMENODE",
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/dfs/snn"
          }, {
            "name" : "secondary_namenode_java_heapsize",
            "value" : "580911104"
          } ]
        } ],
        "items" : [ {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "6uTdvXwNEog92U2nBWY9sp5c20y7kD"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "6DzBMRLH1RIs4uvOVuGijL3DfrZUf3"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "OkuwJRZIyMDSCdzQMYY8LKKE2Plqne"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-ddb686fe5b3727b404abc759eeb81b32",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "i-038c81a93875d91cc"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-577b123b289501485bbcd7f2c478cd49",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-08cf4470476efdce1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bi4xy0crra74v7hul43c4ndpr"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-84605f78e0dcc198e7d36c1ae61e633c",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-0a765a424be73c151"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1v68jg11kp29veet398o2ej1o"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-8712269ceb5ae063a959f25111d67cfb",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-0f0315f45e1d850f5"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "c2lal5isyjhh9lthsbi9eev5k"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-aa6cac7c5ef2e1baee75c68b1412768c",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-0f236dc00314be139"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "87ts9wnbxg9y6wasn0t7bml7s"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-ddb686fe5b3727b404abc759eeb81b32",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "i-038c81a93875d91cc"
        },
        "config" : {
          "items" : [ {
            "name" : "namenode_id",
            "value" : "63"
          }, {
            "name" : "role_jceks_password",
            "value" : "1gozoe47extnknz831bkf3pi8"
          } ]
        }
      }, {
        "name" : "hdfs-SECONDARYNAMENODE-ddb686fe5b3727b404abc759eeb81b32",
        "type" : "SECONDARYNAMENODE",
        "hostRef" : {
          "hostId" : "i-038c81a93875d91cc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "680bdrz1fqvcx289238n391mk"
          } ]
        }
      } ],
      "displayName" : "HDFS"
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "i-038c81a93875d91cc",
    "ipAddress" : "172.31.33.170",
    "hostname" : "ip-172-31-33-170.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-0f0315f45e1d850f5",
    "ipAddress" : "172.31.38.243",
    "hostname" : "ip-172-31-38-243.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-08cf4470476efdce1",
    "ipAddress" : "172.31.42.120",
    "hostname" : "ip-172-31-42-120.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-0a765a424be73c151",
    "ipAddress" : "172.31.43.3",
    "hostname" : "ip-172-31-43-3.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-0f236dc00314be139",
    "ipAddress" : "172.31.44.20",
    "hostname" : "ip-172-31-44-20.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-ddb686fe5b3727b404abc759eeb81b32",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "a8e82d8f8db001defeed1799754ed8848f07567ef1d2cdc0daa1cc3757e739d1",
    "pwSalt" : 8560020191924456455,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-ddb686fe5b3727b404abc759eeb81b32",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "e585cfe346589cd86ea8ca6334e84999f52fa2af72a19aea0fa834cf9ed8e310",
    "pwSalt" : -4919902554870068371,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-ddb686fe5b3727b404abc759eeb81b32",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "d6969b016f42d8873c21eab1c6ef399b1cf09ebc05cc677a34551106fb0a30d5",
    "pwSalt" : -5153054677457566786,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-ddb686fe5b3727b404abc759eeb81b32",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "17251d3ce27ea75c3430beb5f831de1d750ee82f113b1595ca57832edc000e15",
    "pwSalt" : -6416145594110984880,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "968a7d3c36035ae060c41c7c2e21b0e0d1d81517c8ee10a0babd53c7afe73940",
    "pwSalt" : 2470426282483829451,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.8.5",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20170505-1728",
    "gitHash" : "d71107915045c3789ec1971e3656459b98a0df5e",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "roleTypeConfigs" : [ {
        "roleType" : "EVENTSERVER",
        "items" : [ {
          "name" : "event_server_heapsize",
          "value" : "580911104"
        } ]
      }, {
        "roleType" : "HOSTMONITOR",
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "580911104"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "805306368"
        } ]
      }, {
        "roleType" : "REPORTSMANAGER",
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "ip-172-31-44-20.us-west-2.compute.internal"
        }, {
          "name" : "headlamp_database_name",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_password",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_user",
          "value" : "rman"
        }, {
          "name" : "headlamp_heapsize",
          "value" : "580911104"
        } ]
      }, {
        "roleType" : "SERVICEMONITOR",
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "580911104"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "805306368"
        } ]
      } ],
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ALERTPUBLISHER-ddb686fe5b3727b404abc759eeb81b32",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "i-038c81a93875d91cc"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "5ptmb0dz4jqmkv0cmddk0u75f"
        } ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-ddb686fe5b3727b404abc759eeb81b32",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "i-038c81a93875d91cc"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "ch65bjit0vbytmlhvkxq7ojqf"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-ddb686fe5b3727b404abc759eeb81b32",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "i-038c81a93875d91cc"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "9dyyky2hukmq8l7eh57njo3o2"
        } ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-ddb686fe5b3727b404abc759eeb81b32",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "i-038c81a93875d91cc"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "93l3s9r4z9paipot80mwdmt0u"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-ddb686fe5b3727b404abc759eeb81b32",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "i-038c81a93875d91cc"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "5oze0v5rbx972k7fi1i0hc4v4"
        } ]
      }
    } ],
    "displayName" : "Cloudera Management Service"
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/25/2012 2:10"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/"
    } ]
  }
}[root@ip-172-31-38-243 ~]#

```