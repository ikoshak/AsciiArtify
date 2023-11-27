# Minimum Viable Product (MVP)

1. Deploy argocd to k3d cluster 

- [ArgoCD-setup](doc/POC.md)

2. Fork repository with go-app-demo

3. Login in ArgoCD and create new deployment and run sychronization with git repository

4. Fix type of service in helm chart - values.yaml file - frome "LoadBalancer" to "NodePort"

5. Run "Refresh" and "Sync" in ArgoCD UI

6. Create port forward for deployed appllication "Ambassador"

7. Run curl to check application

8. Appload image for demo repsponce


## ArgoCD, Demo of deploying application


![Image](../.data/ikote_mvp_demo.gif)
