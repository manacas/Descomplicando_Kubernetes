# Descomplicando Kubernetes

## Install ``kubectl``

On Linux:

1. Download the latest release with the command:

    ```text
    curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
    ```

2. Install kubectl:

    ```text
    sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl
    ```

3. Test to ensure the version you installed is up-to-date:

    ```text
    kubectl version --client --output=yaml
    ```

## Install ``kind``

On Linux:

```text
curl -Lo ./kind https://kind.sigs.k8s.io/dl/v0.17.0/kind-linux-amd64

chmod +x ./kind

sudo mv ./kind /usr/local/bin/kind
```
