Create a pod from a file:
```bash
kubectl create -f pod.yaml
```

Update or create a pod from a file:
```bash
kubectl apply -f pod.yaml
```

Get information about a pod:
```bash
kubectl describe pod {name}
```

Get list of pods:
```bash
kubectl get pod
```

Delete a pod:
```bash
kubectl delete pod {name}
kubectl delete -f pod.yaml
```
