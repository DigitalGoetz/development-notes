# Kubectl 

```bash
export KUBECTL=$(curl -L -s https://dl.k8s.io/release/stable.txt)
curl -LO "https://dl.k8s.io/release/$KUBECTL/bin/linux/amd64/kubectl"
sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl
```


## Plugins

### Kubectl Minio Plugin

```bash
curl -L https://github.com/minio/operator/releases/download/v5.0.14/kubectl-minio_5.0.14_linux_amd64 -o kubectl-minio
chmod +x kubectl-minio
sudo mv kubectl-minio /usr/local/bin/
```