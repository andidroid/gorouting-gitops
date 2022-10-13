# gorouting-gitops

## Working with library charts
https://helm.sh/docs/topics/library_charts/

helm create mylibchart
helm dependency update mychart/
helm install mydemo mychart/ --debug --dry-run
helm install mydemo mychart/
helm get manifest mydemo



$ helm dependency update .
$ helm template test .
$ helm lint .

helm install ... -n fleet
 
helm install routingservice ./charts/routingservice/ --values env-values.yaml
helm upgrade routingservice ./charts/routingservice/ --values env-values.yaml
helm install fleetservice ./charts/fleetservice/ --values env-values.yaml
helm upgrade fleetservice ./charts/fleetservice/ --values env-values.yaml
helm install searchservice ./charts/searchservice/ --values env-values.yaml 
helm upgrade searchservice ./charts/searchservice/ --values env-values.yaml
helm install messagingservice ./charts/messagingservice/ --values env-values.yaml
helm upgrade messagingservice ./charts/messagingservice/ --values env-values.yaml


helm dependency update ./charts/routingservice/
helm dependency update ./charts/fleetservice/
helm dependency update ./charts/searchservice/
helm dependency update ./charts/messagingservice/

## helm repo url
helm repo add gorouting-gitops https://andidroid.github.io/gorouting-gitops
https://andidroid.github.io/gorouting-gitops/index.yaml