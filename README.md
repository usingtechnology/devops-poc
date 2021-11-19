# devops-poc
prototyping devops for openshift4

Basing initial tekton pr pipeline on https://www.arthurkoziel.com/tutorial-tekton-triggers-with-github-integration

## install pipeline
Assume access and privileges to the openshift4 namespace...

```
kubectl apply -f tekton/
```

### list all task runs

tkn tr ls

### delete all task runs

kubectl delete tr --all

### get last task run logs

tkn tr logs -f -a $(tkn tr ls | awk 'NR==2{print $1}')

### list all pipeline runs

tkn pr ls

### delete all pipeline runs

kubectl delete pr --all
