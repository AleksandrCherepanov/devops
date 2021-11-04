Create a secret:
```bash
kubectl create secret {type} {name} --from-literal=test1=asdf --from-literal=password=123456
```

Create a tls secret:
```bash
kubectl create secret {type} {name} --key {key_file} --cert {cert_file} 
```

Get a secret:
```bash
kubectl get secret
```
