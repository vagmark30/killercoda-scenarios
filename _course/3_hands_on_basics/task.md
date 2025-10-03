## Run a Pod

`kubectl run nginx --image=nginx`{{exec}}

This creates a Pod running the nginx container.

## Inspect the Pod
There are multiple ways we can inspect a pod.

- `kubectl get pods`{{exec}} shows all Pods.
- `kubectl get pods -n default` shows all Pods on default namespace.
- `kubectl get pods --all-namespaces`{{exec}} shows all Pods on all namespaces.
- `kubectl get pods -A`{{exec}} similar shows all Pods on all namespaces.
- `kubectl describe pod nginx`{{exec}} gives details about the Pod (events, IP, status, etc.).
- `kubectl get pod nginx -o yaml`{{exec}} gives the definition file of the Pod

## Delete the Pod

`kubectl delete pod nginx`{{exec}}
