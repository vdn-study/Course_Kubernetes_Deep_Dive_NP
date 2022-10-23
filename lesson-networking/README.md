## Recap
* Service Type:
  * ClusterPort
  * NodePort
  * LoadBlancer

## Usage

```sh
# Create app
kubectl apply -f ping-deploy.yml

# Get the CIDR of nodes
kubectl get nodes -o jsonpath='{.items[*].spec.podCIDR}'
kubectl get nodes -o wide

# run bash inside the pod to check netwoking
kubectl exec -it pingtest-84646bf5d4-26rdf bash
apt update
apt install iputils-ping curl dnsutils iproute2 -y
```
