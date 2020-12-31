# deploy-kubernetes
### Atividade do curso KubeDev

> Separe a aplicação em 2 namespaces, um namespace com o banco de dados MongoDB e outro com a API. Lembre-se que a API precisa se comunicar corretamente com o MongoDB.​

- Criação dos namespaces

```console
kubectl create namespace api
```
```console
kubectl create namespace mongo
```

- Execução dos manifestos

```console
kubectl apply -f k8s/mongodb/deployment.yaml -f k8s/mongodb/service.yaml k8s/api/deployment.yaml -f k8s/api/service.yaml
```
