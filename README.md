# EKS-Nov-2025

## Class links
- [Access to labs and course materials](https://us-east-1.student.classrooms.aws.training/class/dy6GmQvvQ8W3xSFSiusjyf): when you open this link, you will be prompted to signin. The preferred way is using "builder id". Problem is this tipically only works with personal emails. If you want to use your corporate account, choose One-time email password (preferred) or SSO. The SSO option eventually prevents us from working properly on the labs. Once registered, you will get an access denied error until I add you to the class. Please send me the email used to register through chat. Below is a screenshot with the options:
<img src="./lab-login.jpg" alt="login options" width="300" height="300"/><br>

## Learning resources
- [Skill builder](https://skillbuilder.aws/)
- [Skill builder subscriptions](https://skillbuilder.aws/subscriptions)

## Recommended pre-req classes
- [Introduction to containers](https://skillbuilder.aws/learn/CUCA1DK47V/introduction-to-containers/XJ58VC1FF5)
- [Amazon EKS primer](https://skillbuilder.aws/learn/Z521GMBP1J/amazon-eks-primer/NGM5AF9K72)
- [AWS Cloud Practitioner Essentials](https://skillbuilder.aws/learn/94T2BEN85A/aws-cloud-practitioner-essentials/8D79F3AVR7)

## Day 1 links
- [12 factor app](https://12factor.net/)
- All docs below from kuberentes.io
  - [Pods](https://kubernetes.io/docs/concepts/workloads/pods/)
  - [Services](https://kubernetes.io/docs/concepts/services-networking/service/)
  - [Kubernetes architecture](https://kubernetes.io/docs/concepts/architecture/)
  - [Taints and tolerations](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/)
  - [Node affinity and anti-affinity](https://kubernetes.io/docs/concepts/scheduling-eviction/assign-pod-node/#node-affinity)
  - [ConfigMap](https://kubernetes.io/docs/concepts/configuration/configmap/)
  - [Secrets](https://kubernetes.io/docs/concepts/configuration/secret/)
  - [Job](https://kubernetes.io/docs/concepts/workloads/controllers/job/)
  - [Cronjob](https://kubernetes.io/docs/concepts/workloads/controllers/cron-jobs/)
  - [Daemonset](https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/)
  - [Replicaset](https://kubernetes.io/docs/concepts/workloads/controllers/replicaset/)
  - [Statefulset](https://kubernetes.io/docs/concepts/workloads/controllers/statefulset/)
  - [Custom resource definitions](https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/)
  - [Operators](https://kubernetes.io/docs/concepts/extend-kubernetes/operator/)
  - [Admission controllers](https://kubernetes.io/docs/reference/access-authn-authz/admission-controllers/)
- Installing a kubernetes cluster
  - [Using Kubeadm to install a cluster](https://kubernetes.io/docs/setup/production-environment/tools/)
  - [Kubernetes the hard way](https://github.com/kelseyhightower/kubernetes-the-hard-way)
  - [EKS auto-mode](https://aws.amazon.com/blogs/aws/streamline-kubernetes-cluster-management-with-new-amazon-eks-auto-mode/?trk=d57158fd-77e3-423f-9e1e-005fd2a64d89&sc_channel=el)

  - [Commands available in the EKS API](https://docs.aws.amazon.com/cli/latest/reference/eks/)
  - Compute options on EKS
    - [Managed node groups](https://docs.aws.amazon.com/eks/latest/userguide/managed-node-groups.html)
    - [Self managed nodes](https://docs.aws.amazon.com/eks/latest/userguide/worker.html)
    - [Fargate](https://docs.aws.amazon.com/eks/latest/userguide/fargate.html)
    - [Hybrid nodes](https://docs.aws.amazon.com/eks/latest/userguide/hybrid-nodes-overview.html)
