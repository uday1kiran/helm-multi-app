my-chart/
├── Chart.yaml
├── values.yaml
├── templates
│   ├── deployment.yaml
│   ├── service.yaml
└── charts
    ├── app1
    │   ├── Chart.yaml
    │   │   └── values.yaml
    │   └── templates
    │       ├── app1-deployment.yaml
    │       └── app1-service.yaml
    └── app2
        ├── Chart.yaml
        │   └── values.yaml
        └── templates
            ├── app2-deployment.yaml
            └── app2-service.yaml

$ helm package my-chart
$ helm install my-chart my-chart-1.0.0.tgz


kubectl get nodes
kubectl label nodes <node-name> frontend=true
kubectl label nodes <node-name> backend=true