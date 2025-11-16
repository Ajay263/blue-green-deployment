### Port forwarding Kubernetes Visualizer

```
kubectl port-forward service/kube-ops-view 8080:80
```


### Access Argocd Dashboard

```
kubectl port-forward svc/argo-rollouts-dashboard 8080:3100 -n argo-rollouts
```

### Check rollouts 

```
kubectl  argo rollouts list rollouts 
```

```
kubectl  argo rollouts get  rollouts vote
```



