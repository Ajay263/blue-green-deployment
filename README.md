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


### Retrieve password from secrets for grafana 


```
kubectl get secret -n monitoring prom-grafana -o jsonpath="{.data.admin-password}" | base64 --decode ; echo
```
### Access  Prometeheus 

```
kubectl port-forward -n monitoring svc/prom-kube-prometheus-stack-prometheus 9091:9090

```

```
kubectl get all -n ingress-nginx
```


