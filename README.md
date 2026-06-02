# Azure AKS Infrastructure with CI/CD Pipeline

End-to-end infrastructure-as-code project demonstrating Azure Kubernetes Service (AKS) cluster provisioning using Terraform, with automated CI/CD pipelines via Azure DevOps.

## Architecture

- **Infrastructure**: Azure AKS cluster provisioned via Terraform modules
- - **CI/CD**: Azure Pipelines for infrastructure deployment and application delivery
  - - **Application**: Containerized Nginx application deployed to AKS
    - - **Container Registry**: Docker image build and push pipeline
     
      - ## Project Structure
     
      - ```
        terraform/          # Terraform modules for AKS infrastructure
        pipelines/          # Azure DevOps YAML pipeline definitions
        k8s-manifests/      # Kubernetes deployment manifests
        src/                # Application source code
        Dockerfile          # Container image definition
        ```

        ## Tech Stack

        - **IaC**: Terraform
        - - **Cloud**: Microsoft Azure (AKS, ACR, VNet, NSG)
          - - **CI/CD**: Azure DevOps Pipelines
            - - **Container Orchestration**: Kubernetes
              - - **Containerization**: Docker
               
                - ## Prerequisites
               
                - - Azure CLI
                  - - Terraform >= 1.0
                    - - kubectl
                      - - Docker
                        - - Azure DevOps organization with service connection
                         
                          - ## Getting Started
                         
                          - 1. Clone the repository
                            2. 2. Configure Azure credentials via `az login`
                               3. 3. Update `terraform.tfvars` with your environment values
                                  4. 4. Run Terraform to provision infrastructure
                                     5. 5. Configure Azure DevOps pipeline with the provided YAML definitions
                                        6. 6. Deploy the application via the CI/CD pipeline
                                          
                                           7. ## Key Features
                                          
                                           8. - Modular Terraform design for reusability
                                              - - Separate environments (dev/staging/prod) via tfvars
                                                - - Automated infrastructure provisioning and application deployment
                                                  - - Kubernetes manifests for scalable container orchestration
                                                    - - Security best practices with NSG rules and RBAC
                                                     
                                                      - ## License
                                                     
                                                      - MIT
