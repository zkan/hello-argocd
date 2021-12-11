# Hello, Argo CD!

```sh
kubectl apply -f application.yaml
```

Try to edit the deployment:

```sh
kubectl edit deployment -n myapp myapp-deployment
```

We'll see that Argo CD will revert back to the desired state.