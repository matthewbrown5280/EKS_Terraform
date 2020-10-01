# EKS_Terraform (EKS 201)

> EKS + KubeCtl + EKSctl + Helm + Terraform
 
Standard k8s would be containers (in this case Docker) within k8s pods (including the kubelet and kube-proxy services (creating a POD).  Each becomes a worker node.  In typical standard k8s installations there is an additional node (an EC2 for instance) with serves as the Master node (think, jumbox with extra duties).  Notice in the screenshot below there are services including the controls:

- K8s API server (we are the master of masters :-) ) so we master this. KUBECTL is the tool.
- Scheduler
- Controller Manager
- etcD

Using the TF files, I was able to spawn a cluster (the 'Beereum' cluster) for my proposed Beereum Crypto-currency website.

I am currently blocked from getting nodes running and recognized by Kubectl (either a config or kublet service not running) and would need to install prometheus and grafana.
