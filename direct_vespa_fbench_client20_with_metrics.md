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
