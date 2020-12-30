### prometheus

- 部署：

```bash
# cd prometheus/
[root@k8s-master prometheus]# kubectl apply -f  public-service-ns.yaml
[root@k8s-master prometheus]# kubectl apply -f node-exporter/
[root@k8s-master prometheus]# kubectl apply -f kube-state-metrics/
[root@k8s-master prometheus]# kubectl apply -f blackbox-exporter/
[root@k8s-master prometheus]# kubectl apply -f dingtalk/
[root@k8s-master prometheus]# kubectl apply -f alertmanager/
[root@k8s-master prometheus]# kubectl apply -f prometheus/
[root@k8s-master prometheus]# kubectl apply -f grafana/
---
