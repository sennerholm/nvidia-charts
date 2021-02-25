# matlab

Mathworks Matlab chart to be used on DGX, as standard create a disk with "100Gi" mounted in /data and using one nvidia GPU.

## TL;DR

To start

```console
helm repo add nvidia-charts https://sennerholm.github.io/nvidia-charts
helm repo update
helm install matlab nvidia-charts/matlab
```

To scale down
```console
kubectl scale deployment matlab --replicas=0
```

Delete
```console
helm uninstall matlab
```