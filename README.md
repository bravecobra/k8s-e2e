# k8s-e2e

This repo demonstrates the usage of `Github Actions`, spinning up local `kubernetes` clusters and running workloads against them.

The example being used here is running a `traefik` reverse proxy before a `whoami` deployment. In `Github Actions` the `whoami` deployment is accessible and therefor testable from outside the cluster.

There are ~~3~~ 2 kinds on cluster showcased

* k3s
* kind
* ~~minikube~~

The way `minikube` exposes services makes it a lot harder to grab the deployment from outside the cluster. Accessing it through DNS resolution is a requirement on my end so I eliminated it as a viable option for my use-case.
