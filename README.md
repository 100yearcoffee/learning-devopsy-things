learning more devops

when resuming run:
kubectl proxy
minikube tunnel -c
kubectl port-forward service/web-service 8080:80

pods: api(1), crawler(1/3 containers), web(3/1)

## Notes
on omarchy something is funky with minikube internal dns.
Need to run this:
minikube ssh -- "printf 'nameserver 1.1.1.1\nnameserver 8.8.8.8\noptions ndots:0\n' | sudo tee /etc/resolv.conf"

So it uses proper dns instead of other stange DNS that was listed there.
