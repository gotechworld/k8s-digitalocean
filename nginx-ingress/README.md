https://github.com/digitalocean/Kubernetes-Starter-Kit-Developers/blob/main/03-setup-ingress-controller/nginx.md


```
helm install ingress-nginx ingress-nginx/ingress-nginx \
    --namespace ingress-nginx \
    --create-namespace \
    -f nginx-ingress/nginx-values.yaml
```

```
doctl compute load-balancer list --format IP,ID,Name,Status
```
&nbsp;

Follow Step2 - Configuring DNS Records for NGINX Ingress Controller