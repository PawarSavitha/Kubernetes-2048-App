# 2048 App

## Create Fargate profile

```
eksctl create fargateprofile \
    --cluster demo-cluster \
    --region us-east-1 \
    --name alb-sample-app \
    --namespace game-2048
```

## Deploy the deployment, service and Ingress

```
kubectl apply -f https://raw.githubusercontent.com/kubernetes-sigs/aws-load-balancer-controller/v2.5.4/docs/examples/2048/2048_full.yaml
```



![game-20481](https://github.com/PawarSavitha/Kubernetes-2048-App/assets/114134446/c342e8ac-ea40-410d-8691-a9a5f6556474)


