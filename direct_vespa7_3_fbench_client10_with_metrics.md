# client -n 10 vespa 7.3

```
[<OurHost> ~]date; LD_LIBRARY_PATH=/tmp/tem_vespa_lib64/ vespa-fbench -n 10 -c 0 -s 300 localhost 4080 -q search_query2.txt -o res
Thu Apr 22 15:12:44 JST 2021
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
connection reuse count -- 885080
***************** Benchmark Summary *****************
clients:                      10
ran for:                     300 seconds
cycle time:                    0 ms
lower response limit:          0 bytes
skipped requests:              0
failed requests:               0
successful requests:      885090
cycles not held:          885090
minimum response time:      1.19 ms
maximum response time:     32.24 ms
average response time:      3.38 ms
25   percentile:              2.60 ms
50   percentile:              3.40 ms
75   percentile:              4.00 ms
90   percentile:              4.40 ms
95   percentile:              4.80 ms
98   percentile:              5.20 ms
99   percentile:              5.60 ms
99.5 percentile:              6.30 ms
99.6 percentile:              6.90 ms
99.7 percentile:              7.60 ms
99.8 percentile:             12.70 ms
99.9 percentile:             17.10 ms
actual query rate:       2954.69 Q/s
utilization:               99.73 %
zero hit queries:         354020
http request status breakdown:
       200 :   884700
       504 :      390
[<OurHost> ~]





http://<OurHost>:4080/state/v1/metrics

{
  "time" : 1619072100791,
  "status" : {
    "code" : "up"
  },
  "metrics" : {
    "snapshot" : {
      "from" : 1.619072040193E9,
      "to" : 1.619072100193E9
    },
    "values" : [ {
      "name" : "search_connections",
      "values" : {
        "average" : 8.244334197767504,
        "sum" : 8.244334197767504,
        "count" : 1,
        "last" : 8.244334197767504,
        "max" : 8.244334197767504,
        "min" : 8.244334197767504,
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
        "average" : 764.8333333333334,
        "sum" : 22945.0,
        "count" : 30,
        "last" : 765.0,
        "max" : 766.0,
        "min" : 762.0,
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
        "average" : 559.5,
        "sum" : 3357.0,
        "count" : 6,
        "last" : 559.0,
        "max" : 560.0,
        "min" : 559.0,
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
        "average" : 26.6,
        "sum" : 798.0,
        "count" : 30,
        "last" : 26.0,
        "max" : 30.0,
        "min" : 26.0,
        "rate" : 0.5
      }
    }, {
      "name" : "serverStartedMillis",
      "values" : {
        "average" : 1.78903E8,
        "sum" : 5.36709E9,
        "count" : 30,
        "last" : 1.78912E8,
        "max" : 1.78932E8,
        "min" : 1.78874E8,
        "rate" : 0.5
      }
    }, {
      "name" : "chain_indexing_documents",
      "values" : {
        "count" : 1469,
        "rate" : 24.483333333333334
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
        "count" : 1469,
        "rate" : 24.483333333333334
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
        "average" : 4.368182785333333E9,
        "sum" : 2.6209096712E10,
        "count" : 6,
        "last" : 3.084203296E9,
        "max" : 6.538809992E9,
        "min" : 2.184392104E9,
        "rate" : 0.1
      }
    }, {
      "name" : "dispatch_internal",
      "values" : {
        "count" : 177372,
        "rate" : 2956.2
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
        "count" : 295,
        "rate" : 4.916666666666667
      }
    }, {
      "name" : "mem.heap.free",
      "values" : {
        "average" : 5.777838590666667E9,
        "sum" : 3.4667031544E10,
        "count" : 6,
        "last" : 7.06181808E9,
        "max" : 7.961629272E9,
        "min" : 3.607211384E9,
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
        "average" : 145.66666666666666,
        "sum" : 874.0,
        "count" : 6,
        "last" : 153.0,
        "max" : 159.0,
        "min" : 130.0,
        "rate" : 0.1
      },
      "dimensions" : {
        "gcName" : "G1YoungGeneration"
      }
    }, {
      "name" : "jdisc.gc.count",
      "values" : {
        "average" : 15.333333333333334,
        "sum" : 92.0,
        "count" : 6,
        "last" : 16.0,
        "max" : 16.0,
        "min" : 15.0,
        "rate" : 0.1
      },
      "dimensions" : {
        "gcName" : "G1YoungGeneration"
      }
    }, {
      "name" : "serverActiveThreads",
      "values" : {
        "average" : 8.37228714524207,
        "sum" : 5015.0,
        "count" : 599,
        "last" : 10.0,
        "max" : 10.0,
        "min" : 0.0,
        "rate" : 9.983333333333333
      },
      "dimensions" : {
        "threadpool" : "search-handler"
      }
    }, {
      "name" : "serverThreadPoolSize",
      "values" : {
        "average" : 1500.0,
        "sum" : 898500.0,
        "count" : 599,
        "last" : 1500.0,
        "max" : 1500.0,
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
        "average" : 0.13856427378964942,
        "sum" : 83.0,
        "count" : 599,
        "last" : 0.0,
        "max" : 2.0,
        "min" : 0.0,
        "rate" : 9.983333333333333
      },
      "dimensions" : {
        "threadpool" : "search-handler"
      }
    }, {
      "name" : "handled.latency",
      "values" : {
        "average" : 3.0958268497846335,
        "sum" : 549113.0,
        "count" : 177372,
        "last" : 1.0,
        "max" : 32.0,
        "min" : 1.0,
        "rate" : 2956.2
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
        "count" : 177514,
        "rate" : 2958.5666666666666
      },
      "dimensions" : {
        "httpMethod" : "GET",
        "requestType" : "read",
        "scheme" : "http"
      }
    }, {
      "name" : "http.status.5xx",
      "values" : {
        "count" : 54,
        "rate" : 0.9
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
        "count" : 1469,
        "rate" : 24.483333333333334
      },
      "dimensions" : {
        "chain" : "indexing",
        "documenttype" : "<OurProductID>"
      }
    }, {
      "name" : "handled.latency",
      "values" : {
        "average" : 0.125,
        "sum" : 1.0,
        "count" : 8,
        "last" : 0.0,
        "max" : 1.0,
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
        "average" : 3515422.1680757687,
        "sum" : 3.741147425487914E11,
        "count" : 106421,
        "last" : 6964334.126576161,
        "max" : 6964334.499999648,
        "min" : 62146.277136710705,
        "rate" : 1773.6833333333334
      },
      "dimensions" : {
        "rankProfile" : "<OurProductID>",
        "chain" : "default"
      }
    }, {
      "name" : "relevance.at_1",
      "values" : {
        "average" : 9.740242177119825E8,
        "sum" : 1.0365663127312689E14,
        "count" : 106421,
        "last" : 1.934000000392648E9,
        "max" : 1.9340000004999907E9,
        "min" : 1.4012180091008153E7,
        "rate" : 1773.6833333333334
      },
      "dimensions" : {
        "rankProfile" : "<OurProductID>",
        "chain" : "default"
      }
    }, {
      "name" : "relevance.at_3",
      "values" : {
        "average" : 1.1251270435980087E7,
        "sum" : 1.1973714510674368E12,
        "count" : 106421,
        "last" : 2.2365789153402936E7,
        "max" : 2.2365789499996353E7,
        "min" : 131502.1401620442,
        "rate" : 1773.6833333333334
      },
      "dimensions" : {
        "rankProfile" : "<OurProductID>",
        "chain" : "default"
      }
    }, {
      "name" : "query_latency",
      "values" : {
        "average" : 2.0225982296386085,
        "sum" : 358748.247991,
        "count" : 177370,
        "last" : 1.724637,
        "max" : 31.137864999999998,
        "min" : 0.791574,
        "rate" : 2956.1666666666665,
        "95percentile" : 2.80859375,
        "99percentile" : 3.27734375
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "documents_covered",
      "values" : {
        "count" : 15825500766174,
        "rate" : 2.637583461029E11
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "query_hit_offset",
      "values" : {
        "average" : 12.0,
        "sum" : 2128440.0,
        "count" : 177370,
        "last" : 12.0,
        "max" : 12.0,
        "min" : 12.0,
        "rate" : 2956.1666666666665
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "documents_total",
      "values" : {
        "count" : 15825777432310,
        "rate" : 2.6376295720516666E11
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "failed_queries",
      "values" : {
        "count" : 4,
        "rate" : 0.06666666666666667
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "empty_results",
      "values" : {
        "count" : 70949,
        "rate" : 1182.4833333333333
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "max_query_latency",
      "values" : {
        "average" : 2.0225982296386085,
        "sum" : 358748.247991,
        "count" : 177370,
        "last" : 1.724637,
        "max" : 31.137864999999998,
        "min" : 0.791574,
        "rate" : 2956.1666666666665
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "peak_qps",
      "values" : {
        "average" : 2956.9551115551117,
        "sum" : 177417.3066933067,
        "count" : 60,
        "last" : 2986.0,
        "max" : 3016.0,
        "min" : 2801.0,
        "rate" : 1.0
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "totalhits_per_query",
      "values" : {
        "average" : 87.59649320629194,
        "sum" : 1.553699E7,
        "count" : 177370,
        "last" : 156.0,
        "max" : 156.0,
        "min" : 0.0,
        "rate" : 2956.1666666666665,
        "95percentile" : 156.5,
        "99percentile" : 156.5
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "hits_per_query",
      "values" : {
        "average" : 7.199932344815921,
        "sum" : 1277052.0,
        "count" : 177370,
        "last" : 12.0,
        "max" : 12.0,
        "min" : 0.0,
        "rate" : 2956.1666666666665,
        "95percentile" : 12.0,
        "99percentile" : 12.0
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "queries",
      "values" : {
        "count" : 177371,
        "rate" : 2956.1833333333334
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "mean_query_latency",
      "values" : {
        "average" : 2.0225982296386085,
        "sum" : 358748.247991,
        "count" : 177370,
        "last" : 1.724637,
        "max" : 31.137864999999998,
        "min" : 0.791574,
        "rate" : 2956.1666666666665
      },
      "dimensions" : {
        "chain" : "default"
      }
    }, {
      "name" : "error.timeout",
      "values" : {
        "count" : 4,
        "rate" : 0.06666666666666667
      },
      "dimensions" : {
        "source" : "<OurProductID>"
      }
    }, {
      "name" : "serverNumRequests",
      "values" : {
        "count" : 177374,
        "rate" : 2956.233333333333
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
        "count" : 177374,
        "rate" : 2956.233333333333
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
        "average" : 3.1784339040767655,
        "sum" : 563762.0,
        "count" : 177371,
        "last" : 4.0,
        "max" : 32.0,
        "min" : 1.0,
        "rate" : 2956.1833333333334
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
        "average" : 4608.251076636324,
        "sum" : 1.552653427E9,
        "count" : 336929,
        "last" : 5637.0,
        "max" : 34781.0,
        "min" : 68.0,
        "rate" : 5615.483333333334
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
        "count" : 336929,
        "rate" : 5615.483333333334
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
        "count" : 177374,
        "rate" : 2956.233333333333
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
        "average" : 404.2956013846449,
        "sum" : 7.1711528E7,
        "count" : 177374,
        "last" : 408.0,
        "max" : 408.0,
        "min" : 17.0,
        "rate" : 2956.233333333333
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
        "count" : 177374,
        "rate" : 2956.233333333333
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
        "average" : 3.263497057032677,
        "sum" : 578853.0,
        "count" : 177372,
        "last" : 4.0,
        "max" : 32.0,
        "min" : 1.0,
        "rate" : 2956.2
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
        "count" : 177374,
        "last" : 0.0,
        "max" : 0.0,
        "min" : 0.0,
        "rate" : 2956.233333333333
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
        "count" : 177372,
        "rate" : 2956.2
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
        "count" : 1,
        "rate" : 0.016666666666666666
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
        "count" : 1,
        "rate" : 0.016666666666666666
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
        "average" : 1.0,
        "sum" : 1.0,
        "count" : 1,
        "last" : 1.0,
        "max" : 1.0,
        "min" : 1.0,
        "rate" : 0.016666666666666666
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
        "average" : 34594.0,
        "sum" : 34594.0,
        "count" : 1,
        "last" : 34594.0,
        "max" : 34594.0,
        "min" : 34594.0,
        "rate" : 0.016666666666666666
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
        "count" : 1,
        "rate" : 0.016666666666666666
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
        "count" : 1,
        "rate" : 0.016666666666666666
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
        "sum" : 17.0,
        "count" : 1,
        "last" : 17.0,
        "max" : 17.0,
        "min" : 17.0,
        "rate" : 0.016666666666666666
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
        "count" : 1,
        "rate" : 0.016666666666666666
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
        "average" : 1.0,
        "sum" : 1.0,
        "count" : 1,
        "last" : 1.0,
        "max" : 1.0,
        "min" : 1.0,
        "rate" : 0.016666666666666666
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
        "count" : 1,
        "rate" : 0.016666666666666666
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
        "count" : 1,
        "last" : 0.0,
        "max" : 0.0,
        "min" : 0.0,
        "rate" : 0.016666666666666666
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
        "count" : 11,
        "rate" : 0.18333333333333332
      },
      "dimensions" : {
        "httpMethod" : "GET",
        "requestType" : "monitoring",
        "scheme" : "http"
      }
    }, {
      "name" : "serverConnectionDurationMean",
      "values" : {
        "average" : 51719.3020973749,
        "sum" : 1551579.062921247,
        "count" : 30,
        "last" : 51720.5304632427,
        "max" : 51720.5304632427,
        "min" : 51716.43591035004,
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
        "average" : 3985.0333333333333,
        "sum" : 119551.0,
        "count" : 30,
        "last" : 3985.0,
        "max" : 3986.0,
        "min" : 3985.0,
        "rate" : 0.5
      },
      "dimensions" : {
        "serverPort" : "4080",
        "serverName" : "myserver"
      }
    }, {
      "name" : "serverNumOpenConnections",
      "values" : {
        "average" : 13.333333333333334,
        "sum" : 400.0,
        "count" : 30,
        "last" : 13.0,
        "max" : 14.0,
        "min" : 13.0,
        "rate" : 0.5
      },
      "dimensions" : {
        "serverPort" : "4080",
        "serverName" : "myserver"
      }
    }, {
      "name" : "serverConnectionDurationStdDev",
      "values" : {
        "average" : 1232089.6760745521,
        "sum" : 3.696269028223656E7,
        "count" : 30,
        "last" : 1232043.1363638863,
        "max" : 1232198.2687327727,
        "min" : 1232043.1363638863,
        "rate" : 0.5
      },
      "dimensions" : {
        "serverPort" : "4080",
        "serverName" : "myserver"
      }
    }, {
      "name" : "query_container_latency",
      "values" : {
        "average" : 0.08130370069684054,
        "sum" : 14421.0,
        "count" : 177372,
        "last" : 0.0,
        "max" : 13.0,
        "min" : 0.0,
        "rate" : 2956.2
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
        "average" : 0.25,
        "sum" : 2.0,
        "count" : 8,
        "last" : 1.0,
        "max" : 1.0,
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
        "average" : 0.25,
        "sum" : 2.0,
        "count" : 8,
        "last" : 1.0,
        "max" : 1.0,
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
        "count" : 177372,
        "rate" : 2956.2
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
        "count" : 77,
        "rate" : 1.2833333333333334
      },
      "dimensions" : {
        "reason" : "timeout",
        "chain" : "default"
      }
    } ]
  }
}
```
