# Infra Automation Using GCP KCC
#### Product Lead:
##### 1. Aayushi Singh
##### 2. Dikshant Verma
##### 3. Kopal Chakravarthy
#### Contributed By:
##### 1. Ansh Agarwal     2. Sumeet Gairola    3. Annu Kumari     4. Hitesh Kumar    5. Chaithra H R     6. Sonam Dixit

# Config-Connector:
Config-Connector is a software solution that leverages Kubernetes as a platform to apply and reconcile infrastructure defined as code.
In practical terms it means that we can define, GCP infrastructure as yaml files that can be deployed to a KCC enabled Kubernetes cluster. Once deployed the KCC operator will asynchronously create those resources within the GCP project specified. The KCC operator will handle the dependency mapping required to sequence the creation of resources.
With Config Connector we can define and operate with a simple, declarative configuration in Kubernetes style. Config Connector provides additional functionality beyond creating resources. For example, we can manage existing Google Cloud resources, and use Kubernetes Secrets to provide sensitive data, such as passwords, to our resources.

# Introduction to Anthos Configmanagement

![2](https://user-images.githubusercontent.com/111974272/197861779-bbec03b1-40e6-4c2b-a4ef-78fef0478838.png)

In the above figure, we can see how Anthos Config Management works. Anthos Configmanagement automate policy and security at scale for Kubernetes clusters on-premises, on GKE, and on other public clouds.
Anthos Config Managemnt components:-


##### Config Sync
Config Sync continuously reconciles clusters to a central set of configurations that are stored in one or more Git repositories. This GitOps methodology lets you apply configuration consistently across clusters and environments with an auditable, transactional, and version-controlled deployment process.

##### Policy Controller
Policy controller act as a guardrails. It lets us to create custom policies to enforce the security and compliance of our resource configurations. We can use these policies to actively block non-compliant API requests, or simply to audit the configuration of our resources and report violations.

#### Workflow of Config-Connector with GitHub

![3](https://user-images.githubusercontent.com/111974272/197865569-05415b81-5872-4685-9a34-a4e83fc2d1d5.png)
