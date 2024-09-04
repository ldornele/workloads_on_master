# workloads_on_master

Depliyment example with Node Selector, Toleration, request and limits resources

Commands to evaluate:

- oc adm top nodes
- oc get node <node>  -o json | jq .' | .status.capacity'| grep cpu
- oc get node <node>  -o json | jq .' | .status.capacity'| grep memory
- oc describe node/<node>

- for i in {1..100}; do curl -k <http://namespace.wildcard>; done;
