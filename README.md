# k3d-helm
run kubernetes cluster in codespace

TLDR;

```
pip install -r requirements.txt
ansible-playbook playbook.yml

```

I did struggle with actually seeing the service outside of the dev container. If the service port is 80 and you want to access on 8080, you can run:

```
kubectl port-forward svc/<what you called your service> 8080:80

```

To delete a cluster (and start over):

```
k3d cluster delete local-k8s
```

Use this as a template and then add helm charts to the playbook.yml as required.
