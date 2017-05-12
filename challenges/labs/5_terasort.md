Copy the command and full output 
```
[root@ip-172-31-38-5 ~]# su - zhou
[zhou@ip-172-31-38-5 ~]$ kinit 
Password for zhou@LUQIMIN2005.CN: 
[zhou@ip-172-31-38-5 ~]$ 
[zhou@ip-172-31-38-5 ~]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar terasort /user/zhou/tgen /user/zhou/tsort
17/05/12 02:53:56 INFO terasort.TeraSort: starting
17/05/12 02:53:58 INFO hdfs.DFSClient: Created token for zhou: HDFS_DELEGATION_TOKEN owner=zhou@LUQIMIN2005.CN, renewer=yarn, realUser=, issueDate=1494557638316, maxDate=1495162438316, sequenceNumber=1, masterKeyId=2 on 172.31.41.1:8020
17/05/12 02:53:58 INFO security.TokenCache: Got dt for hdfs://ip-172-31-41-1:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.41.1:8020, Ident: (token for zhou: HDFS_DELEGATION_TOKEN owner=zhou@LUQIMIN2005.CN, renewer=yarn, realUser=, issueDate=1494557638316, maxDate=1495162438316, sequenceNumber=1, masterKeyId=2)
17/05/12 02:53:58 INFO input.FileInputFormat: Total input paths to process : 6
Spent 374ms computing base-splits.
Spent 4ms computing TeraScheduler splits.
Computing input splits took 379ms
Sampling 10 splits of 102
Making 10 from 100000 sampled records
Computing parititions took 942ms
Spent 1324ms computing partitions.
17/05/12 02:53:59 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-41-1/172.31.41.1:8032
17/05/12 02:53:59 INFO mapreduce.JobSubmitter: number of splits:102
17/05/12 02:54:00 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1494557406271_0001
17/05/12 02:54:00 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.41.1:8020, Ident: (token for zhou: HDFS_DELEGATION_TOKEN owner=zhou@LUQIMIN2005.CN, renewer=yarn, realUser=, issueDate=1494557638316, maxDate=1495162438316, sequenceNumber=1, masterKeyId=2)
17/05/12 02:54:01 INFO impl.YarnClientImpl: Submitted application application_1494557406271_0001
17/05/12 02:54:01 INFO mapreduce.Job: The url to track the job: http://ip-172-31-41-1:8088/proxy/application_1494557406271_0001/
17/05/12 02:54:01 INFO mapreduce.Job: Running job: job_1494557406271_0001
17/05/12 02:54:11 INFO mapreduce.Job: Job job_1494557406271_0001 running in uber mode : false
17/05/12 02:54:11 INFO mapreduce.Job:  map 0% reduce 0%
17/05/12 02:54:24 INFO mapreduce.Job:  map 2% reduce 0%
17/05/12 02:54:27 INFO mapreduce.Job:  map 5% reduce 0%
17/05/12 02:54:30 INFO mapreduce.Job:  map 6% reduce 0%
17/05/12 02:54:32 INFO mapreduce.Job:  map 7% reduce 0%
17/05/12 02:54:35 INFO mapreduce.Job:  map 8% reduce 0%
17/05/12 02:54:37 INFO mapreduce.Job:  map 10% reduce 0%
17/05/12 02:54:38 INFO mapreduce.Job:  map 11% reduce 0%
17/05/12 02:54:40 INFO mapreduce.Job:  map 12% reduce 0%
17/05/12 02:54:43 INFO mapreduce.Job:  map 13% reduce 0%
17/05/12 02:54:44 INFO mapreduce.Job:  map 14% reduce 0%
17/05/12 02:54:46 INFO mapreduce.Job:  map 16% reduce 0%
17/05/12 02:54:48 INFO mapreduce.Job:  map 17% reduce 0%
17/05/12 02:54:51 INFO mapreduce.Job:  map 19% reduce 0%
17/05/12 02:54:56 INFO mapreduce.Job:  map 22% reduce 0%
17/05/12 02:54:58 INFO mapreduce.Job:  map 23% reduce 0%
17/05/12 02:54:59 INFO mapreduce.Job:  map 24% reduce 0%
17/05/12 02:55:04 INFO mapreduce.Job:  map 25% reduce 0%
17/05/12 02:55:05 INFO mapreduce.Job:  map 27% reduce 0%
17/05/12 02:55:07 INFO mapreduce.Job:  map 28% reduce 0%
17/05/12 02:55:12 INFO mapreduce.Job:  map 30% reduce 0%
17/05/12 02:55:14 INFO mapreduce.Job:  map 32% reduce 0%
17/05/12 02:55:15 INFO mapreduce.Job:  map 33% reduce 0%
17/05/12 02:55:19 INFO mapreduce.Job:  map 34% reduce 0%
17/05/12 02:55:20 INFO mapreduce.Job:  map 35% reduce 0%
17/05/12 02:55:23 INFO mapreduce.Job:  map 38% reduce 0%
17/05/12 02:55:26 INFO mapreduce.Job:  map 39% reduce 0%
17/05/12 02:55:28 INFO mapreduce.Job:  map 40% reduce 0%
17/05/12 02:55:31 INFO mapreduce.Job:  map 41% reduce 0%
17/05/12 02:55:32 INFO mapreduce.Job:  map 42% reduce 0%
17/05/12 02:55:33 INFO mapreduce.Job:  map 44% reduce 0%
17/05/12 02:55:37 INFO mapreduce.Job:  map 45% reduce 0%
17/05/12 02:55:40 INFO mapreduce.Job:  map 46% reduce 0%
17/05/12 02:55:41 INFO mapreduce.Job:  map 47% reduce 0%
17/05/12 02:55:42 INFO mapreduce.Job:  map 49% reduce 0%
17/05/12 02:55:45 INFO mapreduce.Job:  map 50% reduce 0%
17/05/12 02:55:48 INFO mapreduce.Job:  map 52% reduce 0%
17/05/12 02:55:51 INFO mapreduce.Job:  map 54% reduce 0%
17/05/12 02:55:53 INFO mapreduce.Job:  map 55% reduce 0%
17/05/12 02:55:55 INFO mapreduce.Job:  map 56% reduce 0%
17/05/12 02:55:56 INFO mapreduce.Job:  map 57% reduce 0%
17/05/12 02:56:01 INFO mapreduce.Job:  map 60% reduce 0%
17/05/12 02:56:02 INFO mapreduce.Job:  map 61% reduce 0%
17/05/12 02:56:04 INFO mapreduce.Job:  map 62% reduce 0%
17/05/12 02:56:09 INFO mapreduce.Job:  map 65% reduce 0%
17/05/12 02:56:10 INFO mapreduce.Job:  map 66% reduce 0%
17/05/12 02:56:12 INFO mapreduce.Job:  map 67% reduce 0%
17/05/12 02:56:16 INFO mapreduce.Job:  map 68% reduce 0%
17/05/12 02:56:17 INFO mapreduce.Job:  map 69% reduce 0%
17/05/12 02:56:18 INFO mapreduce.Job:  map 70% reduce 0%
17/05/12 02:56:19 INFO mapreduce.Job:  map 71% reduce 0%
17/05/12 02:56:20 INFO mapreduce.Job:  map 72% reduce 0%
17/05/12 02:56:23 INFO mapreduce.Job:  map 73% reduce 0%
17/05/12 02:56:25 INFO mapreduce.Job:  map 74% reduce 0%
17/05/12 02:56:27 INFO mapreduce.Job:  map 75% reduce 0%
17/05/12 02:56:28 INFO mapreduce.Job:  map 76% reduce 0%
17/05/12 02:56:30 INFO mapreduce.Job:  map 77% reduce 0%
17/05/12 02:56:32 INFO mapreduce.Job:  map 78% reduce 0%
17/05/12 02:56:36 INFO mapreduce.Job:  map 80% reduce 0%
17/05/12 02:56:37 INFO mapreduce.Job:  map 82% reduce 0%
17/05/12 02:56:41 INFO mapreduce.Job:  map 83% reduce 0%
17/05/12 02:56:44 INFO mapreduce.Job:  map 85% reduce 0%
17/05/12 02:56:45 INFO mapreduce.Job:  map 86% reduce 0%
17/05/12 02:56:46 INFO mapreduce.Job:  map 87% reduce 0%
17/05/12 02:56:49 INFO mapreduce.Job:  map 88% reduce 0%
17/05/12 02:56:52 INFO mapreduce.Job:  map 89% reduce 0%
17/05/12 02:56:54 INFO mapreduce.Job:  map 89% reduce 3%
17/05/12 02:56:56 INFO mapreduce.Job:  map 89% reduce 6%
17/05/12 02:56:57 INFO mapreduce.Job:  map 90% reduce 6%
17/05/12 02:56:58 INFO mapreduce.Job:  map 90% reduce 9%
17/05/12 02:57:00 INFO mapreduce.Job:  map 91% reduce 9%
17/05/12 02:57:03 INFO mapreduce.Job:  map 92% reduce 9%
17/05/12 02:57:08 INFO mapreduce.Job:  map 93% reduce 9%
17/05/12 02:57:09 INFO mapreduce.Job:  map 94% reduce 9%
17/05/12 02:57:14 INFO mapreduce.Job:  map 95% reduce 9%
17/05/12 02:57:15 INFO mapreduce.Job:  map 96% reduce 9%
17/05/12 02:57:16 INFO mapreduce.Job:  map 96% reduce 10%
17/05/12 02:57:20 INFO mapreduce.Job:  map 97% reduce 10%
17/05/12 02:57:21 INFO mapreduce.Job:  map 98% reduce 10%
17/05/12 02:57:27 INFO mapreduce.Job:  map 99% reduce 10%
17/05/12 02:57:29 INFO mapreduce.Job:  map 100% reduce 10%
17/05/12 02:57:30 INFO mapreduce.Job:  map 100% reduce 11%
17/05/12 02:57:31 INFO mapreduce.Job:  map 100% reduce 14%
17/05/12 02:57:32 INFO mapreduce.Job:  map 100% reduce 17%
17/05/12 02:57:33 INFO mapreduce.Job:  map 100% reduce 19%
17/05/12 02:57:34 INFO mapreduce.Job:  map 100% reduce 21%
17/05/12 02:57:36 INFO mapreduce.Job:  map 100% reduce 22%
17/05/12 02:57:37 INFO mapreduce.Job:  map 100% reduce 23%
17/05/12 02:57:38 INFO mapreduce.Job:  map 100% reduce 29%
17/05/12 02:57:39 INFO mapreduce.Job:  map 100% reduce 35%
17/05/12 02:57:40 INFO mapreduce.Job:  map 100% reduce 36%
17/05/12 02:57:41 INFO mapreduce.Job:  map 100% reduce 39%
17/05/12 02:57:42 INFO mapreduce.Job:  map 100% reduce 41%
17/05/12 02:57:43 INFO mapreduce.Job:  map 100% reduce 42%
17/05/12 02:57:44 INFO mapreduce.Job:  map 100% reduce 44%
17/05/12 02:57:45 INFO mapreduce.Job:  map 100% reduce 46%
17/05/12 02:57:47 INFO mapreduce.Job:  map 100% reduce 47%
17/05/12 02:57:48 INFO mapreduce.Job:  map 100% reduce 48%
17/05/12 02:57:50 INFO mapreduce.Job:  map 100% reduce 54%
17/05/12 02:57:53 INFO mapreduce.Job:  map 100% reduce 57%
17/05/12 02:57:56 INFO mapreduce.Job:  map 100% reduce 58%
17/05/12 02:57:57 INFO mapreduce.Job:  map 100% reduce 63%
17/05/12 02:57:59 INFO mapreduce.Job:  map 100% reduce 64%
17/05/12 02:58:00 INFO mapreduce.Job:  map 100% reduce 71%
17/05/12 02:58:01 INFO mapreduce.Job:  map 100% reduce 81%
17/05/12 02:58:03 INFO mapreduce.Job:  map 100% reduce 82%
17/05/12 02:58:04 INFO mapreduce.Job:  map 100% reduce 87%
17/05/12 02:58:06 INFO mapreduce.Job:  map 100% reduce 89%
17/05/12 02:58:07 INFO mapreduce.Job:  map 100% reduce 91%
17/05/12 02:58:09 INFO mapreduce.Job:  map 100% reduce 93%
17/05/12 02:58:10 INFO mapreduce.Job:  map 100% reduce 96%
17/05/12 02:58:12 INFO mapreduce.Job:  map 100% reduce 99%
17/05/12 02:58:13 INFO mapreduce.Job:  map 100% reduce 100%
17/05/12 02:58:14 INFO mapreduce.Job: Job job_1494557406271_0001 completed successfully
17/05/12 02:58:14 INFO mapreduce.Job: Counters: 50
	File System Counters
		FILE: Number of bytes read=2930661976
		FILE: Number of bytes written=5817665525
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=6553612138
		HDFS: Number of bytes written=6553600000
		HDFS: Number of read operations=336
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=20
	Job Counters 
		Launched map tasks=102
		Launched reduce tasks=10
		Data-local map tasks=100
		Rack-local map tasks=2
		Total time spent by all maps in occupied slots (ms)=740617
		Total time spent by all reduces in occupied slots (ms)=332054
		Total time spent by all map tasks (ms)=740617
		Total time spent by all reduce tasks (ms)=332054
		Total vcore-seconds taken by all map tasks=740617
		Total vcore-seconds taken by all reduce tasks=332054
		Total megabyte-seconds taken by all map tasks=758391808
		Total megabyte-seconds taken by all reduce tasks=340023296
	Map-Reduce Framework
		Map input records=65536000
		Map output records=65536000
		Map output bytes=6684672000
		Map output materialized bytes=2873059199
		Input split bytes=12138
		Combine input records=0
		Combine output records=0
		Reduce input groups=65536000
		Reduce shuffle bytes=2873059199
		Reduce input records=65536000
		Reduce output records=65536000
		Spilled Records=131072000
		Shuffled Maps =1020
		Failed Shuffles=0
		Merged Map outputs=1020
		GC time elapsed (ms)=14319
		CPU time spent (ms)=694980
		Physical memory (bytes) snapshot=60218122240
		Virtual memory (bytes) snapshot=175752515584
		Total committed heap usage (bytes)=67717038080
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
17/05/12 02:58:14 INFO terasort.TeraSort: done

real	4m20.069s
user	0m9.144s
sys	0m0.939s

```
