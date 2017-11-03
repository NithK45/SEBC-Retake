```
[root@ip-172-31-42-120 ~]# time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples-2.6.0-cdh5.8.5.jar pi 50 100
Number of Maps  = 50
Samples per Map = 100
Wrote input for Map #0
Wrote input for Map #1
Wrote input for Map #2
Wrote input for Map #3
Wrote input for Map #4
Wrote input for Map #5
Wrote input for Map #6
Wrote input for Map #7
Wrote input for Map #8
Wrote input for Map #9
Wrote input for Map #10
Wrote input for Map #11
Wrote input for Map #12
Wrote input for Map #13
Wrote input for Map #14
Wrote input for Map #15
Wrote input for Map #16
Wrote input for Map #17
Wrote input for Map #18
Wrote input for Map #19
Wrote input for Map #20
Wrote input for Map #21
Wrote input for Map #22
Wrote input for Map #23
Wrote input for Map #24
Wrote input for Map #25
Wrote input for Map #26
Wrote input for Map #27
Wrote input for Map #28
Wrote input for Map #29
Wrote input for Map #30
Wrote input for Map #31
Wrote input for Map #32
Wrote input for Map #33
Wrote input for Map #34
Wrote input for Map #35
Wrote input for Map #36
Wrote input for Map #37
Wrote input for Map #38
Wrote input for Map #39
Wrote input for Map #40
Wrote input for Map #41
Wrote input for Map #42
Wrote input for Map #43
Wrote input for Map #44
Wrote input for Map #45
Wrote input for Map #46
Wrote input for Map #47
Wrote input for Map #48
Wrote input for Map #49
Starting Job
17/11/03 10:09:14 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-33-170.us-west-2.compute.internal/172.31.33.170:8032
17/11/03 10:09:14 INFO hdfs.DFSClient: Created token for frankola: HDFS_DELEGATION_TOKEN owner=frankola@NithK45.FNG, renewer=yarn, realUser=, issueDate=1509703754813, maxDate=1510308554813, sequenceNumber=2, masterKeyId=2 on 172.31.33.170:8020
17/11/03 10:09:14 INFO security.TokenCache: Got dt for hdfs://ip-172-31-33-170.us-west-2.compute.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.33.170:8020, Ident: (token for frankola: HDFS_DELEGATION_TOKEN owner=frankola@NithK45.FNG, renewer=yarn, realUser=, issueDate=1509703754813, maxDate=1510308554813, sequenceNumber=2, masterKeyId=2)
17/11/03 10:09:15 INFO input.FileInputFormat: Total input paths to process : 50
17/11/03 10:09:15 INFO mapreduce.JobSubmitter: number of splits:50
17/11/03 10:09:15 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1509702562193_0002
17/11/03 10:09:15 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.33.170:8020, Ident: (token for frankola: HDFS_DELEGATION_TOKEN owner=frankola@NithK45.FNG, renewer=yarn, realUser=, issueDate=1509703754813, maxDate=1510308554813, sequenceNumber=2, masterKeyId=2)
17/11/03 10:09:15 INFO impl.YarnClientImpl: Submitted application application_1509702562193_0002
17/11/03 10:09:15 INFO mapreduce.Job: The url to track the job: http://ip-172-31-33-170.us-west-2.compute.internal:8088/proxy/application_1509702562193_0002/
17/11/03 10:09:15 INFO mapreduce.Job: Running job: job_1509702562193_0002
17/11/03 10:09:25 INFO mapreduce.Job: Job job_1509702562193_0002 running in uber mode : false
17/11/03 10:09:25 INFO mapreduce.Job:  map 0% reduce 0%
17/11/03 10:09:35 INFO mapreduce.Job:  map 6% reduce 0%
17/11/03 10:09:42 INFO mapreduce.Job:  map 14% reduce 0%
17/11/03 10:09:43 INFO mapreduce.Job:  map 36% reduce 0%
17/11/03 10:09:48 INFO mapreduce.Job:  map 38% reduce 0%
17/11/03 10:09:50 INFO mapreduce.Job:  map 40% reduce 0%
17/11/03 10:09:51 INFO mapreduce.Job:  map 42% reduce 0%
17/11/03 10:09:52 INFO mapreduce.Job:  map 50% reduce 0%
17/11/03 10:09:53 INFO mapreduce.Job:  map 60% reduce 0%
17/11/03 10:09:54 INFO mapreduce.Job:  map 66% reduce 0%
17/11/03 10:09:55 INFO mapreduce.Job:  map 68% reduce 0%
17/11/03 10:09:58 INFO mapreduce.Job:  map 72% reduce 0%
17/11/03 10:10:01 INFO mapreduce.Job:  map 74% reduce 0%
17/11/03 10:10:02 INFO mapreduce.Job:  map 82% reduce 0%
17/11/03 10:10:03 INFO mapreduce.Job:  map 94% reduce 0%
17/11/03 10:10:04 INFO mapreduce.Job:  map 100% reduce 0%
17/11/03 10:10:09 INFO mapreduce.Job:  map 100% reduce 100%
17/11/03 10:10:09 INFO mapreduce.Job: Job job_1509702562193_0002 completed successfully
17/11/03 10:10:09 INFO mapreduce.Job: Counters: 49
        File System Counters
                FILE: Number of bytes read=259
                FILE: Number of bytes written=6350577
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=15140
                HDFS: Number of bytes written=215
                HDFS: Number of read operations=203
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=3
        Job Counters
                Launched map tasks=50
                Launched reduce tasks=1
                Data-local map tasks=50
                Total time spent by all maps in occupied slots (ms)=490081
                Total time spent by all reduces in occupied slots (ms)=4053
                Total time spent by all map tasks (ms)=490081
                Total time spent by all reduce tasks (ms)=4053
                Total vcore-seconds taken by all map tasks=490081
                Total vcore-seconds taken by all reduce tasks=4053
                Total megabyte-seconds taken by all map tasks=501842944
                Total megabyte-seconds taken by all reduce tasks=4150272
        Map-Reduce Framework
                Map input records=50
                Map output records=100
                Map output bytes=900
                Map output materialized bytes=1700
                Input split bytes=9240
                Combine input records=0
                Combine output records=0
                Reduce input groups=2
                Reduce shuffle bytes=1700
                Reduce input records=100
                Reduce output records=0
                Spilled Records=200
                Shuffled Maps =50
                Failed Shuffles=0
                Merged Map outputs=50
                GC time elapsed (ms)=2829
                CPU time spent (ms)=47110
                Physical memory (bytes) snapshot=22714544128
                Virtual memory (bytes) snapshot=79670018048
                Total committed heap usage (bytes)=26104299520
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=5900
        File Output Format Counters
                Bytes Written=97
Job Finished in 55.223 seconds
Estimated value of Pi is 3.14160000000000000000

real    0m59.678s
user    0m6.146s
sys     0m0.822s
[root@ip-172-31-42-120 ~]#
```