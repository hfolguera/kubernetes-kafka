Installation:
```
kubectl apply -f kafka-namespace.yaml
kubectl apply -f kafka-volumes.yaml
helm repo add bitnami https://charts.bitnami.com/bitnami
helm install kafka bitnami/kafka -n kafka -f values.yaml
```


Notes:
 Storage configuration:
   chown -R 1001:1001 kafka
   chmod -R 777 kakfa
