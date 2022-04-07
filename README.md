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