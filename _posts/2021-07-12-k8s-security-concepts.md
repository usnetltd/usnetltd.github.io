---
layout: post
title:  "Overview of Cloud Native Security"
author: sal
categories: [ Big-Data, Cyber, Kubernetes, Container Security ]
image: assets/images/4c.png
---
## The 4C's of Cloud Native security 
The 4C's of Cloud Native security are 
- Cloud
- Clusters
- Containers
- Code

![K8s Security]({{ site.baseurl }}/assets/images/4c.png "K8s Security")

Each layer of the Cloud Native security model builds upon the next outermost layer. The Code layer benefits from strong base (Cloud, Cluster, Container) security layers. You cannot safeguard against poor security standards in the base layers by addressing security at the Code level.

## Cloud
In many ways, the Cloud (or co-located servers, or the corporate datacenter) is the trusted computing base of a Kubernetes cluster. If the Cloud layer is vulnerable (or configured in a vulnerable way) then there is no guarantee that the components built on top of this base are secure. Each cloud provider makes security recommendations for running workloads securely in their environment.

## Cluster
There are two areas of concern for securing Kubernetes:

- Components OF the Cluster
- Components IN the cluster (your application)

## Container
Area of Concern for Containers
- Container Vulnerability Scanning and OS Dependency Security
- Image Signing and Enforcement
- Disallow privileged users	
- Use container runtime with stronger isolation

![Static Code Analysis]({{ site.baseurl }}/assets/images/static_code.png "Static Code Analysis")

## Code
Application code is one of the primary attack surfaces over which you have the most control. While securing application code is outside of the Kubernetes security topic including (Code Security)
- Access over TLS only
- Limiting port ranges of communication
- 3rd Party Dependency Security
- Static Code Analysis
- Dynamic probing attacks




