# ai-homelab
## Pre-requisites
helm repo add open-webui https://helm.openwebui.com

helm repo add kestra https://helm.kestra.io/
### install steps
```
helm install my-open-webui open-webui/open-webui --version 3.0.1 -f helm/openwebui/values.yaml 

helm install n8n --version 3.0.1 -f helm/n8n/values.yaml

helm install my-n8n oci://8gears.container-registry.com/library/n8n --version 0.23.1 -f helm/n8n/values.yaml 

helm install kestra kestra/kestra -f helm/kestra/values.yaml
```




