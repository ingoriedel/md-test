```shell
[root@dlp ~]# microk8s add-node
From the node you wish to join to this cluster, run the following:
microk8s join 10.0.0.30:25000/e4d12ddd881447063bfb7aa157989737

If the node you are adding is not reachable through the default interface you can use one of the following:
 microk8s join 10.0.0.30:25000/e4d12ddd881447063bfb7aa157989737

# if Firewalld is running, allow ports
[root@dlp ~]# firewall-cmd --add-port={25000/tcp,16443/tcp,12379/tcp,10250/tcp,10255/tcp,10257/tcp,10259/tcp} --permanent
[root@dlp ~]# firewall-cmd --reload
```
