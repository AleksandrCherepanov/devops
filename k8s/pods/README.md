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

Execute command in a pod:
```bash
kubectl exec -it {pod_id} -- {command} (bash, env, etc)
```

Open ports for an application in a pod (developing purpose only)
& - background process
```bash
kubectl port-forward {pod} {local_port:pod_port} &
```

