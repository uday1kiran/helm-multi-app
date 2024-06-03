my-chart/
├── Chart.yaml
├── values.yaml
├── templates
│   ├── deployment.yaml
│ 
└── charts
    ├── app1
    │   ├── Chart.yaml
    │   │   values.yaml
    │   └── templates
    │       ├── deployment.yaml
    │       └── service.yaml
    └── app2
        ├── Chart.yaml
        │   values.yaml
        └── templates
            ├── deployment.yaml
            └── service.yaml

$ helm package my-chart
$ helm install my-chart my-chart-1.0.0.tgz


kubectl get nodes
kubectl label nodes <node-name> frontend=true
kubectl label nodes <node-name> backend=true






--------------
New-Item -Path 'c:\' -Name 'minikube' -ItemType Directory -Force
Invoke-WebRequest -OutFile 'c:\minikube\minikube.exe' -Uri 'https://github.com/kubernetes/minikube/releases/latest/download/minikube-windows-amd64.exe' -UseBasicParsing

curl.exe -LO "https://dl.k8s.io/release/v1.30.0/bin/windows/amd64/kubectl.exe"

minikube start --nodes=3 --driver=docker

kubectl cluster-info




Ref:
https://kubernetes.io/docs/tasks/tools/install-kubectl-windows/
https://minikube.sigs.k8s.io/docs/start/?arch=%2Fwindows%2Fx86-64%2Fstable%2F.exe+download
https://github.com/helm/helm/releases
https://www.youtube.com/watch?v=4BNDEnwmEYM