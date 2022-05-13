#### basic

`node/nodes/no`

`compontentstatuses/cs`

`namespaces/ns`

`pods/pod/po`

___

`kubectl get ns`

`kubectl get pod -n $namespaces`

`kubectl get service -n $namespaces`

`kubectl logs -f $pod -n $namespaces`

___

#### docker

docker ps

清理磁盘，删除关闭的容器、无用的数据卷和网络，以及dangling镜像(即无tag的镜像)

`docker system prune`
