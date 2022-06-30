# redis-cluster
ansible-playbook redis_cluster_yml 

Добавление узлов в кластер:

redis-cli --cluster create master1ip:6379 master2ip:6379 master3ip:6379 slave1ip:6379 slave2ip:6379 slave3ip:6379 --cluster-replicas 1 

Check кластера:

redis-cli -c -h 10.0.1.4 -p 6379 cluster nodes
