# dest-addr-cis-example
This is a small repo intended to host files for a customer demo

## Instructions
### CIS must be running
1. Deploy CIS. This can be done with the file included, or CIS may be pre-installed. 
2. Ensure CIS is deployed *without* the ````--custom-resource-mode```` flag, or set this flag to ````false````
3. Ensure CIS is deployed *with* the ````--manage-configmaps=true```` flag

### Deploy a service to be exposed with labels
1. If you need, a demo app can be deployed with the file ````demo_app.yaml````
2. Notice the labels on the service in the example provided. The configMap will need to match these.

### Deploy a configMap
1. Deploy the configMap using the file ````as3-configMap.yaml````

### Observe CIS functions 
1. CIS will create a VirtualServer on BIG-IP using the declaration from the configMap.
