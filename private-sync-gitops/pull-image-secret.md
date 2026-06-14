kubectl create secret docker-registry dockerhub-secret \
    --docker-server=https://index.docker.io/v1/ \
    --docker-username= \
    --docker-password= \ 
    --docker-email= \
    --namespace=app1-ns

Here we have created the above secret imperatively

#### 
- Here Docker-registry is not registry restricted
- It is registry agnostic
- We can also create secret for AWS ECR, Github Container Registory


If we hit, kubectl create secret -h
It will display 3 options as: docker-registry, generic & tls
1. Docker-registry: Create a secret for use with Docker registry
2. Generic: Creata a secret from a localfile, directory or literal value
3. tls: Create a TLS Secret.

-----------------------------------------------------------------------------------


argocd repo add https://github.com/ayanchasrinivas/srinivas-app1-agrocd.git \
    --name app1-config-app \
    --username psychovivek \




git remote set-url origin https://ayanchasrinivas:@github.com/ayanchasrinivas/srinivas-app1-agrocd.git
