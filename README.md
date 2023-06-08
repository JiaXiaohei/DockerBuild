# Dockerfile

#### NETWORK
##### bridge
```
docker network create -d bridge --subnet=172.18.0.0/16 bridge_network
```
##### macvlan
```
docker network create -d macvlan --subnet=172.16.0.0/16 --gateway=172.16.0.6 -o parent=ovs_eth0 macvlan_ovs_eth0
```