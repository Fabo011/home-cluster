# Home Cluster

## Minikube + Helm Install

#### Mac
```
brew install minikube
brew install helm
```

#### Create helm project
```
helm create <clusterName>
```


#### Use kubectl
```
alias kubectl="minikube kubectl --"
```

---

<br>

#### Start and Stop Minikube
```
minikube start
minikube stop
```

#### Minikube Dashboard
```
minikube dashboard
```

---

<br>

## Helm Commands

#### Before Install
```
helm dependency update
helm dependency build
```
#### Install Commands

```
helm install home-cluster . -f environments/values.yaml
helm install home-cluster . -f environments/values.yaml -n dev
```

#### Uninstall
```
helm uninstall home-cluster
```

#### Get Pods

```
helm get pods
```

---

<br>

## Kuberetes Commands
#### Create New Namespace
```
kubectl create namespace namespace-name
```
