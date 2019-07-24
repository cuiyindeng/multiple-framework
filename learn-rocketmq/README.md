
     namesrvAddr=192.168.152.128:9876;192.168.152.129:9876
     brokerClusterName=DefaultCluster
     brokerName=broker-a
     brokerId=0
     deleteWhen=04
     fileReservedTime=48
     brokerRole=SYNC_MASTER
     flushDiskType=ASYNC_FLUSH
     listenPort=10911
     storePathRootDir=/opt/rocketmq/store-a


     nohup sh bin/mqnamesrv &
     sh bin/mqshutdown namesrv

     nohup sh bin/mqbroker -c conf/2m-2s-sync/broker-a.properties &