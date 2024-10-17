
# Kubernetes Deployment with Monitoring on AWS

This repository contains an Ansible playbook for deploying a Kubernetes cluster on AWS with integrated monitoring solutions using Grafana and Splunk. The setup also utilizes Terraform for infrastructure provisioning and Jenkins for CI/CD processes.

## Prerequisites

- Ansible 2.9+
- Jenkins with appropriate plugins installed
- Terraform 0.12+
- AWS CLI configured with administrative access
- Helm 3.x installed on the machine executing the playbook
- Kubernetes CLI (kubectl) configured to interact with your cluster

## Setup

1. **AWS Credentials**: Ensure your AWS credentials are configured by setting the environment variables `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY`.
2. **Terraform Files**: Place your Terraform files in the `terraform` directory. These files should be prepared to set up the AWS infrastructure and the Kubernetes cluster.
3. **Helm Charts**: The playbook uses Helm to deploy Grafana and Splunk; ensure the charts are compatible with your Kubernetes version.

## Running the Playbook

To run the playbook, navigate to the `ansible` directory and execute:

```bash
ansible-playbook deploy_k8s_with_monitoring.yml
```

This will start the process of setting up your infrastructure, deploying the Kubernetes cluster, and configuring the monitoring tools.

## Contributions

Contributions are welcome. Please fork the repository and submit a pull request with your suggested changes.

## License

Specify your license or simply mention that this project is licensed under the MIT License.
