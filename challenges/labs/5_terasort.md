Run the terasort program as user reilly with the output target /user/reilly/tsort
```
[root@ip-172-31-38-243 ~]# time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples-2.6.0-cdh5.8.5.jar terasort /user/reilly/tgen /user/reilly/tsort
17/11/03 09:56:49 INFO terasort.TeraSort: starting
17/11/03 09:56:51 INFO hdfs.DFSClient: Created token for reilly: HDFS_DELEGATION_TOKEN owner=reilly@NithK45.FNG, renewer=yarn, realUser=, issueDate=1509703011159, maxDate=1510307811159, sequenceNumber=1, masterKeyId=2 on 172.31.33.170:8020
17/11/03 09:56:51 INFO security.TokenCache: Got dt for hdfs://ip-172-31-33-170.us-west-2.compute.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.33.170:8020, Ident: (token for reilly: HDFS_DELEGATION_TOKEN owner=reilly@NithK45.FNG, renewer=yarn, realUser=, issueDate=1509703011159, maxDate=1510307811159, sequenceNumber=1, masterKeyId=2)
17/11/03 09:56:51 INFO input.FileInputFormat: Total input paths to process : 12
Spent 457ms computing base-splits.
Spent 5ms computing TeraScheduler splits.
Computing input splits took 463ms
Sampling 10 splits of 204
Making 8 from 100000 sampled records
Computing parititions took 1640ms
Spent 2106ms computing partitions.
17/11/03 09:56:53 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-33-170.us-west-2.compute.internal/172.31.33.170:8032
17/11/03 09:56:53 INFO mapreduce.JobSubmitter: number of splits:204
17/11/03 09:56:53 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1509702562193_0001
17/11/03 09:56:53 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.33.170:8020, Ident: (token for reilly: HDFS_DELEGATION_TOKEN owner=reilly@NithK45.FNG, renewer=yarn, realUser=, issueDate=1509703011159, maxDate=1510307811159, sequenceNumber=1, masterKeyId=2)
17/11/03 09:56:54 INFO impl.YarnClientImpl: Submitted application application_1509702562193_0001
17/11/03 09:56:54 INFO mapreduce.Job: The url to track the job: http://ip-172-31-33-170.us-west-2.compute.internal:8088/proxy/application_1509702562193_0001/
17/11/03 09:56:54 INFO mapreduce.Job: Running job: job_1509702562193_0001
17/11/03 09:57:05 INFO mapreduce.Job: Job job_1509702562193_0001 running in uber mode : false
17/11/03 09:57:05 INFO mapreduce.Job:  map 0% reduce 0%
17/11/03 09:57:17 INFO mapreduce.Job:  map 1% reduce 0%
17/11/03 09:57:26 INFO mapreduce.Job:  map 4% reduce 0%
17/11/03 09:57:27 INFO mapreduce.Job:  map 8% reduce 0%
17/11/03 09:57:28 INFO mapreduce.Job:  map 9% reduce 0%
17/11/03 09:57:38 INFO mapreduce.Job:  map 10% reduce 0%
17/11/03 09:57:40 INFO mapreduce.Job:  map 15% reduce 0%
17/11/03 09:57:41 INFO mapreduce.Job:  map 16% reduce 0%
17/11/03 09:57:47 INFO mapreduce.Job:  map 17% reduce 0%
17/11/03 09:57:49 INFO mapreduce.Job:  map 18% reduce 0%
17/11/03 09:57:53 INFO mapreduce.Job:  map 20% reduce 0%
17/11/03 09:57:54 INFO mapreduce.Job:  map 22% reduce 0%
17/11/03 09:57:55 INFO mapreduce.Job:  map 24% reduce 0%
17/11/03 09:57:58 INFO mapreduce.Job:  map 25% reduce 0%
17/11/03 09:58:05 INFO mapreduce.Job:  map 26% reduce 0%
17/11/03 09:58:06 INFO mapreduce.Job:  map 28% reduce 0%
17/11/03 09:58:08 INFO mapreduce.Job:  map 31% reduce 0%
17/11/03 09:58:09 INFO mapreduce.Job:  map 32% reduce 0%
17/11/03 09:58:17 INFO mapreduce.Job:  map 33% reduce 0%
17/11/03 09:58:18 INFO mapreduce.Job:  map 35% reduce 0%
17/11/03 09:58:19 INFO mapreduce.Job:  map 36% reduce 0%
17/11/03 09:58:20 INFO mapreduce.Job:  map 37% reduce 0%
17/11/03 09:58:21 INFO mapreduce.Job:  map 38% reduce 0%
17/11/03 09:58:22 INFO mapreduce.Job:  map 40% reduce 0%
17/11/03 09:58:28 INFO mapreduce.Job:  map 41% reduce 0%
17/11/03 09:58:31 INFO mapreduce.Job:  map 42% reduce 0%
17/11/03 09:58:32 INFO mapreduce.Job:  map 44% reduce 0%
17/11/03 09:58:34 INFO mapreduce.Job:  map 45% reduce 0%
17/11/03 09:58:36 INFO mapreduce.Job:  map 48% reduce 0%
17/11/03 09:58:39 INFO mapreduce.Job:  map 49% reduce 0%
17/11/03 09:58:44 INFO mapreduce.Job:  map 50% reduce 0%
17/11/03 09:58:45 INFO mapreduce.Job:  map 51% reduce 0%
17/11/03 09:58:47 INFO mapreduce.Job:  map 53% reduce 0%
17/11/03 09:58:49 INFO mapreduce.Job:  map 56% reduce 0%
17/11/03 09:58:57 INFO mapreduce.Job:  map 57% reduce 0%
17/11/03 09:58:58 INFO mapreduce.Job:  map 58% reduce 0%
17/11/03 09:58:59 INFO mapreduce.Job:  map 60% reduce 0%
17/11/03 09:59:00 INFO mapreduce.Job:  map 61% reduce 0%
17/11/03 09:59:04 INFO mapreduce.Job:  map 63% reduce 0%
17/11/03 09:59:05 INFO mapreduce.Job:  map 64% reduce 0%
17/11/03 09:59:09 INFO mapreduce.Job:  map 65% reduce 0%
17/11/03 09:59:10 INFO mapreduce.Job:  map 66% reduce 0%
17/11/03 09:59:11 INFO mapreduce.Job:  map 67% reduce 0%
17/11/03 09:59:13 INFO mapreduce.Job:  map 68% reduce 0%
17/11/03 09:59:14 INFO mapreduce.Job:  map 69% reduce 0%
17/11/03 09:59:17 INFO mapreduce.Job:  map 70% reduce 0%
17/11/03 09:59:18 INFO mapreduce.Job:  map 71% reduce 0%
17/11/03 09:59:19 INFO mapreduce.Job:  map 72% reduce 0%
17/11/03 09:59:22 INFO mapreduce.Job:  map 73% reduce 0%
17/11/03 09:59:24 INFO mapreduce.Job:  map 75% reduce 0%
17/11/03 09:59:26 INFO mapreduce.Job:  map 76% reduce 0%
17/11/03 09:59:29 INFO mapreduce.Job:  map 78% reduce 0%
17/11/03 09:59:31 INFO mapreduce.Job:  map 79% reduce 0%
17/11/03 09:59:34 INFO mapreduce.Job:  map 80% reduce 0%
17/11/03 09:59:35 INFO mapreduce.Job:  map 81% reduce 0%
17/11/03 09:59:37 INFO mapreduce.Job:  map 82% reduce 0%
17/11/03 09:59:38 INFO mapreduce.Job:  map 83% reduce 0%
17/11/03 09:59:40 INFO mapreduce.Job:  map 85% reduce 0%
17/11/03 09:59:43 INFO mapreduce.Job:  map 86% reduce 0%
17/11/03 09:59:44 INFO mapreduce.Job:  map 87% reduce 0%
17/11/03 09:59:46 INFO mapreduce.Job:  map 88% reduce 0%
17/11/03 09:59:49 INFO mapreduce.Job:  map 88% reduce 3%
17/11/03 09:59:51 INFO mapreduce.Job:  map 88% reduce 5%
17/11/03 09:59:52 INFO mapreduce.Job:  map 88% reduce 15%
17/11/03 09:59:53 INFO mapreduce.Job:  map 89% reduce 15%
17/11/03 09:59:54 INFO mapreduce.Job:  map 89% reduce 19%
17/11/03 09:59:55 INFO mapreduce.Job:  map 89% reduce 20%
17/11/03 09:59:56 INFO mapreduce.Job:  map 90% reduce 21%
17/11/03 09:59:58 INFO mapreduce.Job:  map 91% reduce 25%
17/11/03 09:59:59 INFO mapreduce.Job:  map 92% reduce 25%
17/11/03 10:00:00 INFO mapreduce.Job:  map 92% reduce 27%
17/11/03 10:00:05 INFO mapreduce.Job:  map 93% reduce 27%
17/11/03 10:00:07 INFO mapreduce.Job:  map 94% reduce 27%
17/11/03 10:00:10 INFO mapreduce.Job:  map 96% reduce 28%
17/11/03 10:00:13 INFO mapreduce.Job:  map 97% reduce 28%
17/11/03 10:00:15 INFO mapreduce.Job:  map 98% reduce 28%
17/11/03 10:00:21 INFO mapreduce.Job:  map 99% reduce 28%
17/11/03 10:00:22 INFO mapreduce.Job:  map 99% reduce 29%
17/11/03 10:00:23 INFO mapreduce.Job:  map 100% reduce 29%
17/11/03 10:00:24 INFO mapreduce.Job:  map 100% reduce 33%
17/11/03 10:00:25 INFO mapreduce.Job:  map 100% reduce 45%
17/11/03 10:00:26 INFO mapreduce.Job:  map 100% reduce 53%
17/11/03 10:00:27 INFO mapreduce.Job:  map 100% reduce 57%
17/11/03 10:00:28 INFO mapreduce.Job:  map 100% reduce 63%
17/11/03 10:00:30 INFO mapreduce.Job:  map 100% reduce 66%
17/11/03 10:00:31 INFO mapreduce.Job:  map 100% reduce 69%
17/11/03 10:00:32 INFO mapreduce.Job:  map 100% reduce 70%
17/11/03 10:00:33 INFO mapreduce.Job:  map 100% reduce 72%
17/11/03 10:00:34 INFO mapreduce.Job:  map 100% reduce 75%
17/11/03 10:00:35 INFO mapreduce.Job:  map 100% reduce 76%
17/11/03 10:00:36 INFO mapreduce.Job:  map 100% reduce 77%
17/11/03 10:00:37 INFO mapreduce.Job:  map 100% reduce 79%
17/11/03 10:00:38 INFO mapreduce.Job:  map 100% reduce 80%
17/11/03 10:00:39 INFO mapreduce.Job:  map 100% reduce 81%
17/11/03 10:00:40 INFO mapreduce.Job:  map 100% reduce 84%
17/11/03 10:00:41 INFO mapreduce.Job:  map 100% reduce 86%
17/11/03 10:00:42 INFO mapreduce.Job:  map 100% reduce 87%
17/11/03 10:00:43 INFO mapreduce.Job:  map 100% reduce 88%
17/11/03 10:00:44 INFO mapreduce.Job:  map 100% reduce 90%
17/11/03 10:00:47 INFO mapreduce.Job:  map 100% reduce 93%
17/11/03 10:00:50 INFO mapreduce.Job:  map 100% reduce 95%
17/11/03 10:00:51 INFO mapreduce.Job:  map 100% reduce 96%
17/11/03 10:00:52 INFO mapreduce.Job:  map 100% reduce 97%
17/11/03 10:00:54 INFO mapreduce.Job:  map 100% reduce 98%
17/11/03 10:01:00 INFO mapreduce.Job:  map 100% reduce 99%
17/11/03 10:01:06 INFO mapreduce.Job:  map 100% reduce 100%
17/11/03 10:01:17 INFO mapreduce.Job: Job job_1509702562193_0001 completed successfully
17/11/03 10:01:18 INFO mapreduce.Job: Counters: 50
        File System Counters
                FILE: Number of bytes read=2931178508
                FILE: Number of bytes written=5825121351
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=6553630600
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=636
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=16
        Job Counters
                Launched map tasks=204
                Launched reduce tasks=8
                Data-local map tasks=203
                Rack-local map tasks=1
                Total time spent by all maps in occupied slots (ms)=2380550
                Total time spent by all reduces in occupied slots (ms)=598420
                Total time spent by all map tasks (ms)=2380550
                Total time spent by all reduce tasks (ms)=598420
                Total vcore-seconds taken by all map tasks=2380550
                Total vcore-seconds taken by all reduce tasks=598420
                Total megabyte-seconds taken by all map tasks=2437683200
                Total megabyte-seconds taken by all reduce tasks=612782080
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Map output bytes=6684672000
                Map output materialized bytes=2867385837
                Input split bytes=30600
                Combine input records=0
                Combine output records=0
                Reduce input groups=65536000
                Reduce shuffle bytes=2867385837
                Reduce input records=65536000
                Reduce output records=65536000
                Spilled Records=131072000
                Shuffled Maps =1632
                Failed Shuffles=0
                Merged Map outputs=1632
                GC time elapsed (ms)=31931
                CPU time spent (ms)=1084830
                Physical memory (bytes) snapshot=102480211968
                Virtual memory (bytes) snapshot=331357147136
                Total committed heap usage (bytes)=119858003968
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=6553600000
        File Output Format Counters
                Bytes Written=6553600000
17/11/03 10:01:18 INFO terasort.TeraSort: done

real    4m29.856s
user    0m8.738s
sys     0m0.983s
[root@ip-172-31-38-243 ~]#

```