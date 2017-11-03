The full teragen command and output
The time command output
```
[reilly@ip-172-31-38-243 ~]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples-2.6.0-cdh5.8.5.jar teragen -Dmapreduce.job.maps=12 -D dfs.block.size=33554432 -Dmapreduce.map.memory.mb=1024 65536000 /user/reilly/tgen
17/11/03 08:49:14 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-33-170.us-west-2.compute.internal/172.31.33.170:8032
17/11/03 08:49:15 INFO terasort.TeraSort: Generating 65536000 using 12
17/11/03 08:49:15 INFO mapreduce.JobSubmitter: number of splits:12
17/11/03 08:49:15 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/11/03 08:49:15 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1509697170737_0001
17/11/03 08:49:15 INFO impl.YarnClientImpl: Submitted application application_1509697170737_0001
17/11/03 08:49:16 INFO mapreduce.Job: The url to track the job: http://ip-172-31-33-170.us-west-2.compute.internal:8088/proxy/application_1509697170737_0001/
17/11/03 08:49:16 INFO mapreduce.Job: Running job: job_1509697170737_0001
17/11/03 08:49:23 INFO mapreduce.Job: Job job_1509697170737_0001 running in uber mode : false
17/11/03 08:49:23 INFO mapreduce.Job:  map 0% reduce 0%
17/11/03 08:49:38 INFO mapreduce.Job:  map 7% reduce 0%
17/11/03 08:49:39 INFO mapreduce.Job:  map 19% reduce 0%
17/11/03 08:49:41 INFO mapreduce.Job:  map 23% reduce 0%
17/11/03 08:49:42 INFO mapreduce.Job:  map 29% reduce 0%
17/11/03 08:49:44 INFO mapreduce.Job:  map 31% reduce 0%
17/11/03 08:49:45 INFO mapreduce.Job:  map 34% reduce 0%
17/11/03 08:49:47 INFO mapreduce.Job:  map 37% reduce 0%
17/11/03 08:49:48 INFO mapreduce.Job:  map 39% reduce 0%
17/11/03 08:49:51 INFO mapreduce.Job:  map 42% reduce 0%
17/11/03 08:49:52 INFO mapreduce.Job:  map 44% reduce 0%
17/11/03 08:49:54 INFO mapreduce.Job:  map 47% reduce 0%
17/11/03 08:49:55 INFO mapreduce.Job:  map 49% reduce 0%
17/11/03 08:49:57 INFO mapreduce.Job:  map 52% reduce 0%
17/11/03 08:50:00 INFO mapreduce.Job:  map 53% reduce 0%
17/11/03 08:50:06 INFO mapreduce.Job:  map 54% reduce 0%
17/11/03 08:50:07 INFO mapreduce.Job:  map 56% reduce 0%
17/11/03 08:50:09 INFO mapreduce.Job:  map 57% reduce 0%
17/11/03 08:50:12 INFO mapreduce.Job:  map 61% reduce 0%
17/11/03 08:50:13 INFO mapreduce.Job:  map 63% reduce 0%
17/11/03 08:50:15 INFO mapreduce.Job:  map 66% reduce 0%
17/11/03 08:50:16 INFO mapreduce.Job:  map 68% reduce 0%
17/11/03 08:50:18 INFO mapreduce.Job:  map 69% reduce 0%
17/11/03 08:50:21 INFO mapreduce.Job:  map 72% reduce 0%
17/11/03 08:50:24 INFO mapreduce.Job:  map 74% reduce 0%
17/11/03 08:50:27 INFO mapreduce.Job:  map 77% reduce 0%
17/11/03 08:50:30 INFO mapreduce.Job:  map 79% reduce 0%
17/11/03 08:50:33 INFO mapreduce.Job:  map 82% reduce 0%
17/11/03 08:50:36 INFO mapreduce.Job:  map 85% reduce 0%
17/11/03 08:50:41 INFO mapreduce.Job:  map 86% reduce 0%
17/11/03 08:50:43 INFO mapreduce.Job:  map 89% reduce 0%
17/11/03 08:50:46 INFO mapreduce.Job:  map 93% reduce 0%
17/11/03 08:50:49 INFO mapreduce.Job:  map 98% reduce 0%
17/11/03 08:50:50 INFO mapreduce.Job:  map 99% reduce 0%
17/11/03 08:50:51 INFO mapreduce.Job:  map 100% reduce 0%
17/11/03 08:50:51 INFO mapreduce.Job: Job job_1509697170737_0001 completed successfully
17/11/03 08:50:51 INFO mapreduce.Job: Counters: 31
        File System Counters
                FILE: Number of bytes read=0
                FILE: Number of bytes written=1476278
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=1025
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=48
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=24
        Job Counters
                Launched map tasks=12
                Other local map tasks=12
                Total time spent by all maps in occupied slots (ms)=914124
                Total time spent by all reduces in occupied slots (ms)=0
                Total time spent by all map tasks (ms)=914124
                Total vcore-seconds taken by all map tasks=914124
                Total megabyte-seconds taken by all map tasks=936062976
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Input split bytes=1025
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=2655
                CPU time spent (ms)=154340
                Physical memory (bytes) snapshot=4318068736
                Virtual memory (bytes) snapshot=18736160768
                Total committed heap usage (bytes)=4719116288
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=140750829423462787
        File Input Format Counters
                Bytes Read=0
        File Output Format Counters
                Bytes Written=6553600000

real    1m40.103s
user    0m6.077s
sys     0m0.821s
[reilly@ip-172-31-38-243 ~]$
```
The command and output of hdfs dfs -ls /user/reilly/tgen
```
[reilly@ip-172-31-38-243 ~]$ hdfs dfs -ls /user/reilly/tgen
Found 13 items
-rw-r--r--   3 reilly sanfrancisco          0 2017-11-03 08:50 /user/reilly/tgen/_SUCCESS
-rw-r--r--   3 reilly sanfrancisco  546133400 2017-11-03 08:50 /user/reilly/tgen/part-m-00000
-rw-r--r--   3 reilly sanfrancisco  546133300 2017-11-03 08:50 /user/reilly/tgen/part-m-00001
-rw-r--r--   3 reilly sanfrancisco  546133300 2017-11-03 08:50 /user/reilly/tgen/part-m-00002
-rw-r--r--   3 reilly sanfrancisco  546133400 2017-11-03 08:50 /user/reilly/tgen/part-m-00003
-rw-r--r--   3 reilly sanfrancisco  546133300 2017-11-03 08:50 /user/reilly/tgen/part-m-00004
-rw-r--r--   3 reilly sanfrancisco  546133300 2017-11-03 08:50 /user/reilly/tgen/part-m-00005
-rw-r--r--   3 reilly sanfrancisco  546133400 2017-11-03 08:50 /user/reilly/tgen/part-m-00006
-rw-r--r--   3 reilly sanfrancisco  546133300 2017-11-03 08:50 /user/reilly/tgen/part-m-00007
-rw-r--r--   3 reilly sanfrancisco  546133300 2017-11-03 08:50 /user/reilly/tgen/part-m-00008
-rw-r--r--   3 reilly sanfrancisco  546133400 2017-11-03 08:50 /user/reilly/tgen/part-m-00009
-rw-r--r--   3 reilly sanfrancisco  546133300 2017-11-03 08:50 /user/reilly/tgen/part-m-00010
-rw-r--r--   3 reilly sanfrancisco  546133300 2017-11-03 08:50 /user/reilly/tgen/part-m-00011
[reilly@ip-172-31-38-243 ~]$

```
The command and output of hadoop fsck -blocks /user/reilly/tgen
```
[reilly@ip-172-31-38-243 ~]$ hadoop fsck -blocks /user/reilly/tgen
DEPRECATED: Use of this script to execute hdfs command is deprecated.
Instead use the hdfs command for it.

Connecting to namenode via http://ip-172-31-33-170.us-west-2.compute.internal:50070
FSCK started by reilly (auth:SIMPLE) from /172.31.38.243 for path /user/reilly/tgen at Fri Nov 03 08:53:15 UTC 2017
.............Status: HEALTHY
 Total size:    6553600000 B
 Total dirs:    1
 Total files:   13
 Total symlinks:                0
 Total blocks (validated):      204 (avg. block size 32125490 B)
 Minimally replicated blocks:   204 (100.0 %)
 Over-replicated blocks:        0 (0.0 %)
 Under-replicated blocks:       0 (0.0 %)
 Mis-replicated blocks:         0 (0.0 %)
 Default replication factor:    3
 Average block replication:     3.0
 Corrupt blocks:                0
 Missing replicas:              0 (0.0 %)
 Number of data-nodes:          4
 Number of racks:               1
FSCK ended at Fri Nov 03 08:53:15 UTC 2017 in 12 milliseconds


The filesystem under path '/user/reilly/tgen' is HEALTHY
[reilly@ip-172-31-38-243 ~]$
```