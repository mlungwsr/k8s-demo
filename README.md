# Orchestrating the Cloud with Kuberenetes

In this lab you will learn how to:

* Deploy and manage Docker containers using kubectl

Kubernetes Version: 1.2.2

### Clone this Repository

Login into your Cloud Shell environment and clone this repository.

```
$ git clone git@github.com:WesleyCharlesBlake/k8s-demo.git
$ cd k8s-demo
$ git checkout orchestrate-k8s
```

## Provision Kubernetes [TODO]

Kubernetes is a distributed system composed of a collection of microservices. Like any system Kubernetes must be installed and configured. In this section you will install Kubernetes from the ground up with the minimal configuration required to get a cluster up and running.

Kubernetes can be configured with many options and add-ons, but can be time consuming to bootstrap from the ground up. In this section you will bootstrap Kubernetes using [EKS](https://aws.amazon.com/eks/)


## Managing Applications with Kubernetes

Kubernetes is all about applications and in this section you will utilize the Kubernetes API to deploy, manage, and upgrade applications. In this part of the workshop you will use an example application called "app" to complete the labs.

[App](https://github.com/kelseyhightower/app) is hosted on GitHub and provides an example 12 Facter application. During this workshop you will be working with the following Docker images:

* [kelseyhightower/monolith](https://hub.docker.com/r/kelseyhightower/monolith) - Monolith includes auth and hello services.
* [kelseyhightower/auth](https://hub.docker.com/r/kelseyhightower/auth) - Auth microservice. Generates JWT tokens for authenticated users.
* [kelseyhightower/hello](https://hub.docker.com/r/kelseyhightower/hello) - Hello microservice. Greets authenticated users.
* [ngnix](https://hub.docker.com/_/nginx) - Frontend to the auth and hello services.

#### Labs

For each of the following labs, you should be in the kubernetes dir:
```
cd orchestrate-with-kubernetes/kubernetes
```

  * [Creating and managing pods](labs/creating-and-managing-pods.md)
  * [Monitoring and health checks](labs/monitoring-and-health-checks.md)
  * [Managing application configurations and secrets](labs/managing-application-configurations-and-secrets.md)
  * [Creating and managing services](labs/creating-and-managing-services.md)
  * [Creating and managing deployments](labs/creating-and-managing-deployments.md)
  * [Rolling out updates](labs/rolling-out-updates.md)

## Links

  * [Kubernetes](http://googlecloudplatform.github.io/kubernetes)
  * [gcloud Tool Guide](https://cloud.google.com/sdk/gcloud)
  * [Docker](https://docs.docker.com)
  * [etcd](https://coreos.com/docs/distributed-configuration/getting-started-with-etcd)
  * [nginx](http://nginx.org)
