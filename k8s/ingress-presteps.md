# Run this to setup the Ingress Controller in AKS instance

helm upgrade --install ingress-nginx ingress-nginx \
  --repo https://kubernetes.github.io/ingress-nginx \
  --namespace ingress-nginx --create-namespace

# Once this is complete, continue with deploying the AKS Resources along with the Ingress Resource using the deployment-with-ingress.yaml