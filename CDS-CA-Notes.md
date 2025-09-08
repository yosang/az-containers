# Setup

We are going to pull a repo from git, edit it and push it to an Azure Registry. Finally we are going to deploy an instance from the created image.
### Preparations
- Remove all existing resources
- Reset azure cloudshell

# Tasks
- Take a screenshot of each step, to be provided in the CA.

<details><summary>Storage account and Cloudshell</summary>

- Create storage account and fileshare for cloudshell

- initiate Azure Cloud Shell Instance and use mount created fileshare

**Resources:** 

- https://learn.microsoft.com/en-us/azure/cloud-shell/get-started/classic?tabs=azurecli

- https://learn.microsoft.com/en-us/azure/cloud-shell/persisting-shell-storage

</details>

<details>
<summary>Container registry</summary>

- Create a container registry and use created storage account

- Give it admin access

- Authenticate the registry with docker

**Resources**
- https://learn.microsoft.com/en-us/azure/container-registry/
</details>

<details>
<summary>Container management</summary>

- Pull image from git
	- https://github.com/Azure-Samples/aci-helloworld

- List the contents of the application

- Change the `H1` text to `This is the Maltese Azure Window that collapsed in 2017`

- Change the `SVG` image to `https://upload.wikimedia.org/wikipedia/commons/thumb/e/ec/Azure_Window_2009.JPG/800px-Azure_Window_2009.JPG`

- Build the image with docker

- Tag the image and push it to the registry

- Create a container instance from created omage and deploy it

**Resources**

- https://learn.microsoft.com/en-us/azure/container-registry/container-registry-get-started-docker-cli?tabs=azure-cli
</details>

<details><summary>Cost</summary>
- Check the actual cost of the current solution and forecast for the next quarter.
</details>