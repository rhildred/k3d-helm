FROM mcr.microsoft.com/vscode/devcontainers/python

RUN apt update 

RUN apt install -y ansible

COPY hosts /etc/ansible/hosts

RUN curl -s https://raw.githubusercontent.com/k3d-io/k3d/main/install.sh | bash

RUN curl https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3 | bash

RUN curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"

RUN install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl