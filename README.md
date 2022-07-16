# CD-CD-argoCD-sample-app
This is a repository that hosts the Dockerfile that has to be pushed to a Docker Registry implementing a CI Pipeline and then argoCD will automatically deploy it into a kubernetes cluster. Instead of deploying it to AWS EKS we will suppose that ArgoCD server and AWS EKS cluster are in the same machine. 

We push our docker images to the public repository antoniobriperez/flask_docker in Docker Hub. We authenticate thanks to GitHub Secrets and this CI flow gets enabled each time we push over master. 

To know about CD part check https://github.com/AntonioBriPerez/argocd-manifests
