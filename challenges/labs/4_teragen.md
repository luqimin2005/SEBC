The full teragen command and job output & The result of the time
```
[zhou@ip-172-31-38-5 ~]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar teragen -Ddfs.blocksize=64M -Dmapreduce.job.maps=6  -Dmapreduce.map.memory.mb=1024 65536000 /user/zhou/tgen
17/05/12 02:32:43 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-41-1/172.31.41.1:8032
17/05/12 02:32:44 INFO terasort.TeraSort: Generating 65536000 using 6
17/05/12 02:32:44 INFO mapreduce.JobSubmitter: number of splits:6
17/05/12 02:32:44 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1494555201739_0002
17/05/12 02:32:44 INFO impl.YarnClientImpl: Submitted application application_1494555201739_0002
17/05/12 02:32:45 INFO mapreduce.Job: The url to track the job: http://ip-172-31-41-1:8088/proxy/application_1494555201739_0002/
17/05/12 02:32:45 INFO mapreduce.Job: Running job: job_1494555201739_0002
17/05/12 02:32:52 INFO mapreduce.Job: Job job_1494555201739_0002 running in uber mode : false
17/05/12 02:32:52 INFO mapreduce.Job:  map 0% reduce 0%
17/05/12 02:33:03 INFO mapreduce.Job:  map 5% reduce 0%
17/05/12 02:33:04 INFO mapreduce.Job:  map 14% reduce 0%
17/05/12 02:33:05 INFO mapreduce.Job:  map 20% reduce 0%
17/05/12 02:33:06 INFO mapreduce.Job:  map 23% reduce 0%
17/05/12 02:33:07 INFO mapreduce.Job:  map 24% reduce 0%
17/05/12 02:33:08 INFO mapreduce.Job:  map 29% reduce 0%
17/05/12 02:33:09 INFO mapreduce.Job:  map 31% reduce 0%
17/05/12 02:33:10 INFO mapreduce.Job:  map 34% reduce 0%
17/05/12 02:33:11 INFO mapreduce.Job:  map 37% reduce 0%
17/05/12 02:33:13 INFO mapreduce.Job:  map 39% reduce 0%
17/05/12 02:33:14 INFO mapreduce.Job:  map 41% reduce 0%
17/05/12 02:33:15 INFO mapreduce.Job:  map 42% reduce 0%
17/05/12 02:33:16 INFO mapreduce.Job:  map 43% reduce 0%
17/05/12 02:33:17 INFO mapreduce.Job:  map 46% reduce 0%
17/05/12 02:33:18 INFO mapreduce.Job:  map 47% reduce 0%
17/05/12 02:33:19 INFO mapreduce.Job:  map 48% reduce 0%
17/05/12 02:33:20 INFO mapreduce.Job:  map 51% reduce 0%
17/05/12 02:33:22 INFO mapreduce.Job:  map 53% reduce 0%
17/05/12 02:33:23 INFO mapreduce.Job:  map 55% reduce 0%
17/05/12 02:33:24 INFO mapreduce.Job:  map 56% reduce 0%
17/05/12 02:33:25 INFO mapreduce.Job:  map 58% reduce 0%
17/05/12 02:33:26 INFO mapreduce.Job:  map 59% reduce 0%
17/05/12 02:33:27 INFO mapreduce.Job:  map 60% reduce 0%
17/05/12 02:33:28 INFO mapreduce.Job:  map 62% reduce 0%
17/05/12 02:33:29 INFO mapreduce.Job:  map 64% reduce 0%
17/05/12 02:33:30 INFO mapreduce.Job:  map 65% reduce 0%
17/05/12 02:33:31 INFO mapreduce.Job:  map 66% reduce 0%
17/05/12 02:33:32 INFO mapreduce.Job:  map 68% reduce 0%
17/05/12 02:33:33 INFO mapreduce.Job:  map 69% reduce 0%
17/05/12 02:33:34 INFO mapreduce.Job:  map 71% reduce 0%
17/05/12 02:33:35 INFO mapreduce.Job:  map 73% reduce 0%
17/05/12 02:33:37 INFO mapreduce.Job:  map 75% reduce 0%
17/05/12 02:33:38 INFO mapreduce.Job:  map 77% reduce 0%
17/05/12 02:33:41 INFO mapreduce.Job:  map 80% reduce 0%
17/05/12 02:33:44 INFO mapreduce.Job:  map 82% reduce 0%
17/05/12 02:33:45 INFO mapreduce.Job:  map 85% reduce 0%
17/05/12 02:33:48 INFO mapreduce.Job:  map 88% reduce 0%
17/05/12 02:33:51 INFO mapreduce.Job:  map 91% reduce 0%
17/05/12 02:33:54 INFO mapreduce.Job:  map 95% reduce 0%
17/05/12 02:33:57 INFO mapreduce.Job:  map 98% reduce 0%
17/05/12 02:33:59 INFO mapreduce.Job:  map 100% reduce 0%
17/05/12 02:34:01 INFO mapreduce.Job: Job job_1494555201739_0002 completed successfully
17/05/12 02:34:02 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=733536
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=511
		HDFS: Number of bytes written=6553600000
		HDFS: Number of read operations=24
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=12
	Job Counters 
		Launched map tasks=6
		Other local map tasks=6
		Total time spent by all maps in occupied slots (ms)=259299
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=259299
		Total vcore-seconds taken by all map tasks=259299
		Total megabyte-seconds taken by all map tasks=265522176
	Map-Reduce Framework
		Map input records=65536000
		Map output records=65536000
		Input split bytes=511
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=972
		CPU time spent (ms)=126500
		Physical memory (bytes) snapshot=1913765888
		Virtual memory (bytes) snapshot=9366212608
		Total committed heap usage (bytes)=1911029760
	org.apache.hadoop.examples.terasort.TeraGen$Counters
		CHECKSUM=140750829423462787
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=6553600000

real	1m21.298s
user	0m5.956s
sys	0m0.656s

```

The command and output of hdfs dfs -ls /user/zhou/tgen
```
[zhou@ip-172-31-38-5 ~]$ hdfs dfs -ls /user/zhou/tgen
Found 7 items
-rw-r--r--   3 zhou supergroup          0 2017-05-12 02:33 /user/zhou/tgen/_SUCCESS
-rw-r--r--   3 zhou supergroup 1092266700 2017-05-12 02:33 /user/zhou/tgen/part-m-00000
-rw-r--r--   3 zhou supergroup 1092266700 2017-05-12 02:33 /user/zhou/tgen/part-m-00001
-rw-r--r--   3 zhou supergroup 1092266600 2017-05-12 02:33 /user/zhou/tgen/part-m-00002
-rw-r--r--   3 zhou supergroup 1092266700 2017-05-12 02:33 /user/zhou/tgen/part-m-00003
-rw-r--r--   3 zhou supergroup 1092266700 2017-05-12 02:33 /user/zhou/tgen/part-m-00004
-rw-r--r--   3 zhou supergroup 1092266600 2017-05-12 02:33 /user/zhou/tgen/part-m-00005
```

