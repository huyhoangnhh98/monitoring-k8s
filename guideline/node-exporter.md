https://devopscounsel.com/prometheus-node-exporter-setup-on-kubernetes/

## Tạo namespace monitoring
```sh
kubectl create namespace monitoring
```

## Thực hiện apply demon set vào trong k8s
```sh
cd k8s-node-exporter

kubectl apply -f daemonset.yaml -n monitoring
```

## Thực hiện apply service vào trong k8s
```sh
kubectl apply -f service.yaml -n monitoring
```
