```
$ sudo cat /opt/vespa/var/db/vespa/config_server/serverdb/tenants/default/sessions/28/services.xml


<?xml version="1.0" encoding="utf-8" ?>
<services version="1.0">
  <config name="cloud.config.log.logd">
    <logserver>
      <use>false</use>
    </logserver>
  </config>
  <admin version="2.0">
    <adminserver hostalias=#### 00 host ####" />
    <configservers>
    #################################################################
     ######  00 ~04, total 5 hosts #########################################
     #################################################################
          </configservers>
    <slobroks>
    #################################################################
     ######  00 ~04, total 5 hosts #########################################
     #################################################################
          </slobroks>
  </admin>

  <container id="httpgateway" version="1.0">
    <config name="container.handler.threadpool">
      <maxthreads>1250</maxthreads>
    </config>
    <document-api/>
    <nodes>
      <!-- Admin nodes need more jobs -->
    #################################################################
     ######  00 ~04, total 5 hosts #########################################
     #################################################################
          </nodes>
    <accesslog fileNamePattern='/opt/vespa/logs/vespa/qrs/JsonAccessLog.httpgateway.%Y%m%d%H%M%S' symlinkName='JsonAccessLog.httpgateway' rotationInterval='0 60 ...' />
  </container>

  <container id="default" version="1.0">
    <accesslog type="disabled" />
    <search>
      <threadpool>
        <max-threads>3000</max-threads>
        <min-threads>1500</min-threads>
        <queue-size>10</queue-size>
      </threadpool>
    </search>
    <config name="jdisc.http.server">
      <maxWorkerThreads>800</maxWorkerThreads>
      <minWorkerThreads>800</minWorkerThreads>
    </config>
    <http>
      <server port="4080" id="myserver">
      </server>
    </http>
    <nodes>
            <jvm allocated-memory="3%" />
    #################################################################
     ######  00 ~29, total 30 hosts #########################################
     #################################################################
          </nodes>
  </container>

  <content id="<OurProductID>" version="1.0">
    <redundancy>2</redundancy>
    <documents>
      <document type="<OurProductID>" mode="index"/>
    </documents>

    <engine>
      <proton>
        <searchable-copies>2</searchable-copies>
        <tuning>
          <searchnode>
            <requestthreads>
              <search>256</search>
              <persearch>8</persearch>
              <summary>32</summary>
            </requestthreads>
            <index>
              <io>
                <search>populate</search>
              </io>
            </index>
          </searchnode>
        </tuning>
      </proton>
    </engine>

    <nodes>
    #################################################################
     ######  00 ~29, total 30 hosts #########################################
     #################################################################
    </nodes>
  </content>
</services>
```
