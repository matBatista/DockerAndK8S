# Docker with K8S
 
comandos para K8S
 

pod.yaml

criar container
kind create cluster --name=nomeaplicacao

set container
kubectl cluster-info --context kind-nomeaplicacao

apos criar pod.yaml para a aplicação
e aplicar alteracoes usando 
kubectl apply -f pod.yaml

kubectl port-forward pod/nginx 8080:80   

assim dando acesso pelo web


replicaset
é para criar um pod se o seu pod atual foi deletado;

kubectl get pods 
kubectl get rs conforme seu yamls