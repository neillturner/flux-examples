# flux-examples
Flux V2 kubernetes examples 

## Overview 

Examples of Flux V2 definitions.

A good way of build AWS EKS is to use terraform to create and update the AWS resources and use Flux V2
to create and update the kubernetes resources using public available helm charts. This creates a simplicity to the complexity of create and updating AWS EKS clusters.  

## Repository Contents 

### actions-runner-controller directory 

Contains an example for defining a self-hosted github actions runner in kubernetes (EKS).

I have not been able to get the supplied runner images to work:
- https://hub.docker.com/r/summerwind/actions-runner
- https://hub.docker.com/r/summerwind/actions-runner-dind
and generally they don't meet your specific requirements for its necessary to build your own runner docker image. See: 
- https://github.com/ministryofjustice/docker-github-actions-runner
- https://github.com/myoung34/docker-github-actions-runner

### github-actions-exporter directory 

Contains an example for defining a github actions exporter for prometheus metrics in kubernetes (EKS).


### prometheus directory 

Contains an example for defining a Prometheus server in kubernetes (EKS) to forward metrics to an AWS Managed Prometheus.

## References 

- [https://neillwturner.medium.com/github-actions-self-hosted-runners-on-kubernetes-2cc0da04d41a](https://neillwturner.medium.com/github-actions-self-hosted-runners-on-kubernetes-2cc0da04d41a)

- [https://github.com/actions-runner-controller/actions-runner-controller](hhttps://github.com/actions-runner-controller/actions-runner-controller)

- [https://github.com/Spendesk/github-actions-exporter](https://github.com/Spendesk/github-actions-exporter)

- [https://aws.amazon.com/blogs/mt/getting-started-amazon-managed-service-for-prometheus/](https://aws.amazon.com/blogs/mt/getting-started-amazon-managed-service-for-prometheus/)


