Get information about a ReplicaSet:
```bash
kubectl describe replicaset {name}
```

Get list of  ReplicaSets:
```bash
kubectl get replicaset
kubectl get rs
```

Increase or decrease amount of pods in a ReplicaSet:
```bash
kubectl scale --replicas 3 replicaset my-replicaset
```

Update image inside a ReplicaSet (it just changes template inside a ReplicaSet's spec, all pods must be recreated for using new image):
```bash
kubectl set image replicaset {name of replicaset} {name of container}={image}
kubectl set image replicaset {name of replicaset} *={image}
```
