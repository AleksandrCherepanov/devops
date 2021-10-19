Create a secret:
```bash
kubectl create secret {type} {name} --from-literal=test1=asdf --from-literal=password=123456
```

Get a secret:
```bash
kubectl get secret
```
