# client -n 20 vespa 7.3
```
date; LD_LIBRARY_PATH=/tmp/tem_vespa_lib64/ vespa-fbench -n 20 -c 0 -s 300 localhost 4080 -q search_query2.txt -o res
Thu Apr 22 15:18:39 JST 2021
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
connection reuse count -- 1070256
***************** Benchmark Summary *****************
clients:                      20
ran for:                     300 seconds
cycle time:                    0 ms
lower response limit:          0 bytes
skipped requests:              0
failed requests:               0
successful requests:     1070276
cycles not held:         1070276
minimum response time:      1.21 ms
maximum response time:     42.16 ms
average response time:      5.59 ms
25   percentile:              4.10 ms
50   percentile:              5.20 ms
75   percentile:              6.70 ms
90   percentile:              7.70 ms
95   percentile:              8.30 ms
98   percentile:              9.20 ms
99   percentile:             12.40 ms
99.5 percentile:             22.10 ms
99.6 percentile:             29.80 ms
99.7 percentile:             30.40 ms
99.8 percentile:             30.70 ms
99.9 percentile:             31.00 ms
actual query rate:       3572.86 Q/s
utilization:               99.83 %
zero hit queries:         427900
http request status breakdown:
       200 :  1067172
       504 :     3104



http://<OurHost>:4080/state/v1/metrics

{
  "time" : 1619072383263,
  "status" : {
    "code" : "up"
  },
  "metrics" : {
    "snapshot" : {
      "from" : 1.619072323193E9,
      "to" : 1.619072383193E9
    },
    "values" : [ {
      "name" : "search_connections",
      "values" : {
        "average" : 17.634136981044147,
        "sum" : 17.634136981044147,
        "count" : 1,
        "last" : 17.634136981044147,
        "max" : 17.634136981044147,
        "min" : 17.634136981044147,
        "rate" : 0.016666666666666666
      }
    }, {
      "name" : "jrt.transport.client.unencrypted-connections-established",
      "values" : {
        "count" : 0,
        "rate" : 0.0
      }
    }, {
      "name" : "jdisc.http.jetty.threadpool.thread.idle",
      "values" : {
        "average" : 761.3333333333334,
        "sum" : 22840.0,
        "count" : 30,
        "last" : 758.0,
        "max" : 763.0,
        "min" : 758.0,
        "rate" : 0.5
      }
    }, {
      "name" : "jdisc.http.jetty.threadpool.thread.total",
      "values" : {
        "average" : 800.0,
        "sum" : 24000.0,
        "count" : 30,
        "last" : 800.0,
        "max" : 800.0,
        "min" : 800.0,
        "rate" : 0.5
      }
    }, {
      "name" : "jdisc.open_file_descriptors",
      "values" : {
        "average" : 569.0,
        "sum" : 3414.0,
        "count" : 6,
        "last" : 570.0,
        "max" : 570.0,
        "min" : 568.0,
        "rate" : 0.1
      }
    }, {
      "name" : "mem.heap.total",
      "values" : {
        "average" : 1.0146021376E10,
        "sum" : 6.0876128256E10,
        "count" : 6,
        "last" : 1.0146021376E10,
        "max" : 1.0146021376E10,
        "min" : 1.0146021376E10,
        "rate" : 0.1
      }
    }, {
      "name" : "jdisc.http.jetty.threadpool.thread.busy",
      "values" : {
        "average" : 27.066666666666666,
        "sum" : 812.0,
        "count" : 30,
        "last" : 30.0,
        "max" : 30.0,
        "min" : 26.0,
        "rate" : 0.5
      }
    }, {
      "name" : "serverStartedMillis",
      "values" : {
        "average" : 1.79187E8,
        "sum" : 5.37561E9,
        "count" : 30,
        "last" : 1.79212E8,
        "max" : 1.79216E8,
        "min" : 1.79158E8,
        "rate" : 0.5
      }
    }, {
      "name" : "chain_indexing_documents",
      "values" : {
        "count" : 1474,
        "rate" : 24.566666666666666
      }
    }, {
      "name" : "jdisc.deactivated_containers.total",
      "values" : {
        "average" : 0.0,
        "sum" : 0.0,
        "count" : 6,
        "last" : 0.0,
        "max" : 0.0,
        "min" : 0.0,
        "rate" : 0.1
      }
    }, {
      "name" : "docprocessor_indexing_com_yahoo_docprocs_indexing_IndexingProcessor_indexing_documents",
      "values" : {
        "count" : 1474,
        "rate" : 24.566666666666666
      }
    }, {
      "name" : "jdisc.memory_mappings",
      "values" : {
        "average" : 6526.0,
        "sum" : 39156.0,
        "count" : 6,
        "last" : 6526.0,
        "max" : 6526.0,
        "min" : 6526.0,
        "rate" : 0.1
      }
    }, {
      "name" : "jdisc.http.jetty.threadpool.thread.max",
      "values" : {
        "average" : 800.0,
        "sum" : 24000.0,
        "count" : 30,
        "last" : 800.0,
        "max" : 800.0,
        "min" : 800.0,
        "rate" : 0.5
      }
    }, {
      "name" : "jdisc.http.jetty.threadpool.thread.reserved",
      "values" : {
        "average" : -1.0,
        "sum" : -30.0,
        "count" : 30,
        "last" : -1.0,
        "max" : -1.0,
        "min" : -1.0,
        "rate" : 0.5
      }
    }, {
      "name" : "mem.heap.used",
      "values" : {
        "average" : 3.7393796693333335E9,
        "sum" : 2.2436278016E10,
        "count" : 6,
        "last" : 3.267682392E9,
        "max" : 6.667337176E9,
        "min" : 1.414956376E9,
        "rate" : 0.1
      }
    }, {
      "name" : "dispatch_internal",
      "values" : {
        "count" : 214508,
        "rate" : 3575.133333333333
      }
    }, {
      "name" : "jdisc.http.jetty.threadpool.thread.min",
      "values" : {
        "average" : 800.0,
        "sum" : 24000.0,
        "count" : 30,
        "last" : 800.0,
        "max" : 800.0,
        "min" : 800.0,
        "rate" : 0.5
      }
    }, {
      "name" : "docprocessor_indexing_com_yahoo_docprocs_indexing_IndexingProcessor_indexing_proctime",
      "values" : {
        "count" : 327,
        "rate" : 5.45
      }
    }, {
      "name" : "mem.heap.free",
      "values" : {
        "average" : 6.406641706666667E9,
        "sum" : 3.843985024E10,
        "count" : 6,
        "last" : 6.878338984E9,
        "max" : 8.731065E9,
        "min" : 3.4786842E9,
        "rate" : 0.1
      }
    }, {
      "name" : "jdisc.http.requests.status",
      "values" : {
        "count" : 8,
        "rate" : 0.13333333333333333
      }
    }, {
      "name" : "jdisc.http.jetty.threadpool.queue.size",
      "values" : {
        "average" : 0.0,
        "sum" : 0.0,
        "count" : 30,
        "last" : 0.0,
        "max" : 0.0,
        "min" : 0.0,
        "rate" : 0.5
      }
    }, {
      "name" : "jdisc.gc.ms",
      "values" : {
        "average" : 76.16666666666667,
        "sum" : 457.0,
        "count" : 6,
        "last" : 134.0,
        "max" : 134.0,
        "min" : 17.0,
        "rate" : 0.1
      },
      "dimensions" : {
        "gcName" : "G1YoungGeneration"
      }
    }, {
      "name" : "jdisc.gc.count",
      "values" : {
        "average" : 10.166666666666666,
        "sum" : 61.0,
        "count" : 6,
        "last" : 18.0,
        "max" : 18.0,
        "min" : 2.0,
        "rate" : 0.1
      },
      "dimensions" : {
        "gcName" : "G1YoungGeneration"
      }
    }, {
      "name" : "serverActiveThreads",
      "values" : {
        "average" : 17.846410684474122,
        "sum" : 10690.0,
        "count" : 599,
        "last" : 17.0,
        "max" : 20.0,
        "min" : 1.0,
        "rate" : 9.983333333333333
      },
      "dimensions" : {
        "threadpool" : "search-handler"
      }
    }, {
      "name" : "serverThreadPoolSize",
      "values" : {
        "average" : 1509.941569282137,
        "sum" : 904455.0,
        "count" : 599,
        "last" : 1518.0,
        "max" : 1518.0,
        "min" : 1500.0,
        "rate" : 9.983333333333333
      },
      "dimensions" : {
        "threadpool" : "search-handler"
      }
    }, {
      "name" : "jdisc.thread_pool.work_queue.capacity",
      "values" : {
        "average" : 10.0,
        "sum" : 5990.0,
        "count" : 599,
        "last" : 10.0,
        "max" : 10.0,
        "min" : 10.0,
        "rate" : 9.983333333333333
      },
      "dimensions" : {
        "threadpool" : "search-handler"
      }
    }, {
      "name" : "jdisc.thread_pool.work_queue.size",
      "values" : {
        "average" : 0.14357262103505844,
        "sum" : 86.0,
        "count" : 599,
        "last" : 0.0,
        "max" : 7.0,
        "min" : 0.0,
        "rate" : 9.983333333333333
      },
      "dimensions" : {
        "threadpool" : "search-handler"
      }
    }, {
      "name" : "handled.latency",
      "values" : {
        "average" : 5.296854167249401,
        "sum" : 1136207.0,
        "count" : 214506,
        "last" : 7.0,
        "max" : 39.0,
        "min" : 1.0,
        "rate" : 3575.1
      },
      "dimensions" : {
        "handler" : "http://*:*/search/*",
        "handler-name" : "com.yahoo.container.jdisc.ThreadedRequestHandler$RequestTask",
        "endpoint" : "localhost:4080",
        "scheme" : "http",
        "port" : "4080"
      }
    }, {
      "name" : "jdisc.gc.ms",
      "values" : {
        "average" : 0.0,
        "sum" : 0.0,
        "count" : 6,
        "last" : 0.0,
        "max" : 0.0,
        "min" : 0.0,
        "rate" : 0.1
      },
      "dimensions" : {
        "gcName" : "G1OldGeneration"
      }
    }, {
      "name" : "jdisc.gc.count",
      "values" : {
        "average" : 0.0,
        "sum" : 0.0,
        "count" : 6,
        "last" : 0.0,
        "max" : 0.0,
        "min" : 0.0,
        "rate" : 0.1
      },
      "dimensions" : {
        "gcName" : "G1OldGeneration"
      }
    }, {
      "name" : "http.status.2xx",
      "values" : {
        "count" : 213841,
        "rate" : 3564.016666666667
      },
      "dimensions" : {
        "httpMethod" : "GET",
        "requestType" : "read",
        "scheme" : "http"
      }
    }, {
      "name" : "http.status.5xx",
      "values" : {
        "count" : 758,
        "rate" : 12.633333333333333
      },
      "dimensions" : {
        "httpMethod" : "GET",
        "requestType" : "read",
        "scheme" : "http"
      }
    }, {
      "name" : "handled.requests",
      "values" : {
        "count" : 8,
        "rate" : 0.13333333333333333
      },
      "dimensions" : {
        "handler" : "http://*:*/status.html",
        "handler-name" : "com.yahoo.container.handler.VipStatusHandler",
        "endpoint" : "0.0.0.0:4080",
        "scheme" : "http",
        "port" : "4080"
      }
    }, {
      "name" : "documents_processed",
      "values" : {
        "count" : 1474,
        "rate" : 24.566666666666666
      },
      "dimensions" : {
        "chain" : "indexing",
        "documenttype" : "<OurProductID>"
      }
    }, {
      "name" : "handled.latency",
      "values" : {
        "average" : 0.0,
        "sum" : 0.0,
        "count" : 8,
        "last" : 0.0,
        "max" : 0.0,
        "min" : 0.0,
        "rate" : 0.13333333333333333
      },
      "dimensions" : {
        "handler" : "http://*:*/status.html",
        "handler-name" : "com.yahoo.container.jdisc.ThreadedRequestHandler$RequestTask",
        "endpoint" : "0.0.0.0:4080",
        "scheme" : "http",
        "port" : "4080"
      }
    }, {
      "name" : "relevance.at_10",
      "values" : {
        "average" : 3514213.3136674343,
        "sum" : 4.522862818956261E11,
        "count" : 128702,
        "last" : 6964334.445994968,
        "max" : 6964334.499994855,
        "min" : 35966.0774461932,
        "rate" : 2145.0333333333333
      },
      "dimensions" : {
        "rankProfile" : "<OurProductID>",
        "chain" : "default"
      }
    }, {
      "name" : "relevance.at_1",
      "values" : {
        "average" : 9.737437097368733E8,
        "sum" : 1.2532276293055506E14,
        "count" : 128702,
        "last" : 1.9340000001745687E9,
        "max" : 1.934000000499976E9,
        "min" : 113904.40438402537,
        "rate" : 2145.0333333333333
      },
      "dimensions" : {
        "rankProfile" : "<OurProductID>",
        "chain" : "default"
      }
    }, {
      "name" : "relevance.at_3",
      "values" : {
        "average" : 1.1249332156292593E7,
        "sum" : 1.4478115471791694E12,
        "count" : 128702,
        "last" : 2.236578930319988E7,
        "max" : 2.2365789499995593E7,
        "min" : 54012.32089614752,
        "rate" : 2145.0333333333333
      },
      "dimensions" : {
        "rankProfile" : "<OurProductID>",
        "chain" : "default"
      }
    }, {
      "name" : "query_latency",
      "values" : {
        "average" : 3.5588566774247687,
        "sum" : 763392.551591,
        "count" : 214505,
        "last" : 5.047345,
        "max" : 37.982841,
        "min" : 0.807646,
        "rate" : 3575.0833333333335,
        "95percentile" : 4.68359375,
        "99percentile" : 8.24609375
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "documents_covered",
      "values" : {
        "count" : 19122274236994,
        "rate" : 3.1870457061656665E11
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "query_hit_offset",
      "values" : {
        "average" : 12.0,
        "sum" : 2574060.0,
        "count" : 214505,
        "last" : 12.0,
        "max" : 12.0,
        "min" : 12.0,
        "rate" : 3575.0833333333335
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "documents_total",
      "values" : {
        "count" : 19127208399118,
        "rate" : 3.187868066519667E11
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "failed_queries",
      "values" : {
        "count" : 122,
        "rate" : 2.033333333333333
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "empty_results",
      "values" : {
        "count" : 85803,
        "rate" : 1430.05
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "max_query_latency",
      "values" : {
        "average" : 3.5588566774247687,
        "sum" : 763392.551591,
        "count" : 214505,
        "last" : 5.047345,
        "max" : 37.982841,
        "min" : 0.807646,
        "rate" : 3575.0833333333335
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "peak_qps",
      "values" : {
        "average" : 3575.905444555445,
        "sum" : 214554.3266733267,
        "count" : 60,
        "last" : 3661.0,
        "max" : 3822.0,
        "min" : 3119.0,
        "rate" : 1.0
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "totalhits_per_query",
      "values" : {
        "average" : 87.56739936132026,
        "sum" : 1.8783645E7,
        "count" : 214505,
        "last" : 0.0,
        "max" : 156.0,
        "min" : 0.0,
        "rate" : 3575.0833333333335,
        "95percentile" : 156.75,
        "99percentile" : 156.75
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "hits_per_query",
      "values" : {
        "average" : 7.199944057248083,
        "sum" : 1544424.0,
        "count" : 214505,
        "last" : 0.0,
        "max" : 12.0,
        "min" : 0.0,
        "rate" : 3575.0833333333335,
        "95percentile" : 12.0,
        "99percentile" : 12.0
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "queries",
      "values" : {
        "count" : 214507,
        "rate" : 3575.116666666667
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "mean_query_latency",
      "values" : {
        "average" : 3.5588566774247687,
        "sum" : 763392.551591,
        "count" : 214505,
        "last" : 5.047345,
        "max" : 37.982841,
        "min" : 0.807646,
        "rate" : 3575.0833333333335
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "error.timeout",
      "values" : {
        "count" : 122,
        "rate" : 2.033333333333333
      },
      "dimensions" : {
        "source" : "<OurProductID>"
      }
    }, {
      "name" : "serverNumRequests",
      "values" : {
        "count" : 214510,
        "rate" : 3575.1666666666665
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "localhost",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "jdisc.http.filtering.response.unhandled",
      "values" : {
        "count" : 214510,
        "rate" : 3575.1666666666665
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "localhost",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "serverTimeToFirstByte",
      "values" : {
        "average" : 5.384726191197654,
        "sum" : 1155083.0,
        "count" : 214511,
        "last" : 7.0,
        "max" : 39.0,
        "min" : 1.0,
        "rate" : 3575.1833333333334
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "localhost",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "serverBytesSent",
      "values" : {
        "average" : 4601.499601719001,
        "sum" : 1.87165076E9,
        "count" : 406748,
        "last" : 6019.0,
        "max" : 35267.0,
        "min" : 68.0,
        "rate" : 6779.133333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "localhost",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "serverNumSuccessfulResponseWrites",
      "values" : {
        "count" : 406748,
        "rate" : 6779.133333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "localhost",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "jdisc.http.filtering.request.unhandled",
      "values" : {
        "count" : 214510,
        "rate" : 3575.1666666666665
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "localhost",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "jdisc.http.request.uri_length",
      "values" : {
        "average" : 404.2962612465619,
        "sum" : 8.6725591E7,
        "count" : 214510,
        "last" : 407.0,
        "max" : 408.0,
        "min" : 17.0,
        "rate" : 3575.1666666666665
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "localhost",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "jdisc.http.requests",
      "values" : {
        "count" : 214510,
        "rate" : 3575.1666666666665
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "localhost",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "serverTotalSuccessfulResponseLatency",
      "values" : {
        "average" : 5.467017854645471,
        "sum" : 1172730.0,
        "count" : 214510,
        "last" : 7.0,
        "max" : 41.0,
        "min" : 1.0,
        "rate" : 3575.1666666666665
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "localhost",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "jdisc.http.request.content_size",
      "values" : {
        "average" : 0.0,
        "sum" : 0.0,
        "count" : 214510,
        "last" : 0.0,
        "max" : 0.0,
        "min" : 0.0,
        "rate" : 3575.1666666666665
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "localhost",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "serverNumSuccessfulResponses",
      "values" : {
        "count" : 214510,
        "rate" : 3575.1666666666665
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "localhost",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "serverNumRequests",
      "values" : {
        "count" : 44,
        "rate" : 0.7333333333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "<OurHost>",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "jdisc.http.filtering.response.unhandled",
      "values" : {
        "count" : 44,
        "rate" : 0.7333333333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "<OurHost>",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "serverTimeToFirstByte",
      "values" : {
        "average" : 1.3863636363636365,
        "sum" : 61.0,
        "count" : 44,
        "last" : 2.0,
        "max" : 2.0,
        "min" : 1.0,
        "rate" : 0.7333333333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "<OurHost>",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "serverBytesSent",
      "values" : {
        "average" : 35305.181818181816,
        "sum" : 1553428.0,
        "count" : 44,
        "last" : 35293.0,
        "max" : 35355.0,
        "min" : 35100.0,
        "rate" : 0.7333333333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "<OurHost>",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "serverNumSuccessfulResponseWrites",
      "values" : {
        "count" : 44,
        "rate" : 0.7333333333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "<OurHost>",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "jdisc.http.filtering.request.unhandled",
      "values" : {
        "count" : 44,
        "rate" : 0.7333333333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "<OurHost>",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "jdisc.http.request.uri_length",
      "values" : {
        "average" : 17.0,
        "sum" : 748.0,
        "count" : 44,
        "last" : 17.0,
        "max" : 17.0,
        "min" : 17.0,
        "rate" : 0.7333333333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "<OurHost>",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "jdisc.http.requests",
      "values" : {
        "count" : 44,
        "rate" : 0.7333333333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "<OurHost>",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "serverTotalSuccessfulResponseLatency",
      "values" : {
        "average" : 1.5227272727272727,
        "sum" : 67.0,
        "count" : 44,
        "last" : 2.0,
        "max" : 2.0,
        "min" : 1.0,
        "rate" : 0.7333333333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "<OurHost>",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "serverNumSuccessfulResponses",
      "values" : {
        "count" : 44,
        "rate" : 0.7333333333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "<OurHost>",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "jdisc.http.request.content_size",
      "values" : {
        "average" : 0.0,
        "sum" : 0.0,
        "count" : 44,
        "last" : 0.0,
        "max" : 0.0,
        "min" : 0.0,
        "rate" : 0.7333333333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "<OurHost>",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "http.status.2xx",
      "values" : {
        "count" : 54,
        "rate" : 0.9
      },
      "dimensions" : {
        "httpMethod" : "GET",
        "requestType" : "monitoring",
        "scheme" : "http"
      }
    }, {
      "name" : "serverConnectionDurationMean",
      "values" : {
        "average" : 52433.29321775813,
        "sum" : 1572998.7965327438,
        "count" : 30,
        "last" : 52425.92271016311,
        "max" : 52434.76731927711,
        "min" : 52425.92271016311,
        "rate" : 0.5
      },
      "dimensions" : {
        "serverPort" : "4080",
        "serverName" : "myserver"
      }
    }, {
      "name" : "serverConnectionDurationMax",
      "values" : {
        "average" : 7.72157E7,
        "sum" : 2.316471E9,
        "count" : 30,
        "last" : 7.72157E7,
        "max" : 7.72157E7,
        "min" : 7.72157E7,
        "rate" : 0.5
      },
      "dimensions" : {
        "serverPort" : "4080",
        "serverName" : "myserver"
      }
    }, {
      "name" : "serverConnectionsOpenMax",
      "values" : {
        "average" : 324.0,
        "sum" : 9720.0,
        "count" : 30,
        "last" : 324.0,
        "max" : 324.0,
        "min" : 324.0,
        "rate" : 0.5
      },
      "dimensions" : {
        "serverPort" : "4080",
        "serverName" : "myserver"
      }
    }, {
      "name" : "serverNumConnections",
      "values" : {
        "average" : 4007.0333333333333,
        "sum" : 120211.0,
        "count" : 30,
        "last" : 4009.0,
        "max" : 4009.0,
        "min" : 4006.0,
        "rate" : 0.5
      },
      "dimensions" : {
        "serverPort" : "4080",
        "serverName" : "myserver"
      }
    }, {
      "name" : "serverNumOpenConnections",
      "values" : {
        "average" : 22.866666666666667,
        "sum" : 686.0,
        "count" : 30,
        "last" : 24.0,
        "max" : 24.0,
        "min" : 22.0,
        "rate" : 0.5
      },
      "dimensions" : {
        "serverPort" : "4080",
        "serverName" : "myserver"
      }
    }, {
      "name" : "serverConnectionDurationStdDev",
      "values" : {
        "average" : 1230230.654212366,
        "sum" : 3.690691962637098E7,
        "count" : 30,
        "last" : 1230102.0853328344,
        "max" : 1230256.3679882716,
        "min" : 1230102.0853328344,
        "rate" : 0.5
      },
      "dimensions" : {
        "serverPort" : "4080",
        "serverName" : "myserver"
      }
    }, {
      "name" : "query_container_latency",
      "values" : {
        "average" : 0.0852835325489026,
        "sum" : 18294.0,
        "count" : 214508,
        "last" : 0.0,
        "max" : 11.0,
        "min" : 0.0,
        "rate" : 3575.133333333333
      },
      "dimensions" : {
        "chain" : "<OurProductID>"
      }
    }, {
      "name" : "handled.latency",
      "values" : {
        "average" : 4.0,
        "sum" : 0.0,
        "count" : 0,
        "last" : 4.0,
        "max" : 4.0,
        "min" : 4.0,
        "rate" : 0.0
      },
      "dimensions" : {
        "handler" : "http://*:*/search/*",
        "handler-name" : "com.yahoo.container.jdisc.ThreadedRequestHandler$RequestTask",
        "endpoint" : "<OurHost>:4080",
        "scheme" : "http",
        "port" : "4080"
      }
    }, {
      "name" : "jdisc.http.filtering.response.unhandled",
      "values" : {
        "count" : 8,
        "rate" : 0.13333333333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "0.0.0.0",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "serverNumRequests",
      "values" : {
        "count" : 8,
        "rate" : 0.13333333333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "0.0.0.0",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "serverTimeToFirstByte",
      "values" : {
        "average" : 0.0,
        "sum" : 0.0,
        "count" : 8,
        "last" : 0.0,
        "max" : 0.0,
        "min" : 0.0,
        "rate" : 0.13333333333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "0.0.0.0",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "serverBytesSent",
      "values" : {
        "average" : 18.0,
        "sum" : 144.0,
        "count" : 8,
        "last" : 18.0,
        "max" : 18.0,
        "min" : 18.0,
        "rate" : 0.13333333333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "0.0.0.0",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "jdisc.http.filtering.request.unhandled",
      "values" : {
        "count" : 8,
        "rate" : 0.13333333333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "0.0.0.0",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "serverNumSuccessfulResponseWrites",
      "values" : {
        "count" : 8,
        "rate" : 0.13333333333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "0.0.0.0",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "jdisc.http.request.uri_length",
      "values" : {
        "average" : 12.0,
        "sum" : 96.0,
        "count" : 8,
        "last" : 12.0,
        "max" : 12.0,
        "min" : 12.0,
        "rate" : 0.13333333333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "0.0.0.0",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "serverTotalSuccessfulResponseLatency",
      "values" : {
        "average" : 0.0,
        "sum" : 0.0,
        "count" : 8,
        "last" : 0.0,
        "max" : 0.0,
        "min" : 0.0,
        "rate" : 0.13333333333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "0.0.0.0",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "jdisc.http.requests",
      "values" : {
        "count" : 8,
        "rate" : 0.13333333333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "0.0.0.0",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "serverNumSuccessfulResponses",
      "values" : {
        "count" : 8,
        "rate" : 0.13333333333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "0.0.0.0",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "jdisc.http.request.content_size",
      "values" : {
        "average" : 0.0,
        "sum" : 0.0,
        "count" : 8,
        "last" : 0.0,
        "max" : 0.0,
        "min" : 0.0,
        "rate" : 0.13333333333333333
      },
      "dimensions" : {
        "clientAuthenticated" : "false",
        "serverName" : "myserver",
        "httpMethod" : "GET",
        "requestServerName" : "0.0.0.0",
        "scheme" : "http",
        "serverPort" : "4080"
      }
    }, {
      "name" : "handled.requests",
      "values" : {
        "count" : 214508,
        "rate" : 3575.133333333333
      },
      "dimensions" : {
        "handler" : "http://*:*/search/*",
        "handler-name" : "com.yahoo.search.handler.SearchHandler",
        "endpoint" : "localhost:4080",
        "scheme" : "http",
        "port" : "4080"
      }
    }, {
      "name" : "handled.requests",
      "values" : {
        "count" : 0,
        "rate" : 0.0
      },
      "dimensions" : {
        "handler" : "http://*:*/search/*",
        "handler-name" : "com.yahoo.search.handler.SearchHandler",
        "endpoint" : "<OurHost>:4080",
        "scheme" : "http",
        "port" : "4080"
      }
    }, {
      "name" : "serverActiveThreads",
      "values" : {
        "average" : 0.0,
        "sum" : 0.0,
        "count" : 599,
        "last" : 0.0,
        "max" : 0.0,
        "min" : 0.0,
        "rate" : 9.983333333333333
      },
      "dimensions" : {
        "threadpool" : "default-pool"
      }
    }, {
      "name" : "serverThreadPoolSize",
      "values" : {
        "average" : 500.0,
        "sum" : 299500.0,
        "count" : 599,
        "last" : 500.0,
        "max" : 500.0,
        "min" : 500.0,
        "rate" : 9.983333333333333
      },
      "dimensions" : {
        "threadpool" : "default-pool"
      }
    }, {
      "name" : "jdisc.thread_pool.work_queue.size",
      "values" : {
        "average" : 0.0,
        "sum" : 0.0,
        "count" : 599,
        "last" : 0.0,
        "max" : 0.0,
        "min" : 0.0,
        "rate" : 9.983333333333333
      },
      "dimensions" : {
        "threadpool" : "default-pool"
      }
    }, {
      "name" : "jdisc.thread_pool.work_queue.capacity",
      "values" : {
        "average" : 0.0,
        "sum" : 0.0,
        "count" : 599,
        "last" : 0.0,
        "max" : 0.0,
        "min" : 0.0,
        "rate" : 9.983333333333333
      },
      "dimensions" : {
        "threadpool" : "default-pool"
      }
    }, {
      "name" : "degraded_queries",
      "values" : {
        "count" : 770,
        "rate" : 12.833333333333334
      },
      "dimensions" : {
        "reason" : "timeout",
        "chain" : "default"
      }
    } ]
  }
}

```
