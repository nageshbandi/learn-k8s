# learn-k8s
learn k8s 

# port forword
kubectl -n ingress-nginx --address 0.0.0.0 port-forward svc/my-nginx-svc 80

#kind --version 
# create k8s cluster 
kind create cluster --image kindest/node:v1.23.5

kubectl get nodes

kubectl create namespace cms

kubectl apply -f https://raw.githubusercontent.com/kubernetes/website/master/content/en/examples/application/nginx-app.yaml

kubectl get svc

kubectl edit svc my-nginx-svc

kubectl get svc

# Install Ingress controller 
kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.1.3/deploy/static/provider/cloud/deploy.yaml

kubectl -n ingress-nginx get pods

#kubectl -n ingress-nginx --address 0.0.0.0 port-forward svc/ingress-nginx-controller 80

kubectl get svc

kubectl get svc -A

kubectl -n ingress-nginx --address 0.0.0.0 port-forward svc/my-nginx-svc 80

kubectl --address 0.0.0.0 port-forward svc/my-nginx-svc 80
apk add helm
helm --version 
helm version
helm repo add kubernetes-dashboard https://kubernetes.github.io/dashboard/
helm upgrade --install kubernetes-dashboard kubernetes-dashboard/kubernetes-dashboard --create-namespace --namespace kubernetes-dashboard
kubectl -n kubernetes-dashboard get svc
kubectl -n kubernetes-dashboard --address 0.0.0.0 port-forward svc/kubernetes-dashboard-kong-proxy 8443
kubectl -n kubernetes-dashboard --address 0.0.0.0 port-forward svc/kubernetes-dashboard-kong-proxy 443

#kubectl -n NAMESPACE create token SERVICE_ACCOUNT
 kubectl get ns

#kubectl -n kubernetes-dashboard create token SERVICE_ACCOUNT
kubectl -n kubernetes-dashboard create token SERVICE_ACCOUNT
kubectl get service-acount
kubectl get sv
kubectl get sa
kubectl -n kubernetes-dashboard create token bandi
  41 kubectl -n kubernetes-dashboard create token default
