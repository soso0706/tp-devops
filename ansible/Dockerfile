FROM python:3.12-slim

# openssh-client : pour qu'Ansible puisse se connecter à ton serveur
RUN apt-get update \
    && apt-get install -y --no-install-recommends openssh-client \
    && rm -rf /var/lib/apt/lists/*

# Installe Ansible
RUN pip install --no-cache-dir ansible

WORKDIR /ansible