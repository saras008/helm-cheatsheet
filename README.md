#Use helm template for Debugging

helm template myrelease ./mychart

#Use helm lint to Validate Charts
helm lint ./mychart
note : use this command always before installing, check for syntax errors on our chart.

helm list

helm get all myapp

helm rollback myapp 1

helm install --generate-name ./mychart
*when deploying multiple instances of the same chart

helm install myapp ./mychart --create-namespace --namespace mynamespace

helm upgrade myapp ./mychart --atomic --cleanup-on-fail

