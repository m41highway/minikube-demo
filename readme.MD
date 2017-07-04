Install Minikube on OSX

```
curl -Lo minikube https://storage.googleapis.com/minikube/releases/v0.20.0/minikube-darwin-amd64 && chmod +x minikube && sudo mv minikube /usr/local/bin/
```

The conifg is found in ~/.kube/config


To install the kubectl
```
curl -LO https://storage.googleapis.com/kubernetes-release/release/v1.7.0/bin/darwin/amd64/kubectl
```

Remark: verson below 1.5 may crash if you have old version installed.


To grant access
```
chmod +x kubectl && sudo mv kubectl /usr/local/bin/
```


To get the url to access the cluster
```
minikube service hello-minikube --url
```

To access with browser http://192.168.99.100:30443