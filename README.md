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

kubectl port-forward service/vote 8081:30100



```
kubectl get all -n ingress-nginx
```
  ### Current Admin password

  ```
   kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d; echo
   ```
