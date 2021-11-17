# devops-poc
prototyping devops for openshift4

Basing initial tekton pr pipeline on https://www.arthurkoziel.com/tutorial-tekton-triggers-with-github-integration

## install pipeline
Assume access and privileges to the openshift4 namespace...

```
kubectl apply -f tekton/
```