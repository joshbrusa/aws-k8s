# aws-k8s

## Required

- `eksctl`
- `awscli`
- `kubectl`

## Docs

- [How to Make a Cluster](https://docs.aws.amazon.com/eks/latest/userguide/getting-started-eksctl.html)
- [How to Deploy an App](https://docs.aws.amazon.com/eks/latest/userguide/sample-deployment.html)

## Steps

1. Create a cluster: `eksctl create cluster --name my-cluster --region us-west-1 --fargate`
2. Deploy app: `kubectl apply -f deployment.yml`
3. Apply service: `kubectl apply -f service.yml`
4. List resources: `kubectl get all`
5. Visit the endpoint listed on the service.
6. Delete cluster: `eksctl delete cluster --name my-cluster`
