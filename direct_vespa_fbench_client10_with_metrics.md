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
