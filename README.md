helm dependency update
helm dependency build

helm install home-cluster . -f environments/values.yaml

helm get pods