## Open5GS on K8

This project deploys a Open5GS 4G/LTE core on the Kubernetes Infrastructure. Make the adjustments to the service files under each folder and then run the project.

Usage
-------------

1. Edit the configuration files under each directory.
2. Create Persistent Storage for the pods by applying the manifests. First check its values and make the required changes before applying.
```
kubectl apply -f PersistentStorage/
```
3. Apply the manifests to the K8 API in order to create the pods.
```
kubectl apply -f hss/
```
```
kubectl apply -f mme/
```

Confirmation
------------

- Check the status of running pods
```
kubectl get pods -A
````
