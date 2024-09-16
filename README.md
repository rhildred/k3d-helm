# k3d-helm
run kubernetes cluster in codespace

TLDR;

```
pip intall -r requirements.txt
ansible-playbook playbook.yml

```

To delete a cluster:

```
k3d cluster delete local-k8s
```

Use this as a template and then add helm charts to the playbook.yml as required.
