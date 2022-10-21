使用prometheus抓去etcd数据是需要提前挂在证书


kubectl  -n prometheus  create  secret  generic etcd-certs --from-file=/etc/kubernetes/pki/etcd/server.key  --from-file=/etc/kubernetes/pki/etcd/server.crt --from-file=/etc/kubernetes/pki/etcd/ca.crt
