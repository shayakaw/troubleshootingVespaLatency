vespa 7.3xx
```
date; LD_LIBRARY_PATH=/opt/vespa/lib64 vespa-fbench -n 10 -c 0 -s 60 localhost 4080 -q search_query2.txt -o res
Tue Apr 20 18:51:22 JST 2021
Starting clients...
[dummydate]: PROGRESS: vespa-fbench: Seconds left 60
Stopping clients
Clients stopped.
..........
Clients Joined.
*** HTTP keep-alive statistics ***
connection reuse count -- 177926
***************** Benchmark Summary *****************
clients:                      10
ran for:                      60 seconds
cycle time:                    0 ms
lower response limit:          0 bytes
skipped requests:              0
failed requests:               0
successful requests:      177936
cycles not held:          177936
minimum response time:      1.21 ms
maximum response time:     32.30 ms
average response time:      3.36 ms
25   percentile:              2.60 ms
50   percentile:              3.40 ms
75   percentile:              3.90 ms
90   percentile:              4.40 ms
95   percentile:              4.70 ms
98   percentile:              5.20 ms
99   percentile:              5.50 ms
99.5 percentile:              6.40 ms
99.6 percentile:              7.10 ms
99.7 percentile:              7.70 ms
99.8 percentile:             15.00 ms
99.9 percentile:             19.20 ms
actual query rate:       2968.55 Q/s
utilization:               99.73 %
zero hit queries:          71174
http request status breakdown:
       200 :   177831
       504 :      105
```


vespa7.1xx
```
date; LD_LIBRARY_PATH=/opt/vespa/lib64 vespa-fbench -n 10 -c 0 -s 60 localhost 4080 -q search_query2.txt -o res
Tue Apr 20 18:51:28 JST 2021
Starting clients...
[dummydate]: PROGRESS: vespa-fbench: Seconds left 60
Stopping clients
Clients stopped.
..........
Clients Joined.
*** HTTP keep-alive statistics ***
connection reuse count -- 193962
***************** Benchmark Summary *****************
clients:                      10
ran for:                      60 seconds
cycle time:                    0 ms
lower response limit:          0 bytes
skipped requests:              0
failed requests:               0
successful requests:      193972
cycles not held:          193972
minimum response time:      1.25 ms
maximum response time:     25.70 ms
average response time:      3.07 ms
25 percentile:              2.40 ms
50 percentile:              3.00 ms
75 percentile:              3.60 ms
90 percentile:              3.90 ms
95 percentile:              4.20 ms
99 percentile:              7.40 ms
actual query rate:       3238.50 Q/s
utilization:               99.49 %
zero hit queries:          77589
http request status breakdown:
       200 :   193972
```
