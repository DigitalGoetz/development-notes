# Kubernetes in Docker (KIND)

## Installing KinD

```bash
VERSION=v0.24.0

[$(uname -m) = x86_64 ] && \
curl -Lo ./kind "https://kind.sigs.k8s.io/dl/${VERSION}/kind-linux-amd64"
chmod +x ./kind
sudo mv ./kind /usr/local/bin/kind
```