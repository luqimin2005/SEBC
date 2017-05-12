Copy the command and full output
```
[root@ip-172-31-38-5 ~]# su - chen
[chen@ip-172-31-38-5 ~]$ 
[chen@ip-172-31-38-5 ~]$ kinit 
Password for chen@LUQIMIN2005.CN: 
[chen@ip-172-31-38-5 ~]$ 
[chen@ip-172-31-38-5 ~]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar pi 100 100000000
Number of Maps  = 100
Samples per Map = 100000000
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
Wrote input for Map #50
Wrote input for Map #51
Wrote input for Map #52
Wrote input for Map #53
Wrote input for Map #54
Wrote input for Map #55
Wrote input for Map #56
Wrote input for Map #57
Wrote input for Map #58
Wrote input for Map #59
Wrote input for Map #60
Wrote input for Map #61
Wrote input for Map #62
Wrote input for Map #63
Wrote input for Map #64
Wrote input for Map #65
Wrote input for Map #66
Wrote input for Map #67
Wrote input for Map #68
Wrote input for Map #69
Wrote input for Map #70
Wrote input for Map #71
Wrote input for Map #72
Wrote input for Map #73
Wrote input for Map #74
Wrote input for Map #75
Wrote input for Map #76
Wrote input for Map #77
Wrote input for Map #78
Wrote input for Map #79
Wrote input for Map #80
Wrote input for Map #81
Wrote input for Map #82
Wrote input for Map #83
Wrote input for Map #84
Wrote input for Map #85
Wrote input for Map #86
Wrote input for Map #87
Wrote input for Map #88
Wrote input for Map #89
Wrote input for Map #90
Wrote input for Map #91
Wrote input for Map #92
Wrote input for Map #93
Wrote input for Map #94
Wrote input for Map #95
Wrote input for Map #96
Wrote input for Map #97
Wrote input for Map #98
Wrote input for Map #99
Starting Job
17/05/12 02:59:36 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-41-1/172.31.41.1:8032
17/05/12 02:59:36 INFO hdfs.DFSClient: Created token for chen: HDFS_DELEGATION_TOKEN owner=chen@LUQIMIN2005.CN, renewer=yarn, realUser=, issueDate=1494557976651, maxDate=1495162776651, sequenceNumber=2, masterKeyId=2 on 172.31.41.1:8020
17/05/12 02:59:36 INFO security.TokenCache: Got dt for hdfs://ip-172-31-41-1:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.41.1:8020, Ident: (token for chen: HDFS_DELEGATION_TOKEN owner=chen@LUQIMIN2005.CN, renewer=yarn, realUser=, issueDate=1494557976651, maxDate=1495162776651, sequenceNumber=2, masterKeyId=2)
17/05/12 02:59:36 INFO input.FileInputFormat: Total input paths to process : 100
17/05/12 02:59:36 INFO mapreduce.JobSubmitter: number of splits:100
17/05/12 02:59:37 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1494557406271_0002
17/05/12 02:59:37 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.41.1:8020, Ident: (token for chen: HDFS_DELEGATION_TOKEN owner=chen@LUQIMIN2005.CN, renewer=yarn, realUser=, issueDate=1494557976651, maxDate=1495162776651, sequenceNumber=2, masterKeyId=2)
17/05/12 02:59:37 INFO impl.YarnClientImpl: Submitted application application_1494557406271_0002
17/05/12 02:59:37 INFO mapreduce.Job: The url to track the job: http://ip-172-31-41-1:8088/proxy/application_1494557406271_0002/
17/05/12 02:59:37 INFO mapreduce.Job: Running job: job_1494557406271_0002
17/05/12 02:59:46 INFO mapreduce.Job: Job job_1494557406271_0002 running in uber mode : false
17/05/12 02:59:46 INFO mapreduce.Job:  map 0% reduce 0%
17/05/12 02:59:54 INFO mapreduce.Job:  map 1% reduce 0%
17/05/12 02:59:56 INFO mapreduce.Job:  map 2% reduce 0%
17/05/12 02:59:57 INFO mapreduce.Job:  map 5% reduce 0%
17/05/12 03:00:01 INFO mapreduce.Job:  map 6% reduce 0%
17/05/12 03:00:03 INFO mapreduce.Job:  map 7% reduce 0%
17/05/12 03:00:04 INFO mapreduce.Job:  map 8% reduce 0%
17/05/12 03:00:05 INFO mapreduce.Job:  map 10% reduce 0%
17/05/12 03:00:08 INFO mapreduce.Job:  map 11% reduce 0%
17/05/12 03:00:11 INFO mapreduce.Job:  map 13% reduce 0%
17/05/12 03:00:13 INFO mapreduce.Job:  map 15% reduce 0%
17/05/12 03:00:15 INFO mapreduce.Job:  map 16% reduce 0%
17/05/12 03:00:18 INFO mapreduce.Job:  map 18% reduce 0%
17/05/12 03:00:20 INFO mapreduce.Job:  map 20% reduce 0%
17/05/12 03:00:23 INFO mapreduce.Job:  map 21% reduce 0%
17/05/12 03:00:25 INFO mapreduce.Job:  map 22% reduce 0%
17/05/12 03:00:26 INFO mapreduce.Job:  map 23% reduce 0%
17/05/12 03:00:27 INFO mapreduce.Job:  map 25% reduce 0%
17/05/12 03:00:30 INFO mapreduce.Job:  map 26% reduce 0%
17/05/12 03:00:32 INFO mapreduce.Job:  map 28% reduce 0%
17/05/12 03:00:34 INFO mapreduce.Job:  map 30% reduce 0%
17/05/12 03:00:37 INFO mapreduce.Job:  map 31% reduce 0%
17/05/12 03:00:39 INFO mapreduce.Job:  map 33% reduce 0%
17/05/12 03:00:41 INFO mapreduce.Job:  map 35% reduce 0%
17/05/12 03:00:43 INFO mapreduce.Job:  map 36% reduce 0%
17/05/12 03:00:46 INFO mapreduce.Job:  map 37% reduce 0%
17/05/12 03:00:47 INFO mapreduce.Job:  map 38% reduce 0%
17/05/12 03:00:48 INFO mapreduce.Job:  map 40% reduce 0%
17/05/12 03:00:51 INFO mapreduce.Job:  map 41% reduce 0%
17/05/12 03:00:53 INFO mapreduce.Job:  map 42% reduce 0%
17/05/12 03:00:54 INFO mapreduce.Job:  map 43% reduce 0%
17/05/12 03:00:55 INFO mapreduce.Job:  map 45% reduce 0%
17/05/12 03:00:58 INFO mapreduce.Job:  map 46% reduce 0%
17/05/12 03:01:00 INFO mapreduce.Job:  map 47% reduce 0%
17/05/12 03:01:01 INFO mapreduce.Job:  map 48% reduce 0%
17/05/12 03:01:02 INFO mapreduce.Job:  map 50% reduce 0%
17/05/12 03:01:04 INFO mapreduce.Job:  map 51% reduce 0%
17/05/12 03:01:07 INFO mapreduce.Job:  map 53% reduce 0%
17/05/12 03:01:09 INFO mapreduce.Job:  map 55% reduce 0%
17/05/12 03:01:11 INFO mapreduce.Job:  map 56% reduce 0%
17/05/12 03:01:14 INFO mapreduce.Job:  map 57% reduce 0%
17/05/12 03:01:15 INFO mapreduce.Job:  map 58% reduce 0%
17/05/12 03:01:16 INFO mapreduce.Job:  map 60% reduce 0%
17/05/12 03:01:18 INFO mapreduce.Job:  map 61% reduce 0%
17/05/12 03:01:21 INFO mapreduce.Job:  map 63% reduce 0%
17/05/12 03:01:23 INFO mapreduce.Job:  map 65% reduce 0%
17/05/12 03:01:26 INFO mapreduce.Job:  map 66% reduce 0%
17/05/12 03:01:28 INFO mapreduce.Job:  map 67% reduce 0%
17/05/12 03:01:29 INFO mapreduce.Job:  map 68% reduce 0%
17/05/12 03:01:30 INFO mapreduce.Job:  map 70% reduce 0%
17/05/12 03:01:33 INFO mapreduce.Job:  map 71% reduce 0%
17/05/12 03:01:35 INFO mapreduce.Job:  map 72% reduce 0%
17/05/12 03:01:36 INFO mapreduce.Job:  map 73% reduce 0%
17/05/12 03:01:37 INFO mapreduce.Job:  map 74% reduce 0%
17/05/12 03:01:38 INFO mapreduce.Job:  map 75% reduce 0%
17/05/12 03:01:39 INFO mapreduce.Job:  map 76% reduce 0%
17/05/12 03:01:42 INFO mapreduce.Job:  map 77% reduce 0%
17/05/12 03:01:43 INFO mapreduce.Job:  map 78% reduce 0%
17/05/12 03:01:44 INFO mapreduce.Job:  map 79% reduce 0%
17/05/12 03:01:45 INFO mapreduce.Job:  map 80% reduce 0%
17/05/12 03:01:46 INFO mapreduce.Job:  map 81% reduce 0%
17/05/12 03:01:49 INFO mapreduce.Job:  map 83% reduce 0%
17/05/12 03:01:51 INFO mapreduce.Job:  map 84% reduce 0%
17/05/12 03:01:52 INFO mapreduce.Job:  map 85% reduce 0%
17/05/12 03:01:53 INFO mapreduce.Job:  map 86% reduce 0%
17/05/12 03:01:56 INFO mapreduce.Job:  map 88% reduce 0%
17/05/12 03:01:58 INFO mapreduce.Job:  map 89% reduce 0%
17/05/12 03:01:59 INFO mapreduce.Job:  map 90% reduce 0%
17/05/12 03:02:03 INFO mapreduce.Job:  map 91% reduce 0%
17/05/12 03:02:04 INFO mapreduce.Job:  map 92% reduce 30%
17/05/12 03:02:05 INFO mapreduce.Job:  map 93% reduce 30%
17/05/12 03:02:06 INFO mapreduce.Job:  map 94% reduce 30%
17/05/12 03:02:07 INFO mapreduce.Job:  map 94% reduce 31%
17/05/12 03:02:10 INFO mapreduce.Job:  map 96% reduce 31%
17/05/12 03:02:11 INFO mapreduce.Job:  map 97% reduce 31%
17/05/12 03:02:13 INFO mapreduce.Job:  map 98% reduce 32%
17/05/12 03:02:16 INFO mapreduce.Job:  map 98% reduce 33%
17/05/12 03:02:17 INFO mapreduce.Job:  map 100% reduce 33%
17/05/12 03:02:18 INFO mapreduce.Job:  map 100% reduce 100%
17/05/12 03:02:19 INFO mapreduce.Job: Job job_1494557406271_0002 completed successfully
17/05/12 03:02:19 INFO mapreduce.Job: Counters: 50
	File System Counters
		FILE: Number of bytes read=865
		FILE: Number of bytes written=12497088
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=26990
		HDFS: Number of bytes written=215
		HDFS: Number of read operations=403
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=3
	Job Counters 
		Launched map tasks=100
		Launched reduce tasks=1
		Data-local map tasks=98
		Rack-local map tasks=2
		Total time spent by all maps in occupied slots (ms)=615029
		Total time spent by all reduces in occupied slots (ms)=24019
		Total time spent by all map tasks (ms)=615029
		Total time spent by all reduce tasks (ms)=24019
		Total vcore-seconds taken by all map tasks=615029
		Total vcore-seconds taken by all reduce tasks=24019
		Total megabyte-seconds taken by all map tasks=629789696
		Total megabyte-seconds taken by all reduce tasks=24595456
	Map-Reduce Framework
		Map input records=100
		Map output records=200
		Map output bytes=1800
		Map output materialized bytes=3700
		Input split bytes=15190
		Combine input records=0
		Combine output records=0
		Reduce input groups=2
		Reduce shuffle bytes=3700
		Reduce input records=200
		Reduce output records=0
		Spilled Records=400
		Shuffled Maps =100
		Failed Shuffles=0
		Merged Map outputs=100
		GC time elapsed (ms)=3909
		CPU time spent (ms)=306270
		Physical memory (bytes) snapshot=46130905088
		Virtual memory (bytes) snapshot=158212337664
		Total committed heap usage (bytes)=57026281472
	Shuffle Errors
		BAD_ID=0
		CONNECTION=0
		IO_ERROR=0
		WRONG_LENGTH=0
		WRONG_MAP=0
		WRONG_REDUCE=0
	File Input Format Counters 
		Bytes Read=11800
	File Output Format Counters 
		Bytes Written=97
Job Finished in 163.457 seconds
Estimated value of Pi is 3.14159264920000000000

real	2m48.838s
user	0m7.107s
sys	0m0.965s

```
