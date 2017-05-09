
Slowest:
MAP:2 , REDUCE:2 , Container memory:512MB
```
real	1m32.115s
user	0m5.864s
sys	0m0.776s

real	2m34.587s
user	0m8.591s
sys	0m0.969s
```

Fastest:
MAP:8 , REDUCE:4 , Container memory:1024MB
```
real	0m58.621s
user	0m6.634s
sys	0m0.840s

real	2m0.396s
user	0m8.828s
sys	0m0.854s
```



All Output:
```
[hdfs@ip-172-31-35-195 ~]$ /tmp/yarntest.sh 
Testing loop started on Tue May 9 09:42:11 UTC 2017

real	1m32.115s
user	0m5.864s
sys	0m0.776s

real	2m34.587s
user	0m8.591s
sys	0m0.969s
Deleted /results/tg-10GB-2-2-512
Deleted /results/ts-10GB-2-2-512

real	1m14.778s
user	0m6.258s
sys	0m0.812s

real	2m34.094s
user	0m8.620s
sys	0m0.916s
Deleted /results/tg-10GB-2-2-1024
Deleted /results/ts-10GB-2-2-1024

real	1m32.916s
user	0m6.310s
sys	0m0.814s

real	2m0.960s
user	0m8.156s
sys	0m0.916s
Deleted /results/tg-10GB-2-4-512
Deleted /results/ts-10GB-2-4-512

real	1m18.444s
user	0m6.437s
sys	0m0.876s

real	2m1.835s
user	0m8.351s
sys	0m0.798s
Deleted /results/tg-10GB-2-4-1024
Deleted /results/ts-10GB-2-4-1024

real	1m5.132s
user	0m6.327s
sys	0m0.838s

real	2m20.468s
user	0m8.197s
sys	0m0.789s
Deleted /results/tg-10GB-4-2-512
Deleted /results/ts-10GB-4-2-512

real	1m7.062s
user	0m6.293s
sys	0m0.758s

real	2m11.293s
user	0m9.016s
sys	0m0.842s
Deleted /results/tg-10GB-4-2-1024
Deleted /results/ts-10GB-4-2-1024

real	1m20.261s
user	0m6.064s
sys	0m0.768s

real	1m59.863s
user	0m8.021s
sys	0m0.827s
Deleted /results/tg-10GB-4-4-512
Deleted /results/ts-10GB-4-4-512

real	1m20.582s
user	0m6.559s
sys	0m0.818s

real	2m19.203s
user	0m8.373s
sys	0m0.918s
Deleted /results/tg-10GB-4-4-1024
Deleted /results/ts-10GB-4-4-1024

real	1m8.623s
user	0m6.039s
sys	0m0.833s

real	2m18.814s
user	0m8.295s
sys	0m0.904s
Deleted /results/tg-10GB-8-2-512
Deleted /results/ts-10GB-8-2-512

real	0m58.449s
user	0m6.371s
sys	0m0.791s

real	2m10.160s
user	0m8.274s
sys	0m0.980s
Deleted /results/tg-10GB-8-2-1024
Deleted /results/ts-10GB-8-2-1024

real	1m1.463s
user	0m6.270s
sys	0m0.837s

real	2m12.355s
user	0m8.679s
sys	0m0.998s
Deleted /results/tg-10GB-8-4-512
Deleted /results/ts-10GB-8-4-512

real	0m58.621s
user	0m6.634s
sys	0m0.840s

real	2m0.396s
user	0m8.828s
sys	0m0.854s
Deleted /results/tg-10GB-8-4-1024
Deleted /results/ts-10GB-8-4-1024
Testing loop ended on Tue May 9 10:24:44 UTC 2017

```
