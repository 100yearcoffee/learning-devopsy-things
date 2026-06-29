learning more devops

when resuming run:
kubectl proxy
minikube tunnel -c
kubectl port-forward service/web-service 8080:80

pods: api(1), crawler(1/3 containers), web(3/1)
