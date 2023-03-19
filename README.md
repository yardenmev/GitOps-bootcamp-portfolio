# GitOps Bootcamp Portfolio

This repository contains a collection of Kubernetes applications and infrastructure that were created as part of the GitOps Bootcamp training program. The applications are deployed using ArgoCD, and the infrastructure is managed by Terraform.

## Applications

The following applications are included in this repository:

### Todo App

This is a simple "todo" web application that is packaged as a Helm chart. The chart is automatically built and pushed to ECR by a Jenkins CI pipeline whenever changes are made to the application code. ArgoCD then deploys the chart to the EKS cluster.

### EFK Stack

The EFK (Elasticsearch, Fluentd, Kibana) stack is a popular logging solution for Kubernetes. This Helm chart installs all three components and configures them to work together. The Kibana GUI is accessible via the `yarden-kibana.duckdns.org` domain name.

### Prometheus Stack

The Prometheus stack is a popular monitoring solution for Kubernetes. This Helm chart installs Prometheus, Grafana, and kube-state-metrics, and configures them to work together. The Grafana GUI is accessible via the `yarden-grafana.duckdns.org` domain name.

## Infrastructure

The Terraform code for the EKS cluster and related resources is located in the [infrastructure-bootcamp-portfolio](https://github.com/yardenmev/infrastructure-bootcamp-portfolio) repository. Please refer to that repository's README for more information.

## Contributing

If you would like to contribute to this repository, please fork the repository and submit a pull request with your changes. Please ensure that all changes are tested and do not introduce any new errors or issues.

