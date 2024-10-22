# Istioctl

## Installation

```bash
curl -L https://istio.io/downloadIstio | ISTIO_VERSION=1.23.2 TARGET_ARCH=x86_64 sh -
sudo mv istio-1.23.2 /usr/local/share/istio-1.23.2
echo 'export ISTIO_HOME="/usr/local/share/istio-1.23.2"' >> ~/.zshrc
echo 'export PATH="$PATH:$ISTIO_HOME/bin"' >> ~/.zshrc
source ~/.zshrc
```
