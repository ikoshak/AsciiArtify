# Kubernetes and GitOps AsciiArtify project

## Links on tasks

- [PoC](doc/Concept.md): Kubernetes cluster for local developing process
- [ArgoCD-setup](doc/POC.md): AgoCD intructions and deployment demo
- [MVP-demo](doc/MVP.md): MVP application setup demo via ArgoCD

### kubeplugin usage instructions

1. Copy plugin file from repository
   ```bash
   cp kubeplugin /path/to/directory
   ```
2. Set execution mod for plugin file
   ```bash
   chmod +x kubeplugin
   ```
3. Run plugin with needed parameters. In our case parameter is "RESOURCE_TYPE" - node or pod, "NAMESPACE" [Example]
   ```bash
   ./path/to/directory kubeplugin pod kube-system
   ```
   As result you will see next [Example]:
   ```bash
   pod, kube-system, coredns-77ccd57875-jsc7w, 3m, 15Mi
   pod, kube-system, local-path-provisioner-957fdf8bc-tmpc2, 1m, 8Mi
   pod, kube-system, metrics-server-648b5df564-rncn2, 8m, 19Mi
   pod, kube-system, svclb-traefik-826b3689-qr84c, 0m, 0Mi
   pod, kube-system, traefik-64f55bb67d-8mhpk, 1m, 28Mi
   ```
