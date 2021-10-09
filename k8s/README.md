Get documentation in a terminal:
```bash
kubectl explain {{entity}} (pod, replicaset, etc)
kubectl explain {{entity.attr}} (pod.spec)
```

Edit a spec of entity inside k8s:
```bash
kubectl edit {entity} {entity_name}
```

Undo changes of an entity:
```bash
kubectl rollout undo {entity} {entity_name}
```

Get history of an entity:
```bash
kubectl history {entity} {entity_name}
```
