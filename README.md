# k8s_site2024
Publish a simple website in a Kubernetes cluster

The file related to website creation are in the **site_main** folder; the webiste is developed using Hugo

The Dockerfile and the docker-compose file are in **docker_site** folder, while the free-available Docker image is stored in DockerHub and you can obtain it using `docker pull gorle19/s314781_site:latest` command

The Kubernetes YAML source files are in **k8s** folder; there are 3 files, one to create the ClusterIP service, one for the pod deployment and one for the ingress creation, in order to expose the webiste on your domain. You can create all these resources using `kubectl apply -f <file_name.yaml>`
