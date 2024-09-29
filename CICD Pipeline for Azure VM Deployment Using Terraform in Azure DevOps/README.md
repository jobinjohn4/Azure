# CI/CD Pipeline for Azure VM Deployment Using Terraform in Azure DevOps
This project aims to automate the deployment of virtual machines (VMs) in Azure by leveraging Azure DevOps and Terraform within a CI/CD pipeline. The pipeline will facilitate the seamless provisioning and management of Azure VMs through Infrastructure as Code (IaC), ensuring consistent and repeatable deployments.
The project will involve creating a Terraform configuration that defines the VM specifications, network settings, and other required resources. Azure DevOps will be utilized to set up the CI/CD pipeline, which will include stages for validating the Terraform code, executing the deployment, and managing any necessary approvals. This automation will not only streamline the deployment process but also improve collaboration among development and operations teams.

![alt text](image.png)
## Creating new project in Azure DevOps
![alt text](image-2.png)

## 	Pushing Terraform Files to Azure Git Repository
![alt text](image-3.png)
### Creating terraform.tfvars file
![alt text](image-4.png)
## Creating a Build pipeline on Azure DevOps
![alt text](image-5.png)
## Created storage account for backend process
![alt text](image-6.png)
## Setting Up a Container in the Newly Created Storage Account
![alt text](image-7.png)
## Adding task in build pipeline in YAML : terraform init
![alt text](image-8.png)
##  Adding task in build pipeline in YAML : terraform validate
![alt text](image-9.png)
##  Adding task in build pipeline in YAML : terraform fmt
![alt text](image-10.png)
##  Adding task in build pipeline in YAML : terraform plan
![alt text](image-11.png)
## Archiving the file
![alt text](image-12.png)
## Publishing the Artifact
![alt text](image-13.png)
## Save and Run the build pipeline
![alt text](image-14.png)
## The build pipeline has completed successfully
![alt text](image-15.png)
## Building Release pipeline
![alt text](image-16.png)
![alt text](image-17.png)
## Creating contineous deploymeny pipeline

![alt text](image-18.png)
## Creating destroy stage
![alt text](image-19.png)
## Adding predeployment approval and assigning a approver
![alt text](image-20.png)
## Release pipeline is completed
![alt text](image-21.png)
## Running the build and release pipeline
![alt text](image-22.png)
## The Virtual Machine has been successfully built in Azure portal
![alt text](image-23.png)
# Conclusion
 this project, we successfully automated the deployment of a virtual machine (VM) in Azure using a Continuous Integration/Continuous Deployment (CI/CD) pipeline with Terraform and Azure DevOps. By leveraging Infrastructure as Code (IaC) principles, we ensured consistent and repeatable VM provisioning, which streamlined the deployment process and reduced the potential for manual errors.

The integration of Terraform with Azure DevOps facilitated a seamless workflow, from code updates to deployment, enhancing collaboration between development and operations teams. With the successful creation of the storage account, container, and VM, the project demonstrates the effectiveness of modern DevOps practices in managing cloud infrastructure efficiently.
