vespa 7.3
```
First time
$ date; LD_LIBRARY_PATH=/opt/vespa/lib64 vespa-fbench -n 20 -c 0 -s 300 localhost 4080 -q search_query2.txt -o res
Wed Apr 21 11:53:01 JST 2021
Starting clients...
[dummydate]: PROGRESS: vespa-fbench: Seconds left 300
[dummydate]: PROGRESS: vespa-fbench: Seconds left 240
[dummydate]: PROGRESS: vespa-fbench: Seconds left 180
[dummydate]: PROGRESS: vespa-fbench: Seconds left 120
[dummydate]: PROGRESS: vespa-fbench: Seconds left 60
Stopping clients
Clients stopped.
....................
Clients Joined.
*** HTTP keep-alive statistics ***
connection reuse count -- 1061065
***************** Benchmark Summary *****************
clients:                      20
ran for:                     300 seconds
cycle time:                    0 ms
lower response limit:          0 bytes
skipped requests:              0
failed requests:               0
successful requests:     1061085
cycles not held:         1061085
minimum response time:      1.18 ms
maximum response time:     42.06 ms
average response time:      5.64 ms
25   percentile:              4.10 ms
50   percentile:              5.20 ms
75   percentile:              6.70 ms
90   percentile:              7.70 ms
95   percentile:              8.30 ms
98   percentile:              9.90 ms
99   percentile:             17.50 ms
99.5 percentile:             30.40 ms
99.6 percentile:             30.60 ms
99.7 percentile:             30.80 ms
99.8 percentile:             30.90 ms
99.9 percentile:             31.20 ms
actual query rate:       3541.99 Q/s
utilization:               99.83 %
zero hit queries:         424134
http request status breakdown:
       200 :  1055908
       504 :     5177
       
Second time
$ date; LD_LIBRARY_PATH=/opt/vespa/lib64 vespa-fbench -n 20 -c 0 -s 300 localhost 4080 -q search_query2.txt -o res
Wed Apr 21 12:19:16 JST 2021
Starting clients...
[dummydate]: PROGRESS: vespa-fbench: Seconds left 300
[dummydate]: PROGRESS: vespa-fbench: Seconds left 240
[dummydate]: PROGRESS: vespa-fbench: Seconds left 180
[dummydate]: PROGRESS: vespa-fbench: Seconds left 120
[dummydate]: PROGRESS: vespa-fbench: Seconds left 60
Stopping clients
Clients stopped.
....................
Clients Joined.
*** HTTP keep-alive statistics ***
connection reuse count -- 1062662
***************** Benchmark Summary *****************
clients:                      20
ran for:                     300 seconds
cycle time:                    0 ms
lower response limit:          0 bytes
skipped requests:              0
failed requests:               0
successful requests:     1062682
cycles not held:         1062682
minimum response time:      1.17 ms
maximum response time:     41.10 ms
average response time:      5.63 ms
25   percentile:              4.10 ms
50   percentile:              5.20 ms
75   percentile:              6.70 ms
90   percentile:              7.70 ms
95   percentile:              8.30 ms
98   percentile:              9.90 ms
99   percentile:             17.00 ms
99.5 percentile:             30.30 ms
99.6 percentile:             30.50 ms
99.7 percentile:             30.70 ms
99.8 percentile:             30.90 ms
99.9 percentile:             31.20 ms
actual query rate:       3546.65 Q/s
utilization:               99.83 %
zero hit queries:         424760
http request status breakdown:
       200 :  1057610
       504 :     5072
       

Third time

$ date; LD_LIBRARY_PATH=/opt/vespa/lib64 vespa-fbench -n 20 -c 0 -s 300 localhost 4080 -q search_query2.txt -o res
Wed Apr 21 12:37:45 JST 2021
Starting clients...
[dummydate]: PROGRESS: vespa-fbench: Seconds left 300
[dummydate]: PROGRESS: vespa-fbench: Seconds left 240
[dummydate]: PROGRESS: vespa-fbench: Seconds left 180
[dummydate]: PROGRESS: vespa-fbench: Seconds left 120
[dummydate]: PROGRESS: vespa-fbench: Seconds left 60
Stopping clients
Clients stopped.
....................
Clients Joined.
*** HTTP keep-alive statistics ***
connection reuse count -- 1062030
***************** Benchmark Summary *****************
clients:                      20
ran for:                     300 seconds
cycle time:                    0 ms
lower response limit:          0 bytes
skipped requests:              0
failed requests:               0
successful requests:     1062050
cycles not held:         1062050
minimum response time:      1.15 ms
maximum response time:     44.98 ms
average response time:      5.63 ms
25   percentile:              4.10 ms
50   percentile:              5.20 ms
75   percentile:              6.70 ms
90   percentile:              7.70 ms
95   percentile:              8.30 ms
98   percentile:              9.70 ms
99   percentile:             17.70 ms
99.5 percentile:             30.40 ms
99.6 percentile:             30.60 ms
99.7 percentile:             30.80 ms
99.8 percentile:             31.00 ms
99.9 percentile:             31.20 ms
actual query rate:       3544.64 Q/s
utilization:               99.84 %
zero hit queries:         424494
http request status breakdown:
       200 :  1056606
       504 :     5444
```

vespa 7.1
```
First time
$ date; LD_LIBRARY_PATH=/opt/vespa/lib64 vespa-fbench -n 20 -c 0 -s 300 localhost 4080 -q search_query2.txt -o res
Wed Apr 21 11:52:57 JST 2021
Starting clients...
[dummydate]: PROGRESS: vespa-fbench: Seconds left 300
[dummydate]: PROGRESS: vespa-fbench: Seconds left 240
[dummydate]: PROGRESS: vespa-fbench: Seconds left 180
[dummydate]: PROGRESS: vespa-fbench: Seconds left 120
[dummydate]: PROGRESS: vespa-fbench: Seconds left 60
Stopping clients
Clients stopped.
....................
Clients Joined.
*** HTTP keep-alive statistics ***
connection reuse count -- 1497346
***************** Benchmark Summary *****************
clients:                      20
ran for:                     300 seconds
cycle time:                    0 ms
lower response limit:          0 bytes
skipped requests:              0
failed requests:               0
successful requests:     1497366
cycles not held:         1497366
minimum response time:      1.31 ms
maximum response time:     35.94 ms
average response time:      3.98 ms
25 percentile:              3.30 ms
50 percentile:              3.90 ms
75 percentile:              4.50 ms
90 percentile:              5.10 ms
95 percentile:              5.50 ms
99 percentile:              6.60 ms
actual query rate:       4998.63 Q/s
utilization:               99.56 %
zero hit queries:         598943
http request status breakdown:
       200 :  1496955
       504 :      411
 

Second time

$ date; LD_LIBRARY_PATH=/opt/vespa/lib64 vespa-fbench -n 20 -c 0 -s 300 localhost 4080 -q search_query2.txt -o res
Wed Apr 21 12:19:17 JST 2021
Starting clients...
[dummydate]: PROGRESS: vespa-fbench: Seconds left 300
[dummydate]: PROGRESS: vespa-fbench: Seconds left 240
[dummydate]: PROGRESS: vespa-fbench: Seconds left 180
[dummydate]: PROGRESS: vespa-fbench: Seconds left 120
[dummydate]: PROGRESS: vespa-fbench: Seconds left 60
Stopping clients
Clients stopped.
....................
Clients Joined.
*** HTTP keep-alive statistics ***
connection reuse count -- 1499275
***************** Benchmark Summary *****************
clients:                      20
ran for:                     300 seconds
cycle time:                    0 ms
lower response limit:          0 bytes
skipped requests:              0
failed requests:               0
successful requests:     1499295
cycles not held:         1499295
minimum response time:      1.27 ms
maximum response time:     35.89 ms
average response time:      3.98 ms
25 percentile:              3.30 ms
50 percentile:              3.90 ms
75 percentile:              4.50 ms
90 percentile:              5.10 ms
95 percentile:              5.50 ms
99 percentile:              6.60 ms
actual query rate:       5004.53 Q/s
utilization:               99.56 %
zero hit queries:         599712
http request status breakdown:
       200 :  1498850
       504 :      445


Third time

$ date; LD_LIBRARY_PATH=/opt/vespa/lib64 vespa-fbench -n 20 -c 0 -s 300 localhost 4080 -q search_query2.txt -o res
Wed Apr 21 12:37:47 JST 2021
Starting clients...
[dummydate]: PROGRESS: vespa-fbench: Seconds left 300
[dummydate]: PROGRESS: vespa-fbench: Seconds left 240
[dummydate]: PROGRESS: vespa-fbench: Seconds left 180
[dummydate]: PROGRESS: vespa-fbench: Seconds left 120
[dummydate]: PROGRESS: vespa-fbench: Seconds left 60
Stopping clients
Clients stopped.
....................
Clients Joined.
*** HTTP keep-alive statistics ***
connection reuse count -- 1500574
***************** Benchmark Summary *****************
clients:                      20
ran for:                     300 seconds
cycle time:                    0 ms
lower response limit:          0 bytes
skipped requests:              0
failed requests:               0
successful requests:     1500594
cycles not held:         1500594
minimum response time:      1.27 ms
maximum response time:     36.14 ms
average response time:      3.98 ms
25 percentile:              3.30 ms
50 percentile:              3.90 ms
75 percentile:              4.50 ms
90 percentile:              5.10 ms
95 percentile:              5.50 ms
99 percentile:              6.60 ms
actual query rate:       5008.89 Q/s
utilization:               99.56 %
zero hit queries:         600231
http request status breakdown:
       200 :  1500271
       504 :      323
```
