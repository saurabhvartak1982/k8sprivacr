# Access Azure Container Registry (ACR) using Azure Private Link from a Kubernetes cluster hosted in a separate environment

## Aim:
To access Azure Container Registry (ACR) using Azure Private Link from a Kubernetes cluster hosted at on-prem/Azure-on-different-tenant/other-cloud-platforms.

## Backdrop: 
For better security, ACR endpoints should always be accessed over a private IP address. This is made possible using Azure Private Link where a private IP address from a Virtual Network is assigned to the ACR endpoint. <br />
However, the challenge comes when the same ACR endpoint needs to be accessed from a different hosting environment like an Azure Subscription belonging to a different tenant, an on-prem or a different cloud platform. <br /> <br />
This article aims to explain one of the reference architectures to address this challenge.<br />

## Reference Architecture:
![SolutionArchitecture](images/SolutionArchitecture.png)
