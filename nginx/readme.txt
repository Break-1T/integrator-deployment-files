kubectl create namespace ingress-nginx
kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/main/deploy/static/provider/cloud/deploy.yaml

get external ip via: kubectl get svc -n ingress-nginx

update hosts in C:\Windows\System32\drivers\etc with <external-ip> myapp.local