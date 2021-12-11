# Hello, Argo CD!

Install Argo CD

```sh
kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
```

or

```
kubectl create namespace argocd
kubectl apply -n argocd -f install.yaml
```

Create Argo CD Application

```sh
kubectl apply -f application.yaml
```

Try to edit the deployment:

```sh
kubectl edit deployment -n myapp myapp-deployment
```

We'll see that Argo CD will revert back to the desired state.
