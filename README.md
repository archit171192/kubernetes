# kubernetes

PODS:

kubectl create -f pod-definition.yml
kubectl get pods
kubectl get pods -o wide (to see ip of pod and on which node it is deployed)
kubectl describe pod POD_NAME (additional info about pod)

* Replica Sets:

kubectl create -f replicaset-definition.yml
kubectl get replicaset (get all replica sets)
kubectl get pods (get all pods)

kubectl describe replicaset (additional info about replica sets)
kubectl delete pod POD_NAME (to delete a pod)
kubect replace -f replicatset-definition.yml (update #replicas)
kubectl scale --replicas=4 -f replicaset-definition.yml (update #replicas)
kubectl delete replicaset REPLICASET_NAME
