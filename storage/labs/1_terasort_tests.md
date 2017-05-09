
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
