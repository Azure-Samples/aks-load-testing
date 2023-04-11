# Azure Load Testing and Azure Kubernetes Service Demo

This demo project showcases an automated load testing solution for Azure Kubernetes Service that acts as a release gate for a minimal SLO (Service Level Objective). There is also an example of a test configuration matrix for using Azure Load Testing to identify a right-size Pod configuration.

The application is a simple web application based on the [Deploy an Azure Kubernetes Service cluster using the Azure CLI](https://learn.microsoft.com/en-us/azure/aks/learn/quick-kubernetes-deploy-cli) quick start tutorial.

## Features

This project framework provides the following features:

* [Example GitHub workflow](.github/workflows/cicd.yml) to staging an image, running a load test and then promoting the image to a production deployment in AKS.
* [Example GitHub workflow](.github/workflows/matrix_test.yml) for periodically running a load test matrix to identify a right-size Pod configuration.

## Getting Started

### Prerequisites

* An [Azure subscription](https://azure.microsoft.com/free/)
* An [Azure Kubernetes Service](https://learn.microsoft.com/en-us/azure/aks/) cluster
* An [Azure Container Registry](https://learn.microsoft.com/en-us/azure/container-registry/) instance
* An [Azure Load Testing](https://learn.microsoft.com/en-us/azure/load-testing/) instance

### Configuring

The following secrets are required for the GitHub workflow:

* `AZURE_CREDENTIALS` - An SDK service principal with stored
* `AZURE_RESOURCE_GROUP_NAME` - The resource group with the Load Testing instance.
* `AZURE_LOAD_TEST_NAME` - The name of the Azure Load Testing instance.
* `ACR_LOGIN` and `ACR_SECRET` - Azure Container Registry credentials.
* `AKS_NAME` - The name of the AKS cluster.

#### Configuring the service principal

...

## Demo

A demo app is included to show how to use the project.

To run the demo, follow these steps:

(Add steps to start up the demo)

1.
2.
3.

## Resources

(Any additional resources or related projects)

* Link to supporting information
* Link to similar sample
* ...
