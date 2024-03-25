Azure Kubernetes Service (AKS) Deployment with Terraform

Introduction:
This repository provides a streamlined guide and Terraform configuration files for deploying an Azure Kubernetes Service (AKS) cluster effortlessly using Terraform. AKS, built on Kubernetes, offers a managed solution for container orchestration within the Microsoft Azure cloud platform. Leveraging Terraform, an infrastructure as code tool, simplifies and automates the AKS cluster creation process.

Pre-requisites:
Before initiating the deployment process, ensure the following pre-requisites are met:

    Installation of Terraform on your local machine.
    Access to a valid Azure subscription.
    Kubectl and Azure CLI installed for seamless interaction with Azure resources.

Steps for Deployment:

    Login to Azure: Begin by logging into the Azure portal using your credentials.
    Configure Terraform Files:
        Define variables in variables.tf.
        Declare variable values in terraform.tfvars.
        Specify providers and versions in providers.tf.
        Configure the main resources in main.tf.
        Export relevant data in output.tf.
    Execute Terraform Commands:
        Run terraform init to initialize the project.
        Validate the configuration using terraform validate.
        Preview the execution plan with terraform plan.
        Apply the configuration changes with terraform apply.
    Post-Deployment Verifications:
        Move the generated Kubeconfig file to ~/.kube/config.
        Verify the status of worker nodes using kubectl get nodes.
    Deploy Applications to AKS Cluster:
        Deploy applications like Nginx using kubectl create.
        Check deployment status and list pods with respective commands.
    Cleanup Operations:
        To avoid unnecessary charges, execute terraform destroy --auto-approve to remove all created resources.

Additional Notes:

    Ensure to replace placeholder values in Terraform files with actual values corresponding to your Azure environment.
    Customize and extend the deployment process as per specific requirements.

Contributing:
Contributions, issues, and feature requests are welcome. Feel free to create pull requests or raise any concerns via GitHub issues.


