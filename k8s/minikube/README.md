Build an image inside minikube
```bash
minikube image build {path} -t {name}:{version}
```

Mount some directory into minikube
```bash
minikube mount {host_path}:{minikube_path}
```

Run application using a service
```bash
minikube service {name}
```
