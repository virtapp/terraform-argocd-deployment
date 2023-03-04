![image](https://user-images.githubusercontent.com/23049337/222911432-63630d1e-1ad2-4a9b-9fa2-a0f532fd7f00.png)

 
Kubernetes in Docker with Terraform and ArgoCD



🎯 About

This project is a simple example of how to use Terraform to create a Kubernetes cluster in Docker using Kind


The following tools were used in this project:

    Terraform
    Kind
    Docker
    


Connect to ArgoCD:
    Get ArgoCD admin password

    kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d
    Port forward ArgoCD to http://localhost:8080
    kubectl port-forward -n argocd service/argocd-server --address 0.0.0.0 8080:80


