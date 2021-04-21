vespa 7.3
```
First

$ date; LD_LIBRARY_PATH=/opt/vespa/lib64 vespa-fbench -n 10 -c 0 -s 60 localhost 4080 -q search_query2.txt -o res
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


Second time

$ date; LD_LIBRARY_PATH=/opt/vespa/lib64 vespa-fbench -n 10 -c 0 -s 300 localhost 4080 -q search_query2.txt -o res
Wed Apr 21 11:42:19 JST 2021
Starting clients...
[dummydate]: PROGRESS: vespa-fbench: Seconds left 300
[dummydate]: PROGRESS: vespa-fbench: Seconds left 240
[dummydate]: PROGRESS: vespa-fbench: Seconds left 180
[dummydate]: PROGRESS: vespa-fbench: Seconds left 120
[dummydate]: PROGRESS: vespa-fbench: Seconds left 60
Stopping clients
Clients stopped.
..........
Clients Joined.
*** HTTP keep-alive statistics ***
connection reuse count -- 892199
***************** Benchmark Summary *****************
clients:                      10
ran for:                     300 seconds
cycle time:                    0 ms
lower response limit:          0 bytes
skipped requests:              0
failed requests:               0
successful requests:      892209
cycles not held:          892209
minimum response time:      1.11 ms
maximum response time:     33.75 ms
average response time:      3.35 ms
25   percentile:              2.60 ms
50   percentile:              3.30 ms
75   percentile:              3.90 ms
90   percentile:              4.40 ms
95   percentile:              4.70 ms
98   percentile:              5.10 ms
99   percentile:              5.50 ms
99.5 percentile:              6.10 ms
99.6 percentile:              6.80 ms
99.7 percentile:              7.60 ms
99.8 percentile:             13.70 ms
99.9 percentile:             16.70 ms
actual query rate:       2978.37 Q/s
utilization:               99.73 %
zero hit queries:         356875
http request status breakdown:
       200 :   891807
       504 :      402


Third time

$ date; LD_LIBRARY_PATH=/opt/vespa/lib64 vespa-fbench -n 10 -c 0 -s 300 localhost 4080 -q search_query2.txt -o res
Wed Apr 21 15:30:59 JST 2021
Starting clients...
[dummydate]: PROGRESS: vespa-fbench: Seconds left 300
[dummydate]: PROGRESS: vespa-fbench: Seconds left 240
[dummydate]: PROGRESS: vespa-fbench: Seconds left 180
[dummydate]: PROGRESS: vespa-fbench: Seconds left 120
[dummydate]: PROGRESS: vespa-fbench: Seconds left 60
Stopping clients
Clients stopped.
..........
Clients Joined.
*** HTTP keep-alive statistics ***
connection reuse count -- 889185
***************** Benchmark Summary *****************
clients:                      10
ran for:                     300 seconds
cycle time:                    0 ms
lower response limit:          0 bytes
skipped requests:              0
failed requests:               0
successful requests:      889195
cycles not held:          889195
minimum response time:      1.20 ms
maximum response time:     32.47 ms
average response time:      3.36 ms
25   percentile:              2.60 ms
50   percentile:              3.40 ms
75   percentile:              3.90 ms
90   percentile:              4.40 ms
95   percentile:              4.70 ms
98   percentile:              5.20 ms
99   percentile:              5.50 ms
99.5 percentile:              6.30 ms
99.6 percentile:              6.90 ms
99.7 percentile:              7.60 ms
99.8 percentile:             13.70 ms
99.9 percentile:             16.70 ms
actual query rate:       2967.74 Q/s
utilization:               99.73 %
zero hit queries:         355663
http request status breakdown:
       200 :   888812
       504 :      383
```

vespa 7.1
```
First time
$ date; LD_LIBRARY_PATH=/opt/vespa/lib64 vespa-fbench -n 10 -c 0 -s 60 localhost 4080 -q search_query2.txt -o res
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




Second time
$ date; LD_LIBRARY_PATH=/opt/vespa/lib64 vespa-fbench -n 10 -c 0 -s 300 localhost 4080 -q search_query2.txt -o res
Wed Apr 21 11:42:29 JST 2021
Starting clients...
[dummydate]: PROGRESS: vespa-fbench: Seconds left 300
[dummydate]: PROGRESS: vespa-fbench: Seconds left 240
[dummydate]: PROGRESS: vespa-fbench: Seconds left 180
[dummydate]: PROGRESS: vespa-fbench: Seconds left 120
[dummydate]: PROGRESS: vespa-fbench: Seconds left 60
Stopping clients
Clients stopped.
..........
Clients Joined.
*** HTTP keep-alive statistics ***
connection reuse count -- 971943
***************** Benchmark Summary *****************
clients:                      10
ran for:                     300 seconds
cycle time:                    0 ms
lower response limit:          0 bytes
skipped requests:              0
failed requests:               0
successful requests:      971953
cycles not held:          971953
minimum response time:      1.25 ms
maximum response time:     24.64 ms
average response time:      3.07 ms
25 percentile:              2.50 ms
50 percentile:              3.00 ms
75 percentile:              3.60 ms
90 percentile:              3.90 ms
95 percentile:              4.20 ms
99 percentile:              4.60 ms
actual query rate:       3242.79 Q/s
utilization:               99.43 %
zero hit queries:         388779
http request status breakdown:
       200 :   971953





Third time
$ date; LD_LIBRARY_PATH=/opt/vespa/lib64 vespa-fbench -n 10 -c 0 -s 300 localhost 4080 -q search_query2.txt -o res

Wed Apr 21 15:31:03 JST 2021
Starting clients...
[dummydate]: PROGRESS: vespa-fbench: Seconds left 300
[dummydate]: PROGRESS: vespa-fbench: Seconds left 240
[dummydate]: PROGRESS: vespa-fbench: Seconds left 180
[dummydate]: PROGRESS: vespa-fbench: Seconds left 120
[dummydate]: PROGRESS: vespa-fbench: Seconds left 60
Stopping clients
Clients stopped.
..........
Clients Joined.
*** HTTP keep-alive statistics ***
connection reuse count -- 993969
***************** Benchmark Summary *****************
clients:                      10
ran for:                     300 seconds
cycle time:                    0 ms
lower response limit:          0 bytes
skipped requests:              0
failed requests:               0
successful requests:      993979
cycles not held:          993979
minimum response time:      1.21 ms
maximum response time:     26.76 ms
average response time:      3.00 ms
25 percentile:              2.40 ms
50 percentile:              3.00 ms
75 percentile:              3.50 ms
90 percentile:              3.90 ms
95 percentile:              4.10 ms
99 percentile:              4.50 ms
actual query rate:       3317.85 Q/s
utilization:               99.48 %
zero hit queries:         397589
http request status breakdown:
       200 :   993979
```
