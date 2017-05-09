Linux account
```
[root@ip-172-31-35-195 ~]# id luqimin2005
uid=500(luqimin2005) gid=500(luqimin2005) groups=500(luqimin2005)
[root@ip-172-31-35-195 ~]# hadoop fs -ls /user | grep luqimin2005
drwxr-xr-x   - luqimin2005 supergroup          0 2017-05-09 06:29 /user/luqimin2005
```

teragen
```
[luqimin2005@ip-172-31-35-195 ~]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar teragen -D dfs.blocksize=32M -D mapreduce.job.maps=4 104857600 /user/luqimin2005/teragen
17/05/09 05:36:28 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-35-195/172.31.35.195:8032
17/05/09 05:36:29 INFO terasort.TeraSort: Generating 104857600 using 4
17/05/09 05:36:29 INFO mapreduce.JobSubmitter: number of splits:4
17/05/09 05:36:29 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1494257893856_0008
17/05/09 05:36:29 INFO impl.YarnClientImpl: Submitted application application_1494257893856_0008
17/05/09 05:36:30 INFO mapreduce.Job: The url to track the job: http://ip-172-31-35-195:8088/proxy/application_1494257893856_0008/
17/05/09 05:36:30 INFO mapreduce.Job: Running job: job_1494257893856_0008
17/05/09 05:36:36 INFO mapreduce.Job: Job job_1494257893856_0008 running in uber mode : false
17/05/09 05:36:36 INFO mapreduce.Job:  map 0% reduce 0%
17/05/09 05:36:48 INFO mapreduce.Job:  map 7% reduce 0%
17/05/09 05:36:49 INFO mapreduce.Job:  map 9% reduce 0%
17/05/09 05:36:50 INFO mapreduce.Job:  map 12% reduce 0%
17/05/09 05:36:51 INFO mapreduce.Job:  map 15% reduce 0%
17/05/09 05:36:52 INFO mapreduce.Job:  map 16% reduce 0%
17/05/09 05:36:53 INFO mapreduce.Job:  map 18% reduce 0%
17/05/09 05:36:54 INFO mapreduce.Job:  map 20% reduce 0%
17/05/09 05:36:55 INFO mapreduce.Job:  map 21% reduce 0%
17/05/09 05:36:57 INFO mapreduce.Job:  map 23% reduce 0%
17/05/09 05:36:58 INFO mapreduce.Job:  map 24% reduce 0%
17/05/09 05:37:00 INFO mapreduce.Job:  map 26% reduce 0%
17/05/09 05:37:01 INFO mapreduce.Job:  map 27% reduce 0%
17/05/09 05:37:02 INFO mapreduce.Job:  map 28% reduce 0%
17/05/09 05:37:03 INFO mapreduce.Job:  map 29% reduce 0%
17/05/09 05:37:04 INFO mapreduce.Job:  map 30% reduce 0%
17/05/09 05:37:05 INFO mapreduce.Job:  map 31% reduce 0%
17/05/09 05:37:06 INFO mapreduce.Job:  map 32% reduce 0%
17/05/09 05:37:08 INFO mapreduce.Job:  map 34% reduce 0%
17/05/09 05:37:09 INFO mapreduce.Job:  map 35% reduce 0%
17/05/09 05:37:10 INFO mapreduce.Job:  map 36% reduce 0%
17/05/09 05:37:11 INFO mapreduce.Job:  map 37% reduce 0%
17/05/09 05:37:13 INFO mapreduce.Job:  map 39% reduce 0%
17/05/09 05:37:14 INFO mapreduce.Job:  map 41% reduce 0%
17/05/09 05:37:16 INFO mapreduce.Job:  map 43% reduce 0%
17/05/09 05:37:17 INFO mapreduce.Job:  map 44% reduce 0%
17/05/09 05:37:20 INFO mapreduce.Job:  map 45% reduce 0%
17/05/09 05:37:21 INFO mapreduce.Job:  map 46% reduce 0%
17/05/09 05:37:23 INFO mapreduce.Job:  map 47% reduce 0%
17/05/09 05:37:24 INFO mapreduce.Job:  map 49% reduce 0%
17/05/09 05:37:26 INFO mapreduce.Job:  map 50% reduce 0%
17/05/09 05:37:27 INFO mapreduce.Job:  map 52% reduce 0%
17/05/09 05:37:29 INFO mapreduce.Job:  map 53% reduce 0%
17/05/09 05:37:30 INFO mapreduce.Job:  map 55% reduce 0%
17/05/09 05:37:32 INFO mapreduce.Job:  map 56% reduce 0%
17/05/09 05:37:33 INFO mapreduce.Job:  map 57% reduce 0%
17/05/09 05:37:35 INFO mapreduce.Job:  map 58% reduce 0%
17/05/09 05:37:36 INFO mapreduce.Job:  map 59% reduce 0%
17/05/09 05:37:37 INFO mapreduce.Job:  map 60% reduce 0%
17/05/09 05:37:39 INFO mapreduce.Job:  map 62% reduce 0%
17/05/09 05:37:40 INFO mapreduce.Job:  map 63% reduce 0%
17/05/09 05:37:42 INFO mapreduce.Job:  map 65% reduce 0%
17/05/09 05:37:43 INFO mapreduce.Job:  map 66% reduce 0%
17/05/09 05:37:44 INFO mapreduce.Job:  map 67% reduce 0%
17/05/09 05:37:45 INFO mapreduce.Job:  map 69% reduce 0%
17/05/09 05:37:47 INFO mapreduce.Job:  map 70% reduce 0%
17/05/09 05:37:48 INFO mapreduce.Job:  map 72% reduce 0%
17/05/09 05:37:49 INFO mapreduce.Job:  map 73% reduce 0%
17/05/09 05:37:51 INFO mapreduce.Job:  map 75% reduce 0%
17/05/09 05:37:53 INFO mapreduce.Job:  map 76% reduce 0%
17/05/09 05:37:54 INFO mapreduce.Job:  map 77% reduce 0%
17/05/09 05:37:55 INFO mapreduce.Job:  map 78% reduce 0%
17/05/09 05:37:56 INFO mapreduce.Job:  map 79% reduce 0%
17/05/09 05:37:58 INFO mapreduce.Job:  map 80% reduce 0%
17/05/09 05:37:59 INFO mapreduce.Job:  map 81% reduce 0%
17/05/09 05:38:01 INFO mapreduce.Job:  map 83% reduce 0%
17/05/09 05:38:02 INFO mapreduce.Job:  map 84% reduce 0%
17/05/09 05:38:03 INFO mapreduce.Job:  map 85% reduce 0%
17/05/09 05:38:04 INFO mapreduce.Job:  map 86% reduce 0%
17/05/09 05:38:05 INFO mapreduce.Job:  map 87% reduce 0%
17/05/09 05:38:06 INFO mapreduce.Job:  map 88% reduce 0%
17/05/09 05:38:08 INFO mapreduce.Job:  map 89% reduce 0%
17/05/09 05:38:10 INFO mapreduce.Job:  map 91% reduce 0%
17/05/09 05:38:11 INFO mapreduce.Job:  map 92% reduce 0%
17/05/09 05:38:12 INFO mapreduce.Job:  map 93% reduce 0%
17/05/09 05:38:14 INFO mapreduce.Job:  map 94% reduce 0%
17/05/09 05:38:17 INFO mapreduce.Job:  map 96% reduce 0%
17/05/09 05:38:20 INFO mapreduce.Job:  map 98% reduce 0%
17/05/09 05:38:23 INFO mapreduce.Job:  map 100% reduce 0%
17/05/09 05:38:24 INFO mapreduce.Job: Job job_1494257893856_0008 completed successfully
17/05/09 05:38:24 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=492452
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=344
		HDFS: Number of bytes written=10485760000
		HDFS: Number of read operations=16
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=8
	Job Counters 
		Launched map tasks=4
		Other local map tasks=4
		Total time spent by all maps in occupied slots (ms)=391156
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=391156
		Total vcore-seconds taken by all map tasks=391156
		Total megabyte-seconds taken by all map tasks=400543744
	Map-Reduce Framework
		Map input records=104857600
		Map output records=104857600
		Input split bytes=344
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=1661
		CPU time spent (ms)=161140
		Physical memory (bytes) snapshot=884609024
		Virtual memory (bytes) snapshot=6268854272
		Total committed heap usage (bytes)=875036672
	org.apache.hadoop.examples.terasort.TeraGen$Counters
		CHECKSUM=225186913807133164
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=10485760000

real	1m58.835s
user	0m5.845s
sys	0m0.721s


```

terasort
```
[luqimin2005@ip-172-31-35-195 ~]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar terasort /user/luqimin2005/teragen /user/luqimin2005/terasort
17/05/09 06:16:09 INFO terasort.TeraSort: starting
17/05/09 06:16:10 INFO input.FileInputFormat: Total input paths to process : 4
Spent 293ms computing base-splits.
Spent 6ms computing TeraScheduler splits.
Computing input splits took 300ms
Sampling 10 splits of 316
Making 10 from 100000 sampled records
Computing parititions took 1104ms
Spent 1407ms computing partitions.
17/05/09 06:16:11 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-35-195/172.31.35.195:8032
17/05/09 06:16:12 INFO mapreduce.JobSubmitter: number of splits:316
17/05/09 06:16:12 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1494257893856_0009
17/05/09 06:16:12 INFO impl.YarnClientImpl: Submitted application application_1494257893856_0009
17/05/09 06:16:12 INFO mapreduce.Job: The url to track the job: http://ip-172-31-35-195:8088/proxy/application_1494257893856_0009/
17/05/09 06:16:12 INFO mapreduce.Job: Running job: job_1494257893856_0009
17/05/09 06:16:20 INFO mapreduce.Job: Job job_1494257893856_0009 running in uber mode : false
17/05/09 06:16:20 INFO mapreduce.Job:  map 0% reduce 0%
17/05/09 06:16:27 INFO mapreduce.Job:  map 1% reduce 0%
17/05/09 06:16:29 INFO mapreduce.Job:  map 2% reduce 0%
17/05/09 06:16:32 INFO mapreduce.Job:  map 3% reduce 0%
17/05/09 06:16:37 INFO mapreduce.Job:  map 4% reduce 0%
17/05/09 06:16:41 INFO mapreduce.Job:  map 5% reduce 0%
17/05/09 06:16:42 INFO mapreduce.Job:  map 6% reduce 0%
17/05/09 06:16:46 INFO mapreduce.Job:  map 7% reduce 0%
17/05/09 06:16:48 INFO mapreduce.Job:  map 8% reduce 0%
17/05/09 06:16:53 INFO mapreduce.Job:  map 9% reduce 0%
17/05/09 06:16:54 INFO mapreduce.Job:  map 10% reduce 0%
17/05/09 06:17:00 INFO mapreduce.Job:  map 11% reduce 0%
17/05/09 06:17:03 INFO mapreduce.Job:  map 13% reduce 0%
17/05/09 06:17:09 INFO mapreduce.Job:  map 14% reduce 0%
17/05/09 06:17:12 INFO mapreduce.Job:  map 15% reduce 0%
17/05/09 06:17:14 INFO mapreduce.Job:  map 16% reduce 0%
17/05/09 06:17:19 INFO mapreduce.Job:  map 17% reduce 0%
17/05/09 06:17:23 INFO mapreduce.Job:  map 18% reduce 0%
17/05/09 06:17:25 INFO mapreduce.Job:  map 19% reduce 0%
17/05/09 06:17:26 INFO mapreduce.Job:  map 20% reduce 0%
17/05/09 06:17:31 INFO mapreduce.Job:  map 21% reduce 0%
17/05/09 06:17:35 INFO mapreduce.Job:  map 22% reduce 0%
17/05/09 06:17:37 INFO mapreduce.Job:  map 23% reduce 0%
17/05/09 06:17:42 INFO mapreduce.Job:  map 24% reduce 0%
17/05/09 06:17:44 INFO mapreduce.Job:  map 25% reduce 0%
17/05/09 06:17:46 INFO mapreduce.Job:  map 26% reduce 0%
17/05/09 06:17:50 INFO mapreduce.Job:  map 27% reduce 0%
17/05/09 06:17:52 INFO mapreduce.Job:  map 28% reduce 0%
17/05/09 06:17:57 INFO mapreduce.Job:  map 29% reduce 0%
17/05/09 06:17:58 INFO mapreduce.Job:  map 30% reduce 0%
17/05/09 06:18:05 INFO mapreduce.Job:  map 31% reduce 0%
17/05/09 06:18:06 INFO mapreduce.Job:  map 32% reduce 0%
17/05/09 06:18:07 INFO mapreduce.Job:  map 33% reduce 0%
17/05/09 06:18:12 INFO mapreduce.Job:  map 34% reduce 0%
17/05/09 06:18:16 INFO mapreduce.Job:  map 35% reduce 0%
17/05/09 06:18:18 INFO mapreduce.Job:  map 36% reduce 0%
17/05/09 06:18:24 INFO mapreduce.Job:  map 37% reduce 0%
17/05/09 06:18:27 INFO mapreduce.Job:  map 38% reduce 0%
17/05/09 06:18:28 INFO mapreduce.Job:  map 39% reduce 0%
17/05/09 06:18:32 INFO mapreduce.Job:  map 40% reduce 0%
17/05/09 06:18:36 INFO mapreduce.Job:  map 41% reduce 0%
17/05/09 06:18:39 INFO mapreduce.Job:  map 42% reduce 0%
17/05/09 06:18:41 INFO mapreduce.Job:  map 43% reduce 0%
17/05/09 06:18:46 INFO mapreduce.Job:  map 44% reduce 0%
17/05/09 06:18:48 INFO mapreduce.Job:  map 45% reduce 0%
17/05/09 06:18:50 INFO mapreduce.Job:  map 46% reduce 0%
17/05/09 06:18:55 INFO mapreduce.Job:  map 47% reduce 0%
17/05/09 06:18:57 INFO mapreduce.Job:  map 48% reduce 0%
17/05/09 06:19:02 INFO mapreduce.Job:  map 49% reduce 0%
17/05/09 06:19:04 INFO mapreduce.Job:  map 50% reduce 0%
17/05/09 06:19:07 INFO mapreduce.Job:  map 51% reduce 0%
17/05/09 06:19:10 INFO mapreduce.Job:  map 52% reduce 0%
17/05/09 06:19:12 INFO mapreduce.Job:  map 53% reduce 0%
17/05/09 06:19:17 INFO mapreduce.Job:  map 54% reduce 0%
17/05/09 06:19:19 INFO mapreduce.Job:  map 55% reduce 0%
17/05/09 06:19:23 INFO mapreduce.Job:  map 56% reduce 0%
17/05/09 06:19:27 INFO mapreduce.Job:  map 57% reduce 0%
17/05/09 06:19:28 INFO mapreduce.Job:  map 58% reduce 0%
17/05/09 06:19:32 INFO mapreduce.Job:  map 59% reduce 0%
17/05/09 06:19:36 INFO mapreduce.Job:  map 60% reduce 0%
17/05/09 06:19:38 INFO mapreduce.Job:  map 61% reduce 0%
17/05/09 06:19:43 INFO mapreduce.Job:  map 62% reduce 0%
17/05/09 06:19:46 INFO mapreduce.Job:  map 63% reduce 0%
17/05/09 06:19:47 INFO mapreduce.Job:  map 64% reduce 0%
17/05/09 06:19:51 INFO mapreduce.Job:  map 65% reduce 0%
17/05/09 06:19:52 INFO mapreduce.Job:  map 66% reduce 0%
17/05/09 06:19:58 INFO mapreduce.Job:  map 67% reduce 0%
17/05/09 06:19:59 INFO mapreduce.Job:  map 68% reduce 0%
17/05/09 06:20:05 INFO mapreduce.Job:  map 69% reduce 0%
17/05/09 06:20:07 INFO mapreduce.Job:  map 70% reduce 0%
17/05/09 06:20:08 INFO mapreduce.Job:  map 71% reduce 0%
17/05/09 06:20:12 INFO mapreduce.Job:  map 72% reduce 0%
17/05/09 06:20:16 INFO mapreduce.Job:  map 73% reduce 0%
17/05/09 06:20:18 INFO mapreduce.Job:  map 74% reduce 0%
17/05/09 06:20:23 INFO mapreduce.Job:  map 75% reduce 0%
17/05/09 06:20:26 INFO mapreduce.Job:  map 76% reduce 0%
17/05/09 06:20:29 INFO mapreduce.Job:  map 77% reduce 0%
17/05/09 06:20:32 INFO mapreduce.Job:  map 78% reduce 0%
17/05/09 06:20:36 INFO mapreduce.Job:  map 79% reduce 0%
17/05/09 06:20:39 INFO mapreduce.Job:  map 80% reduce 0%
17/05/09 06:20:40 INFO mapreduce.Job:  map 81% reduce 0%
17/05/09 06:20:46 INFO mapreduce.Job:  map 82% reduce 0%
17/05/09 06:20:47 INFO mapreduce.Job:  map 83% reduce 0%
17/05/09 06:20:49 INFO mapreduce.Job:  map 84% reduce 0%
17/05/09 06:20:58 INFO mapreduce.Job:  map 84% reduce 4%
17/05/09 06:20:59 INFO mapreduce.Job:  map 84% reduce 7%
17/05/09 06:21:00 INFO mapreduce.Job:  map 85% reduce 10%
17/05/09 06:21:01 INFO mapreduce.Job:  map 85% reduce 11%
17/05/09 06:21:02 INFO mapreduce.Job:  map 85% reduce 12%
17/05/09 06:21:03 INFO mapreduce.Job:  map 85% reduce 14%
17/05/09 06:21:09 INFO mapreduce.Job:  map 86% reduce 14%
17/05/09 06:21:18 INFO mapreduce.Job:  map 87% reduce 14%
17/05/09 06:21:22 INFO mapreduce.Job:  map 87% reduce 15%
17/05/09 06:21:25 INFO mapreduce.Job:  map 88% reduce 15%
17/05/09 06:21:32 INFO mapreduce.Job:  map 89% reduce 15%
17/05/09 06:21:39 INFO mapreduce.Job:  map 90% reduce 15%
17/05/09 06:21:47 INFO mapreduce.Job:  map 91% reduce 15%
17/05/09 06:21:57 INFO mapreduce.Job:  map 92% reduce 15%
17/05/09 06:22:04 INFO mapreduce.Job:  map 93% reduce 15%
17/05/09 06:22:07 INFO mapreduce.Job:  map 93% reduce 16%
17/05/09 06:22:11 INFO mapreduce.Job:  map 94% reduce 16%
17/05/09 06:22:19 INFO mapreduce.Job:  map 95% reduce 16%
17/05/09 06:22:27 INFO mapreduce.Job:  map 96% reduce 16%
17/05/09 06:22:34 INFO mapreduce.Job:  map 97% reduce 16%
17/05/09 06:22:43 INFO mapreduce.Job:  map 98% reduce 16%
17/05/09 06:22:50 INFO mapreduce.Job:  map 99% reduce 16%
17/05/09 06:22:56 INFO mapreduce.Job:  map 99% reduce 17%
17/05/09 06:22:59 INFO mapreduce.Job:  map 100% reduce 17%
17/05/09 06:23:02 INFO mapreduce.Job:  map 100% reduce 23%
17/05/09 06:23:04 INFO mapreduce.Job:  map 100% reduce 27%
17/05/09 06:23:05 INFO mapreduce.Job:  map 100% reduce 37%
17/05/09 06:23:08 INFO mapreduce.Job:  map 100% reduce 41%
17/05/09 06:23:11 INFO mapreduce.Job:  map 100% reduce 48%
17/05/09 06:23:13 INFO mapreduce.Job:  map 100% reduce 49%
17/05/09 06:23:14 INFO mapreduce.Job:  map 100% reduce 54%
17/05/09 06:23:15 INFO mapreduce.Job:  map 100% reduce 55%
17/05/09 06:23:17 INFO mapreduce.Job:  map 100% reduce 60%
17/05/09 06:23:20 INFO mapreduce.Job:  map 100% reduce 63%
17/05/09 06:23:21 INFO mapreduce.Job:  map 100% reduce 66%
17/05/09 06:23:23 INFO mapreduce.Job:  map 100% reduce 68%
17/05/09 06:23:25 INFO mapreduce.Job:  map 100% reduce 73%
17/05/09 06:23:26 INFO mapreduce.Job:  map 100% reduce 78%
17/05/09 06:23:28 INFO mapreduce.Job:  map 100% reduce 79%
17/05/09 06:23:29 INFO mapreduce.Job:  map 100% reduce 80%
17/05/09 06:23:30 INFO mapreduce.Job:  map 100% reduce 81%
17/05/09 06:23:32 INFO mapreduce.Job:  map 100% reduce 83%
17/05/09 06:23:34 INFO mapreduce.Job:  map 100% reduce 87%
17/05/09 06:23:35 INFO mapreduce.Job:  map 100% reduce 91%
17/05/09 06:23:37 INFO mapreduce.Job:  map 100% reduce 92%
17/05/09 06:23:38 INFO mapreduce.Job:  map 100% reduce 94%
17/05/09 06:23:40 INFO mapreduce.Job:  map 100% reduce 95%
17/05/09 06:23:41 INFO mapreduce.Job:  map 100% reduce 97%
17/05/09 06:23:43 INFO mapreduce.Job:  map 100% reduce 98%
17/05/09 06:23:45 INFO mapreduce.Job:  map 100% reduce 99%
17/05/09 06:23:47 INFO mapreduce.Job:  map 100% reduce 100%
17/05/09 06:23:48 INFO mapreduce.Job: Job job_1494257893856_0009 completed successfully
17/05/09 06:23:48 INFO mapreduce.Job: Counters: 50
	File System Counters
		FILE: Number of bytes read=4695156802
		FILE: Number of bytes written=9323112280
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=10485801396
		HDFS: Number of bytes written=10485760000
		HDFS: Number of read operations=978
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=20
	Job Counters 
		Launched map tasks=316
		Launched reduce tasks=10
		Data-local map tasks=309
		Rack-local map tasks=7
		Total time spent by all maps in occupied slots (ms)=2175760
		Total time spent by all reduces in occupied slots (ms)=930088
		Total time spent by all map tasks (ms)=2175760
		Total time spent by all reduce tasks (ms)=930088
		Total vcore-seconds taken by all map tasks=2175760
		Total vcore-seconds taken by all reduce tasks=930088
		Total megabyte-seconds taken by all map tasks=2227978240
		Total megabyte-seconds taken by all reduce tasks=952410112
	Map-Reduce Framework
		Map input records=104857600
		Map output records=104857600
		Map output bytes=10695475200
		Map output materialized bytes=4587323710
		Input split bytes=41396
		Combine input records=0
		Combine output records=0
		Reduce input groups=104857600
		Reduce shuffle bytes=4587323710
		Reduce input records=104857600
		Reduce output records=104857600
		Spilled Records=209715200
		Shuffled Maps =3160
		Failed Shuffles=0
		Merged Map outputs=3160
		GC time elapsed (ms)=30347
		CPU time spent (ms)=1454780
		Physical memory (bytes) snapshot=154383134720
		Virtual memory (bytes) snapshot=510451367936
		Total committed heap usage (bytes)=186116997120
	Shuffle Errors
		BAD_ID=0
		CONNECTION=0
		IO_ERROR=0
		WRONG_LENGTH=0
		WRONG_MAP=0
		WRONG_REDUCE=0
	File Input Format Counters 
		Bytes Read=10485760000
	File Output Format Counters 
		Bytes Written=10485760000
17/05/09 06:23:48 INFO terasort.TeraSort: done

real	7m41.095s
user	0m10.717s
sys	0m1.227s
```
