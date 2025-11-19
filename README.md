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
- [Kubernetes architecture](https://kubernetes.io/docs/concepts/architecture/)
- All docs below from kuberentes.io
  - [Pods](https://kubernetes.io/docs/concepts/workloads/pods/)
  - [Services](https://kubernetes.io/docs/concepts/services-networking/service/)
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
- [eksctl](https://github.com/eksctl-io/eksctl)
- Compute options on EKS
  - [Managed node groups](https://docs.aws.amazon.com/eks/latest/userguide/managed-node-groups.html)
  - [Self managed nodes](https://docs.aws.amazon.com/eks/latest/userguide/worker.html)
  - [Fargate](https://docs.aws.amazon.com/eks/latest/userguide/fargate.html)
  - [Hybrid nodes](https://docs.aws.amazon.com/eks/latest/userguide/hybrid-nodes-overview.html)
  - [Creating your custom image](https://docs.aws.amazon.com/eks/latest/userguide/eks-ami-build-scripts.html)
- [Blog discussing EKS blueprints, focusing on the Terraform ones](https://aws.amazon.com/blogs/containers/bootstrapping-clusters-with-eks-blueprints/)
- [EKS blueprints repo](https://github.com/aws-ia/terraform-aws-eks-blueprints/)
- Upgrading clusters
  - [version skew policy](https://kubernetes.io/releases/version-skew-policy/)
  - [Steps for Upgrading eks clusters](https://docs.aws.amazon.com/eks/latest/userguide/update-cluster.html#update-cluster-summary)
  - [Best practices for EKS upgrade](https://docs.aws.amazon.com/eks/latest/best-practices/cluster-upgrades.html)
  - [Kubernetes currently - Nov, 2025 - supports latest and 2 previous versions](https://kubernetes.io/releases/)
  - [EKS version support](https://docs.aws.amazon.com/eks/latest/userguide/kubernetes-versions.html)
- Using container registries
  - [Using artifactory on EKS](https://aws.amazon.com/blogs/containers/use-private-certificates-to-enable-a-container-repository-in-amazon-eks/)
  - [Logging in to ECR](https://docs.aws.amazon.com/AmazonECR/latest/userguide/registry_auth.html)
  - [Scanning ECR images](https://docs.aws.amazon.com/AmazonECR/latest/userguide/image-scanning-basic.html#clair-deprecation)
- Scaling 
  - [Horizontal pod autoscaler, on kubernetes.io](kubernetes.io/docs/tasks/run-application/horizontal-pod-autoscale/)
  - [Vertical pod autoscaler doc on kubernetes.io](https://kubernetes.io/docs/concepts/workloads/autoscaling/#scaling-workloads-vertically)
  - [Cluster auto scaler](https://docs.aws.amazon.com/eks/latest/best-practices/cas.html)
  - [List of metrics that can be used for scaling](https://kubernetes.io/docs/reference/instrumentation/metrics/)
  - [Keda - Kubernetes event-driven autoscaler](https://keda.sh/docs/2.18/concepts/#keda-architecture)
  - [Scalers, way for keda to connect to event sources](https://keda.sh/docs/2.18/scalers/)
  - [Helm charts available for VPA and Cluster autoscaler](https://github.com/kubernetes/autoscaler/?tab=readme-ov-file)
  - [In-place vertical pod resizing is beta on 1.33](https://kubernetes.io/blog/2025/05/16/kubernetes-v1-33-in-place-pod-resize-beta/)
## Day 2 links
- Karpenter
  - [Best practices, from EKS docs](https://docs.aws.amazon.com/eks/latest/best-practices/karpenter.html)
  - [Allocation strategies for spot instances, Karpenter uses the priceCapacityOptimized](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-fleet-allocation-strategy.html)
  - [Karpenter in use to optimize spot usage](https://aws.amazon.com/blogs/compute/applying-spot-to-spot-consolidation-best-practices-with-karpenter/)
  - [Karpenter node pools, where we define all constraints for nodes](https://karpenter.sh/docs/concepts/nodepools/)
- CDK, use your high level programming language of choice to synthesize your code in CloudFormation templates
  - [CDK hello world](https://docs.aws.amazon.com/cdk/v2/guide/hello-world.html)
  - [Construct hub](https://constructs.dev/search?q=&cdk=aws-cdk&cdkver=2&offset=0&tags=aws-published)
  - [CDK8s, applies the same principles of high-level programming language development from the CDK, but producting kubernetes manifests](https://cdk8s.io/)
- Networking in kubernetes
  - [DNS for pods and services](https://kubernetes.io/docs/concepts/services-networking/dns-pod-service/)
  - [VPC CNI](https://github.com/aws/amazon-vpc-cni-k8s)
  - [CNI - Container network interface](https://github.com/containernetworking/cni?tab=readme-ov-file)
  - [Security groups for pods, SecurityGroupPolicy resource](https://docs.aws.amazon.com/eks/latest/userguide/security-groups-for-pods.html)
  - [LoadBalancer service. It can use ip or instance-level target. Can also be NLB or ALB](https://docs.aws.amazon.com/eks/latest/best-practices/load-balancing.html)
  - [Services in kubernetes.io - ClusterIP, NodePort, LoadBalancer and ExternalName](https://kubernetes.io/docs/concepts/services-networking/service/)
  - [LoadBalancer controller, ingress for AWS](https://kubernetes-sigs.github.io/aws-load-balancer-controller/v2.1/how-it-works/)
  - [Alternate CNI plugins on EKS, popular ones are Cilium and Calico](https://docs.aws.amazon.com/eks/latest/userguide/alternate-cni-plugins.html)
  - [Network policies on kubernetes.io](https://kubernetes.io/docs/concepts/services-networking/network-policies/)
- Observability
  - [Fluentbit outputs](https://docs.fluentbit.io/manual/data-pipeline/outputs)
  - [X-ray replacement with OTel](https://docs.aws.amazon.com/xray/latest/devguide/xray-sdk-migration.html)
  - [Setting up container insights on EKS. Important steps are deploying an observability and a pod identity add-on](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/deploy-container-insights-EKS.html)
  - [Logging on fargate](https://docs.aws.amazon.com/eks/latest/userguide/fargate-logging.html)
- [Pod Identity announcement on EKS](https://aws.amazon.com/blogs/aws/amazon-eks-pod-identity-simplifies-iam-permissions-for-applications-on-amazon-eks-clusters/)
- [Storage classes](https://kubernetes.io/docs/concepts/storage/storage-classes/)
## Day 3 links
- [CSI - the container interface for storage, supporting multiple drivers, among others EBS - announcement](https://kubernetes.io/blog/2019/01/15/container-storage-interface-ga/)
- [EBS CSI](https://github.com/kubernetes-sigs/aws-ebs-csi-driver)
- [EBS multi-attach](https://docs.aws.amazon.com/ebs/latest/userguide/ebs-volumes-multi.html)
- [Rotation lambdas for secrets manager](https://docs.aws.amazon.com/secretsmanager/latest/userguide/reference_available-rotation-templates.html)
- [Secrets provider CSI driver](https://github.com/aws/secrets-store-csi-driver-provider-aws)
