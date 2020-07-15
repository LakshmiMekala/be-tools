---
title: Kubernetes
weight: 4200
# chapter: true
# pre: "<i class=\"fas fa-cloud\" aria-hidden=\"true\"></i> "
---

## Running TIBCO BusinessEvents Applications in Kubernetes

Kubernetes is an open-source platform designed to automate deploying, scaling, and operating application containers. Kubernetes can run application containers on clusters of physical or virtual machines.

For more information about Kubernetes, see [Kubernetes documentation](https://kubernetes.io/docs/home/).

In TIBCO BusinessEvents, to form a cluster, discovery nodes starts a cluster and other non-discovery nodes (cache and inference). These non-discovery nodes connect to one or more discovery nodes and become a member of the cluster. In Kubernetes, each TIBCO BusinessEvents node runs as a Kubernetes pod. Pods communicate with each other by using their IP addresses. However, due to the dynamic nature of the IP addresses, non-discovery nodes cannot always connect to discovery nodes. Thus, to resolve this issue, discovery nodes are modeled as Kubernetes services. The service is reachable by its name by using the Kubernetes DNS. Non-discovery nodes use indirection by using the Kubernetes service to connect to discovery nodes. 

* OpenShift Container Platform Based Kubernetes
* Pivotal Based Kubernetes