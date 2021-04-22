
# client -n 20 vespa 7.1
```
date; LD_LIBRARY_PATH=/tmp/tem_vespa_lib64/ vespa-fbench -n 20 -c 0 -s 300 localhost 4080 -q search_query2.txt -o res
Thu Apr 22 15:18:44 JST 2021
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
connection reuse count -- 1516422
***************** Benchmark Summary *****************
clients:                      20
ran for:                     300 seconds
cycle time:                    0 ms
lower response limit:          0 bytes
skipped requests:              0
failed requests:               0
successful requests:     1516442
cycles not held:         1516442
minimum response time:      1.32 ms
maximum response time:     35.54 ms
average response time:      3.93 ms
25 percentile:              3.30 ms
50 percentile:              3.90 ms
75 percentile:              4.50 ms
90 percentile:              5.00 ms
95 percentile:              5.40 ms
99 percentile:              6.60 ms
actual query rate:       5062.51 Q/s
utilization:               99.59 %
zero hit queries:         606573
http request status breakdown:
       200 :  1516351
       504 :       91


{
    "metrics": {
        "snapshot": {
            "from": 1.619072349805E9,
            "to": 1.619072409805E9
        },
        "values": [
            {
                "name": "search_connections",
                "values": {
                    "average": 17.518028235434773,
                    "count": 1,
                    "last": 17.518028235434773,
                    "max": 17.518028235434773,
                    "min": 17.518028235434773,
                    "rate": 0.016666666666666666,
                    "sum": 17.518028235434773
                }
            },
            {
                "name": "jrt.transport.client.unencrypted-connections-established",
                "values": {
                    "count": 0,
                    "rate": 0
                }
            },
            {
                "name": "serverThreadPoolSize",
                "values": {
                    "average": 500,
                    "count": 599,
                    "last": 500,
                    "max": 500,
                    "min": 500,
                    "rate": 9.983333333333333,
                    "sum": 299500
                }
            },
            {
                "name": "serverActiveThreads",
                "values": {
                    "average": 17.68948247078464,
                    "count": 599,
                    "last": 16,
                    "max": 20,
                    "min": 7,
                    "rate": 9.983333333333333,
                    "sum": 10596
                }
            },
            {
                "name": "jdisc.open_file_descriptors",
                "values": {
                    "average": 630,
                    "count": 6,
                    "last": 630,
                    "max": 630,
                    "min": 630,
                    "rate": 0.1,
                    "sum": 3780
                }
            },
            {
                "name": "mem.heap.total",
                "values": {
                    "average": 1.610612736E9,
                    "count": 6,
                    "last": 1.610612736E9,
                    "max": 1.610612736E9,
                    "min": 1.610612736E9,
                    "rate": 0.1,
                    "sum": 9.663676416E9
                }
            },
            {
                "name": "serverStartedMillis",
                "values": {
                    "average": 1.08447092E8,
                    "count": 30,
                    "last": 1.08418092E8,
                    "max": 1.08476092E8,
                    "min": 1.08418092E8,
                    "rate": 0.5,
                    "sum": 3.25341276E9
                }
            },
            {
                "name": "chain_indexing_documents",
                "values": {
                    "count": 1515,
                    "rate": 25.25
                }
            },
            {
                "name": "jdisc.deactivated_containers.total",
                "values": {
                    "average": 0,
                    "count": 6,
                    "last": 0,
                    "max": 0,
                    "min": 0,
                    "rate": 0.1,
                    "sum": 0
                }
            },
            {
                "name": "docprocessor_indexing_com_yahoo_docprocs_indexing_IndexingProcessor_indexing_documents",
                "values": {
                    "count": 1515,
                    "rate": 25.25
                }
            },
            {
                "name": "jdisc.memory_mappings",
                "values": {
                    "average": 2047,
                    "count": 6,
                    "last": 2047,
                    "max": 2047,
                    "min": 2047,
                    "rate": 0.1,
                    "sum": 12282
                }
            },
            {
                "name": "dispatch_fdispatch",
                "values": {
                    "count": 301946,
                    "rate": 5032.433333333333
                }
            },
            {
                "name": "mem.heap.used",
                "values": {
                    "average": 1.0991862106666667E9,
                    "count": 6,
                    "last": 1.194947144E9,
                    "max": 1.417755264E9,
                    "min": 9.00875136E8,
                    "rate": 0.1,
                    "sum": 6.595117264E9
                }
            },
            {
                "name": "docprocessor_indexing_com_yahoo_docprocs_indexing_IndexingProcessor_indexing_proctime",
                "values": {
                    "count": 313,
                    "rate": 5.216666666666667
                }
            },
            {
                "name": "mem.heap.free",
                "values": {
                    "average": 5.114265253333333E8,
                    "count": 6,
                    "last": 4.15665592E8,
                    "max": 7.097376E8,
                    "min": 1.92857472E8,
                    "rate": 0.1,
                    "sum": 3.068559152E9
                }
            },
            {
                "name": "jdisc.http.requests.status",
                "values": {
                    "count": 8,
                    "rate": 0.13333333333333333
                }
            },
            {
                "dimensions": {
                    "httpMethod": "GET",
                    "scheme": "http",
                    "serverName": "myserver",
                    "serverPort": "4080"
                },
                "name": "serverNumRequests",
                "values": {
                    "count": 301953,
                    "rate": 5032.55
                }
            },
            {
                "dimensions": {
                    "httpMethod": "GET",
                    "scheme": "http",
                    "serverName": "myserver",
                    "serverPort": "4080"
                },
                "name": "serverTimeToFirstByte",
                "values": {
                    "average": 3.8031673908435777,
                    "count": 301952,
                    "last": 5,
                    "max": 32,
                    "min": 0,
                    "rate": 5032.533333333334,
                    "sum": 1148374
                }
            },
            {
                "dimensions": {
                    "httpMethod": "GET",
                    "scheme": "http",
                    "serverName": "myserver",
                    "serverPort": "4080"
                },
                "name": "serverBytesSent",
                "values": {
                    "average": 4609.06773320876,
                    "count": 573692,
                    "last": 5885,
                    "max": 25299,
                    "min": 18,
                    "rate": 9561.533333333333,
                    "sum": 2.644185286E9
                }
            },
            {
                "dimensions": {
                    "httpMethod": "GET",
                    "scheme": "http",
                    "serverName": "myserver",
                    "serverPort": "4080"
                },
                "name": "serverNumSuccessfulResponseWrites",
                "values": {
                    "count": 573692,
                    "rate": 9561.533333333333
                }
            },
            {
                "dimensions": {
                    "httpMethod": "GET",
                    "scheme": "http",
                    "serverName": "myserver",
                    "serverPort": "4080"
                },
                "name": "jdisc.http.request.uri_length",
                "values": {
                    "average": 404.28199752941686,
                    "count": 301953,
                    "last": 408,
                    "max": 408,
                    "min": 12,
                    "rate": 5032.55,
                    "sum": 1.22074162E8
                }
            },
            {
                "dimensions": {
                    "httpMethod": "GET",
                    "scheme": "http",
                    "serverName": "myserver",
                    "serverPort": "4080"
                },
                "name": "serverTotalFailedResponseLatency",
                "values": {
                    "average": 3,
                    "count": 0,
                    "last": 3,
                    "max": 3,
                    "min": 3,
                    "rate": 0,
                    "sum": 0
                }
            },
            {
                "dimensions": {
                    "httpMethod": "GET",
                    "scheme": "http",
                    "serverName": "myserver",
                    "serverPort": "4080"
                },
                "name": "serverTotalSuccessfulResponseLatency",
                "values": {
                    "average": 3.860282428995337,
                    "count": 301952,
                    "last": 5,
                    "max": 32,
                    "min": 0,
                    "rate": 5032.533333333334,
                    "sum": 1165620
                }
            },
            {
                "dimensions": {
                    "httpMethod": "GET",
                    "scheme": "http",
                    "serverName": "myserver",
                    "serverPort": "4080"
                },
                "name": "jdisc.http.requests",
                "values": {
                    "count": 301953,
                    "rate": 5032.55
                }
            },
            {
                "dimensions": {
                    "httpMethod": "GET",
                    "scheme": "http",
                    "serverName": "myserver",
                    "serverPort": "4080"
                },
                "name": "serverNumSuccessfulResponses",
                "values": {
                    "count": 301952,
                    "rate": 5032.533333333334
                }
            },
            {
                "dimensions": {
                    "httpMethod": "GET",
                    "scheme": "http",
                    "serverName": "myserver",
                    "serverPort": "4080"
                },
                "name": "jdisc.http.request.content_size",
                "values": {
                    "average": 0,
                    "count": 301955,
                    "last": 0,
                    "max": 0,
                    "min": 0,
                    "rate": 5032.583333333333,
                    "sum": 0
                }
            },
            {
                "dimensions": {
                    "httpMethod": "GET",
                    "scheme": "http",
                    "serverName": "myserver",
                    "serverPort": "4080"
                },
                "name": "serverNumFailedResponses",
                "values": {
                    "count": 0,
                    "rate": 0
                }
            },
            {
                "dimensions": {"gcName": "G1YoungGeneration"},
                "name": "jdisc.gc.ms",
                "values": {
                    "average": 385.6666666666667,
                    "count": 6,
                    "last": 475,
                    "max": 475,
                    "min": 222,
                    "rate": 0.1,
                    "sum": 2314
                }
            },
            {
                "dimensions": {"gcName": "G1YoungGeneration"},
                "name": "jdisc.gc.count",
                "values": {
                    "average": 121.33333333333333,
                    "count": 6,
                    "last": 148,
                    "max": 148,
                    "min": 71,
                    "rate": 0.1,
                    "sum": 728
                }
            },
            {
                "dimensions": {"chain": "indexing"},
                "name": "documents_processed",
                "values": {
                    "count": 1515,
                    "rate": 25.25
                }
            },
            {
                "dimensions": {"gcName": "G1OldGeneration"},
                "name": "jdisc.gc.ms",
                "values": {
                    "average": 0,
                    "count": 6,
                    "last": 0,
                    "max": 0,
                    "min": 0,
                    "rate": 0.1,
                    "sum": 0
                }
            },
            {
                "dimensions": {"gcName": "G1OldGeneration"},
                "name": "jdisc.gc.count",
                "values": {
                    "average": 0,
                    "count": 6,
                    "last": 0,
                    "max": 0,
                    "min": 0,
                    "rate": 0.1,
                    "sum": 0
                }
            },
            {
                "dimensions": {"handler": "http://*:*/search/*"},
                "name": "handled.latency",
                "values": {
                    "average": 3.7383560146653108,
                    "count": 301937,
                    "last": 6,
                    "max": 31,
                    "min": 1,
                    "rate": 5032.283333333334,
                    "sum": 1128748
                }
            },
            {
                "dimensions": {"handler": "http://*:*/search/*"},
                "name": "handled.requests",
                "values": {
                    "count": 301940,
                    "rate": 5032.333333333333
                }
            },
            {
                "dimensions": {"handler": "http://*:*/status.html"},
                "name": "handled.latency",
                "values": {
                    "average": 0.25,
                    "count": 8,
                    "last": 0,
                    "max": 1,
                    "min": 0,
                    "rate": 0.13333333333333333,
                    "sum": 2
                }
            },
            {
                "dimensions": {"handler": "http://*:*/status.html"},
                "name": "handled.requests",
                "values": {
                    "count": 8,
                    "rate": 0.13333333333333333
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "rankProfile": "<OurProductID>"
                },
                "name": "relevance.at_10",
                "values": {
                    "average": 3515579.3611487783,
                    "count": 181163,
                    "last": 6964334.118567502,
                    "max": 6964334.4999970235,
                    "min": 66710.00000724499,
                    "rate": 3019.383333333333,
                    "sum": 6.368929038037961E11
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "rankProfile": "<OurProductID>"
                },
                "name": "relevance.at_1",
                "values": {
                    "average": 9.740310942845309E8,
                    "count": 181163,
                    "last": 1.934000000450011E9,
                    "max": 1.9340000004999979E9,
                    "min": 1.4030394000001779E7,
                    "rate": 3019.383333333333,
                    "sum": 1.7645839513386847E14
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "rankProfile": "<OurProductID>"
                },
                "name": "relevance.at_3",
                "values": {
                    "average": 1.1251405845421325E7,
                    "count": 181163,
                    "last": 2.236578938718591E7,
                    "max": 2.2365789499997623E7,
                    "min": 136654.00001597614,
                    "rate": 3019.383333333333,
                    "sum": 2.0383384371740635E12
                }
            },
            {
                "dimensions": {
                    "serverName": "myserver",
                    "serverPort": "4080"
                },
                "name": "serverConnectionDurationMean",
                "values": {
                    "average": 258.3864511303445,
                    "count": 30,
                    "last": 258.1328037577398,
                    "max": 258.3951975914689,
                    "min": 258.1328037577398,
                    "rate": 0.5,
                    "sum": 7751.593533910335
                }
            },
            {
                "dimensions": {
                    "serverName": "myserver",
                    "serverPort": "4080"
                },
                "name": "serverConnectionDurationMax",
                "values": {
                    "average": 1.4554441E7,
                    "count": 30,
                    "last": 1.4554441E7,
                    "max": 1.4554441E7,
                    "min": 1.4554441E7,
                    "rate": 0.5,
                    "sum": 4.3663323E8
                }
            },
            {
                "dimensions": {
                    "serverName": "myserver",
                    "serverPort": "4080"
                },
                "name": "serverConnectionsOpenMax",
                "values": {
                    "average": 377,
                    "count": 30,
                    "last": 377,
                    "max": 377,
                    "min": 377,
                    "rate": 0.5,
                    "sum": 11310
                }
            },
            {
                "dimensions": {
                    "serverName": "myserver",
                    "serverPort": "4080"
                },
                "name": "serverNumConnections",
                "values": {
                    "average": 750687.0666666667,
                    "count": 30,
                    "last": 750687,
                    "max": 750689,
                    "min": 750687,
                    "rate": 0.5,
                    "sum": 2.2520612E7
                }
            },
            {
                "dimensions": {
                    "serverName": "myserver",
                    "serverPort": "4080"
                },
                "name": "serverNumOpenConnections",
                "values": {
                    "average": 22.1,
                    "count": 30,
                    "last": 23,
                    "max": 24,
                    "min": 22,
                    "rate": 0.5,
                    "sum": 663
                }
            },
            {
                "dimensions": {
                    "serverName": "myserver",
                    "serverPort": "4080"
                },
                "name": "serverConnectionDurationStdDev",
                "values": {
                    "average": 17515.625366938613,
                    "count": 30,
                    "last": 17514.210407744853,
                    "max": 17515.674158634945,
                    "min": 17514.210407744853,
                    "rate": 0.5,
                    "sum": 525468.7610081584
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "endpoint": "localhost:4080"
                },
                "name": "query_latency",
                "values": {
                    "95percentile": 4.0234375,
                    "99percentile": 5.0234375,
                    "average": 2.8360944041121297,
                    "count": 301936,
                    "last": 3,
                    "max": 24,
                    "min": 1,
                    "rate": 5032.266666666666,
                    "sum": 856319
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "endpoint": "localhost:4080"
                },
                "name": "documents_covered",
                "values": {
                    "count": 26925165404383,
                    "rate": 4.487527567397167E11
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "endpoint": "localhost:4080"
                },
                "name": "documents_total",
                "values": {
                    "count": 26925165404383,
                    "rate": 4.487527567397167E11
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "endpoint": "localhost:4080"
                },
                "name": "empty_results",
                "values": {
                    "count": 120773,
                    "rate": 2012.8833333333334
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "endpoint": "localhost:4080"
                },
                "name": "max_query_latency",
                "values": {
                    "average": 2.8360944041121297,
                    "count": 301936,
                    "last": 3,
                    "max": 24,
                    "min": 1,
                    "rate": 5032.266666666666,
                    "sum": 856319
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "endpoint": "localhost:4080"
                },
                "name": "hits_per_query",
                "values": {
                    "average": 7.200055640930528,
                    "count": 301936,
                    "last": 12,
                    "max": 12,
                    "min": 0,
                    "rate": 5032.266666666666,
                    "sum": 2173956
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "endpoint": "localhost:4080"
                },
                "name": "totalhits_per_query",
                "values": {
                    "average": 87.60077632345927,
                    "count": 301936,
                    "last": 156,
                    "max": 156,
                    "min": 0,
                    "rate": 5032.266666666666,
                    "sum": 2.6449828E7
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "endpoint": "localhost:4080"
                },
                "name": "queries",
                "values": {
                    "count": 301945,
                    "rate": 5032.416666666667
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "endpoint": "localhost:4080"
                },
                "name": "mean_query_latency",
                "values": {
                    "average": 2.8360944041121297,
                    "count": 301936,
                    "last": 3,
                    "max": 24,
                    "min": 1,
                    "rate": 5032.266666666666,
                    "sum": 856319
                }
            },
            {
                "dimensions": {"chain": "<OurProductID>"},
                "name": "query_container_latency",
                "values": {
                    "average": 0.09849443277937114,
                    "count": 301946,
                    "last": 0,
                    "max": 6,
                    "min": 0,
                    "rate": 5032.433333333333,
                    "sum": 29740
                }
            },
            {
                "dimensions": {
                    "httpMethod": "GET",
                    "scheme": "http"
                },
                "name": "http.status.2xx",
                "values": {
                    "count": 301624,
                    "rate": 5027.066666666667
                }
            },
            {
                "dimensions": {
                    "httpMethod": "GET",
                    "scheme": "http"
                },
                "name": "http.status.4xx",
                "values": {
                    "count": 0,
                    "rate": 0
                }
            },
            {
                "dimensions": {
                    "httpMethod": "GET",
                    "scheme": "http"
                },
                "name": "http.status.5xx",
                "values": {
                    "count": 42,
                    "rate": 0.7
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "endpoint": "0.0.0.0:4080"
                },
                "name": "peak_qps",
                "values": {
                    "average": 5028.015578140704,
                    "count": 60,
                    "last": 4653,
                    "max": 5287,
                    "min": 4653,
                    "rate": 1,
                    "sum": 301680.9346884422
                }
            }
        ]
    },
    "status": {"code": "up"},
    "time": 1619072410593
}

```
