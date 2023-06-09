# ms-homework 2

#### Запуск Ingress через файл манифеста для minikube:
`minikube addons enable ingress`<br/>
`kubectl apply -f nginx-ingress.yaml`
<br/>
<br/>

#### Запуск манифеста - Deployment и Service:
`kubectl apply -f app.yaml`
<br/>
<br/>

#### Запустить Ingress через Helm:
`kubectl create namespace m && helm repo add ingress-nginx https://kubernetes.github.io/ingress-nginx/ && helm repo update && helm install nginx ingress-nginx/ingress-nginx --namespace m -f nginx-ingress.yaml`
<br/>
<br/>

#### Эндпоинты:
http://arch.homework/health <br/>
http://arch.homework/otusapp/aaabbb/ccc
<br/>
<br/>

#### Запуск Postman коллекции:
newman run ms_hw_2.postman