

# client -n 10 vespa 7.1
```
[<OurHost> ~]date; LD_LIBRARY_PATH=/tmp/tem_vespa_lib64/ vespa-fbench -n 10 -c 0 -s 300 localhost 4080 -q search_query2.txt -o res
Thu Apr 22 15:12:50 JST 2021
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
connection reuse count -- 986374
***************** Benchmark Summary *****************
clients:                      10
ran for:                     300 seconds
cycle time:                    0 ms
lower response limit:          0 bytes
skipped requests:              0
failed requests:               0
successful requests:      986384
cycles not held:          986384
minimum response time:      1.26 ms
maximum response time:     31.28 ms
average response time:      3.02 ms
25 percentile:              2.50 ms
50 percentile:              3.00 ms
75 percentile:              3.50 ms
90 percentile:              3.90 ms
95 percentile:              4.10 ms
99 percentile:              4.50 ms
actual query rate:       3292.90 Q/s
utilization:               99.48 %
zero hit queries:         394552
http request status breakdown:
       200 :   986376
       504 :        8
[<OurHost> ~]


http://<OurHost>:4080/state/v1/metrics
{
    "metrics": {
        "snapshot": {
            "from": 1.619072095805E9,
            "to": 1.619072155805E9
        },
        "values": [
            {
                "name": "search_connections",
                "values": {
                    "average": 8.042322446129088,
                    "count": 1,
                    "last": 8.042322446129088,
                    "max": 8.042322446129088,
                    "min": 8.042322446129088,
                    "rate": 0.016666666666666666,
                    "sum": 8.042322446129088
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
                    "count": 600,
                    "last": 500,
                    "max": 500,
                    "min": 500,
                    "rate": 10,
                    "sum": 300000
                }
            },
            {
                "name": "serverActiveThreads",
                "values": {
                    "average": 8.52,
                    "count": 600,
                    "last": 10,
                    "max": 10,
                    "min": 0,
                    "rate": 10,
                    "sum": 5112
                }
            },
            {
                "name": "jdisc.open_file_descriptors",
                "values": {
                    "average": 620.3333333333334,
                    "count": 6,
                    "last": 620,
                    "max": 622,
                    "min": 620,
                    "rate": 0.1,
                    "sum": 3722
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
                    "average": 1.08193092E8,
                    "count": 30,
                    "last": 1.08178092E8,
                    "max": 1.08222092E8,
                    "min": 1.08164092E8,
                    "rate": 0.5,
                    "sum": 3.24579276E9
                }
            },
            {
                "name": "chain_indexing_documents",
                "values": {
                    "count": 1474,
                    "rate": 24.566666666666666
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
                    "count": 1474,
                    "rate": 24.566666666666666
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
                    "count": 198668,
                    "rate": 3311.133333333333
                }
            },
            {
                "name": "mem.heap.used",
                "values": {
                    "average": 1.144234224E9,
                    "count": 6,
                    "last": 1.06649552E9,
                    "max": 1.224724696E9,
                    "min": 1.06649552E9,
                    "rate": 0.1,
                    "sum": 6.865405344E9
                }
            },
            {
                "name": "docprocessor_indexing_com_yahoo_docprocs_indexing_IndexingProcessor_indexing_proctime",
                "values": {
                    "count": 258,
                    "rate": 4.3
                }
            },
            {
                "name": "mem.heap.free",
                "values": {
                    "average": 4.66378512E8,
                    "count": 6,
                    "last": 5.44117216E8,
                    "max": 5.44117216E8,
                    "min": 3.8588804E8,
                    "rate": 0.1,
                    "sum": 2.798271072E9
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
                    "count": 198682,
                    "rate": 3311.366666666667
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
                    "average": 2.856650325646007,
                    "count": 198682,
                    "last": 3,
                    "max": 25,
                    "min": 0,
                    "rate": 3311.366666666667,
                    "sum": 567565
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
                    "average": 4609.23478097317,
                    "count": 377488,
                    "last": 5506,
                    "max": 24666,
                    "min": 18,
                    "rate": 6291.466666666666,
                    "sum": 1.739930819E9
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
                    "count": 377488,
                    "rate": 6291.466666666666
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
                    "average": 404.2724806474668,
                    "count": 198682,
                    "last": 397,
                    "max": 408,
                    "min": 12,
                    "rate": 3311.366666666667,
                    "sum": 8.0321665E7
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
                    "count": 1,
                    "last": 3,
                    "max": 3,
                    "min": 3,
                    "rate": 0.016666666666666666,
                    "sum": 3
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
                    "average": 2.912120434263971,
                    "count": 198681,
                    "last": 3,
                    "max": 25,
                    "min": 0,
                    "rate": 3311.35,
                    "sum": 578583
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
                    "count": 198682,
                    "rate": 3311.366666666667
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
                    "count": 198681,
                    "rate": 3311.35
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
                    "count": 198681,
                    "last": 0,
                    "max": 0,
                    "min": 0,
                    "rate": 3311.35,
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
                    "count": 1,
                    "rate": 0.016666666666666666
                }
            },
            {
                "dimensions": {"gcName": "G1YoungGeneration"},
                "name": "jdisc.gc.ms",
                "values": {
                    "average": 294.3333333333333,
                    "count": 6,
                    "last": 295,
                    "max": 297,
                    "min": 293,
                    "rate": 0.1,
                    "sum": 1766
                }
            },
            {
                "dimensions": {"gcName": "G1YoungGeneration"},
                "name": "jdisc.gc.count",
                "values": {
                    "average": 95.5,
                    "count": 6,
                    "last": 95,
                    "max": 96,
                    "min": 95,
                    "rate": 0.1,
                    "sum": 573
                }
            },
            {
                "dimensions": {"chain": "indexing"},
                "name": "documents_processed",
                "values": {
                    "count": 1474,
                    "rate": 24.566666666666666
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
                    "average": 2.7942396359755977,
                    "count": 198668,
                    "last": 1,
                    "max": 25,
                    "min": 1,
                    "rate": 3311.133333333333,
                    "sum": 555126
                }
            },
            {
                "dimensions": {"handler": "http://*:*/search/*"},
                "name": "handled.requests",
                "values": {
                    "count": 198668,
                    "rate": 3311.133333333333
                }
            },
            {
                "dimensions": {"handler": "http://*:*/status.html"},
                "name": "handled.latency",
                "values": {
                    "average": 0,
                    "count": 8,
                    "last": 0,
                    "max": 0,
                    "min": 0,
                    "rate": 0.13333333333333333,
                    "sum": 0
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
                    "average": 3515348.6436768696,
                    "count": 119194,
                    "last": 66710.00294997357,
                    "max": 6964334.4999956675,
                    "min": 66710.00001418497,
                    "rate": 1986.5666666666666,
                    "sum": 4.190084662344208E11
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "rankProfile": "<OurProductID>"
                },
                "name": "relevance.at_1",
                "values": {
                    "average": 9.739668734341794E8,
                    "count": 119194,
                    "last": 1.4030394255812163E7,
                    "max": 1.9340000004999933E9,
                    "min": 1.403039400000658E7,
                    "rate": 1986.5666666666666,
                    "sum": 1.1609100751211358E14
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "rankProfile": "<OurProductID>"
                },
                "name": "relevance.at_3",
                "values": {
                    "average": 1.1250662305290144E7,
                    "count": 119194,
                    "last": 136654.1201416012,
                    "max": 2.2365789499984737E7,
                    "min": 136654.00000429316,
                    "rate": 1986.5666666666666,
                    "sum": 1.3410114428167534E12
                }
            },
            {
                "dimensions": {
                    "serverName": "myserver",
                    "serverPort": "4080"
                },
                "name": "serverConnectionDurationMean",
                "values": {
                    "average": 254.0134189832052,
                    "count": 30,
                    "last": 254.0134189832053,
                    "max": 254.0134189832053,
                    "min": 254.0134189832053,
                    "rate": 0.5,
                    "sum": 7620.4025694961565
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
                    "average": 750665.0666666667,
                    "count": 30,
                    "last": 750665,
                    "max": 750667,
                    "min": 750665,
                    "rate": 0.5,
                    "sum": 2.2519952E7
                }
            },
            {
                "dimensions": {
                    "serverName": "myserver",
                    "serverPort": "4080"
                },
                "name": "serverNumOpenConnections",
                "values": {
                    "average": 12.066666666666666,
                    "count": 30,
                    "last": 12,
                    "max": 14,
                    "min": 12,
                    "rate": 0.5,
                    "sum": 362
                }
            },
            {
                "dimensions": {
                    "serverName": "myserver",
                    "serverPort": "4080"
                },
                "name": "serverConnectionDurationStdDev",
                "values": {
                    "average": 17479.862445190593,
                    "count": 30,
                    "last": 17479.862445190585,
                    "max": 17479.862445190585,
                    "min": 17479.862445190585,
                    "rate": 0.5,
                    "sum": 524395.8733557177
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "endpoint": "localhost:4080"
                },
                "name": "query_latency",
                "values": {
                    "95percentile": 3.0078125,
                    "99percentile": 3.0078125,
                    "average": 2.02786195370939,
                    "count": 198658,
                    "last": 2,
                    "max": 16,
                    "min": 0,
                    "rate": 3310.9666666666667,
                    "sum": 402851
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "endpoint": "localhost:4080"
                },
                "name": "documents_covered",
                "values": {
                    "count": 17723874128361,
                    "rate": 2.9539790213935E11
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "endpoint": "localhost:4080"
                },
                "name": "documents_total",
                "values": {
                    "count": 17723874128361,
                    "rate": 2.9539790213935E11
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "endpoint": "localhost:4080"
                },
                "name": "empty_results",
                "values": {
                    "count": 79464,
                    "rate": 1324.4
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "endpoint": "localhost:4080"
                },
                "name": "max_query_latency",
                "values": {
                    "average": 2.02786195370939,
                    "count": 198658,
                    "last": 2,
                    "max": 16,
                    "min": 0,
                    "rate": 3310.9666666666667,
                    "sum": 402851
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "endpoint": "localhost:4080"
                },
                "name": "hits_per_query",
                "values": {
                    "average": 7.199951675744244,
                    "count": 198658,
                    "last": 0,
                    "max": 12,
                    "min": 0,
                    "rate": 3310.9666666666667,
                    "sum": 1430328
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "endpoint": "localhost:4080"
                },
                "name": "totalhits_per_query",
                "values": {
                    "average": 87.59911002828983,
                    "count": 198658,
                    "last": 0,
                    "max": 156,
                    "min": 0,
                    "rate": 3310.9666666666667,
                    "sum": 1.7402264E7
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "endpoint": "localhost:4080"
                },
                "name": "queries",
                "values": {
                    "count": 198668,
                    "rate": 3311.133333333333
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "endpoint": "localhost:4080"
                },
                "name": "mean_query_latency",
                "values": {
                    "average": 2.02786195370939,
                    "count": 198658,
                    "last": 2,
                    "max": 16,
                    "min": 0,
                    "rate": 3310.9666666666667,
                    "sum": 402851
                }
            },
            {
                "dimensions": {"chain": "<OurProductID>"},
                "name": "query_container_latency",
                "values": {
                    "average": 0.0867880081341736,
                    "count": 198668,
                    "last": 0,
                    "max": 5,
                    "min": 0,
                    "rate": 3311.133333333333,
                    "sum": 17242
                }
            },
            {
                "dimensions": {
                    "httpMethod": "GET",
                    "scheme": "http"
                },
                "name": "http.status.2xx",
                "values": {
                    "count": 198726,
                    "rate": 3312.1
                }
            },
            {
                "dimensions": {
                    "httpMethod": "GET",
                    "scheme": "http"
                },
                "name": "http.status.4xx",
                "values": {
                    "count": 1,
                    "rate": 0.016666666666666666
                }
            },
            {
                "dimensions": {
                    "chain": "default",
                    "endpoint": "0.0.0.0:4080"
                },
                "name": "peak_qps",
                "values": {
                    "average": 3311.338994338994,
                    "count": 60,
                    "last": 3410.589410589411,
                    "max": 3507,
                    "min": 3121,
                    "rate": 1,
                    "sum": 198680.33966033964
                }
            }
        ]
    },
    "status": {"code": "up"},
    "time": 1619072155964
}


```
