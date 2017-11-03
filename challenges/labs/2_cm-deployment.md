Copy the command and output to get your CM deployment to challenges/labs/2_cm-deployment.md

```
[root@ip-172-31-38-243 ~]# curl -u admin:admin 'http://ec2-52-32-156-77.us-west-2.compute.amazonaws.com:7180/api/v2/cm/deployment'
{
  "timestamp" : "2017-11-03T07:57:32.820Z",
  "clusters" : [ ],
  "hosts" : [ ],
  "users" : [ {
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