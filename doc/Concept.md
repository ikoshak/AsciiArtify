#Kubernetes for local developing process

We have the proof of concept task. The dev team needs to choose which one of the Kubernetes instruments should be used. We have three options: minikube, kind, and k3d. So my task is to demonstrate the pros and cons of all options and choose the best for local development.

The following features are important for the development process:
1. Easy to install
2. Easy to use
3. Low resource consumption
4. Automation
5. Add ons

##Minikube
It's a local Kubernetes system that can deploy clusters on one host.  Minikube is easy to use for testing and development on local PCs. However, minikube can run in single-node mode only.

##Kind (Kubernetes IN Docker)
It's a tool that can create Kubernetes clusters in Docker containers. Kind is a good choice for testing needs.

##K3d/K3s
It's a tool that can create Kubernetes clusters in Docker containers like the previous one. However, K3d has a few differences. K3d uses Rancher Kubernetes Engine. 

##Comparison Table

| Feature              | minikube | kind  | k3d          |
|----------------------|----------|-------|--------------|
| Supported Arch.      | AMD64    | AMD64 | AMD64, ARM64 |
| Multiple Nodes       | -        | +     | +            |
| Add ons              | +        | -     | +/-          |
| Automations          | +        | +     | +            |
| Resource consumption | ++       | +     | +++          |
| Documentation        | +        | +     | +            |
| Easy to install      | ++       |       | ++           |
| Easy to use          | +        | +     | +            |


So as you can see k3d has advantages. Kd3 needs to start only 512 MB RAM. However, has fewer add-ons than Minikube. In my opinion, the best solution for the project will be to use K3d.

##Short Demo - deploying container in K3d cluster

![Image](../ikote_demo.gif)
