**Learning** about fundamentals of using *Kubernetes*

# Guia de Configuração do Kubernetes com kubectl e kind

Este guia fornece instruções passo a passo para configurar o Kubernetes usando as ferramentas `kubectl` e `kind`.

## Instalação do kubectl

Para instalar o `kubectl`, execute os seguintes comandos:

```shell
curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl
```

## Instalação do kind

Para instalar o `kind`, execute os seguintes comandos:

```shell
[ $(uname -m) = x86_64 ] && curl -Lo ./kind https://kind.sigs.k8s.io/dl/v0.20.0/kind-linux-amd64
chmod +x ./kind
sudo mv ./kind /usr/local/bin/kind 
```

<input type="checkbox"> kind create cluster
```shell
kind create cluster --config Meu-primeiro-cluester.yaml --name my-cluster
```

<input type="checkbox"> kubectl apply -f your-pod.yaml
```shell
kubectl apply -f your-pod.yaml
```

##
<span style="color:lightcoral">
Certifique-se de substituir `Meu-primeiro-cluester.yaml` e `your-pod.yaml` pelos nomes reais dos seus arquivos de configuração. Este texto Markdown contém as etapas para instalar o `kubectl`, o `kind`, criar um cluster e criar um pod usando o Kubernetes.</span>

##

- day 1-  created podes.yaml files, and the use of basic commands, installation of kind

