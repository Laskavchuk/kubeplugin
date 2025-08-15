## Плагін `kubectl kubeplugin`

Плагін для отримання статистики CPU та пам’яті з Kubernetes (на основі `kubectl top`).

### Встановлення
```bash
chmod +x kubectl-kubeplugin
mkdir -p ~/.kube/plugins
mv kubectl-kubeplugin ~/.kube/plugins/
export PATH=$PATH:~/.kube/plugins
```

### Використання
```
kubectl kubeplugin <namespace> <resource_type>
```

### Приклад виводу
```
Resource, Namespace, Name, CPU, Memory
pods, kube-system, coredns-565d847f94-6z4rt, 2m, 10Mi
pods, kube-system, metrics-server-5f9f776df-abc12, 1m, 15Mi
```
