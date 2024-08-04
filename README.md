# k3d-helm
run kubernetes cluster in codespace

TLDR;

```
k3d cluster create local-k8s

```

To delete a cluster:

```
k3d cluster delete local-k8s
```

kubectl get nodes

kubectl -n default apply -f kube/admin-user.yml

helm repo add kubernetes-dashboard https://kubernetes.github.io/dashboard

helm install dashboard kubernetes-dashboard/kubernetes-dashboard

kubectl get pods
```
Then with the 0th pod, dashboard-kong-68687498db-5jk5m

```
kubectl -n default port-forward dashboard-kong-68687498db-5jk5m 8443:8443

kubectl -n default create token admin-user
```

My plan is to use this for a course on monitoring and logging (with open telemetry).