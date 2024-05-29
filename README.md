# flux-primer
Repository used as a primer to [flux.io](https://fluxcd.io)

This repository is used as an introduction to flux and some very basic usage. 

Simplifications:
* No private gitlab or s3 bucket sources
* no patching

Deploying:
- prepare Kubernetes cluster
- `kubectl create ns flux-system`
- `kubectl apply -f clusters/flux-primer/flux-system/gotk-components.yaml`
- `kubectl apply -f clusters/flux-primer/flux-system/gotk-sync.yaml`
