# Create Build Integrations

### Using \`kli\`

Install kli tool to access your clusters

```
# Install kli
curl https://kli.devc.kloudlite.io/v1.0.5-nightly! | bash

# Login
kli auth login

# Access Cluster
kli --cluster-name=<cluster-name> -- kubectl get nodes
```

### Using kubeconfig file

Download your kubeconfig file provided in the dashboard and start accessing your cluster

```bash
export KUBECONFIG=/path/to/config 
kubectl get nodes
```

