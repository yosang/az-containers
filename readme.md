# About
This repo holds notes for a simple workflow of creating an image from a Dockerfile, pushing it to an `Azure Container Registry` and finally deploying it.

The workflow is divided into  multiple steps:

## Step 1: Registry management
We will create a private `Azure Container Registry` resource and a storage account for our images through the `Azure Portal` on `portal.azure.com`

## Step 2: Registry authentication
We will authenticate our new registry with `Docker` through the `Azure CLI` using the following command: `az acr login -n [registry_name]`

## Step 3: Image Management
We will use this fork https://github.com/yosang/aci-helloworld, do some changes on it, build it with the `Dockerfile`, then push it to our `Azure Contaner Registry`.

## Step 4: Instance Deployment
We will create a new `Azure Container Instance` resource through the `Azure Potal` on `porta.azure.com` and deploy the image created from our private registry.

## Step 5: Cost management
We will analyze and inspect the current cost of our running container, as well as forecast for the next quarter.