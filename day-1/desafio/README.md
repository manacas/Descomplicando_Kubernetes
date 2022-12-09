# Descomplicando o Kubernetes | Day-1 | Desafio-1

Chegou a hora de criar o nosso primeiro cluster Kubernetes !

## Instalando o kind e criando o cluster Kubernetes

1. Instalar o kind e criar o nosso primeiro cluster kubernetes:

    Agora é a hora de instalar o sensacional Kind, para que possamos ter o nosso primeiro cluster Kubernetes criado com sucesso!

    Para a criação do seu cluster Kubernetes, nós vamos utilizar o Kind! O nosso cluster será composto de um node Control-Plane e 3 nodes Workers.

    Você deve criar um arquivo chamado meu-primeiro-cluster.yaml no diretório /root com todas as definições necessárias para o Kind criar o seu cluster.

    - Instalar ``kubectl``

    - Instalar ``kind``

    - Criar arquivo meu-primeiro-cluster.yaml

        ```text
        kind create cluster --name kind-multinodes --config meu-primeiro-cluster.yaml
        ```

2. Deploy do nosso primeiro Pod

    Temos um arquivo já criado esperando somente você realizar o deploy desse nosso primeiro pod!

    O manifesto com todas as definições para a criação desse pod está em /root/meu-primeiro-pod.yaml.

    Lembre-se, se tiver algum erro no momento do deploy, você precisa ajustar o que estiver errado e tentar novamente!

    Precisamos ter esse pod em execução!

    ```text
    kubectl apply -f meu-primeiro-pod.yaml
    ```
