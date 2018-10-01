# redis-HA-cluster-slave

目前支持架構：
------
1. master-slave + 哨兵 <br>
2. redis-cluster (未來會再加入, 目前無法運行) <br>
<br>
佈署前設定 : 
------
檔案位址 : docker-compose/master-slave-redis/host1/sentinel.conf (host2跟host3也記得設定好IP) <br>
設定sentinel.conf 內的IP位址 <br>
務必確保三台安裝時每台設定的IP正確 <br>
<br>
佈署:
------

進到docker-compose/master-slave-redis/host1/下運行每yaml檔
目前是以三台為範例 :

    docker-compose -f docker-compose-master-slave.yaml up -d
    
