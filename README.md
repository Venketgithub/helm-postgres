To install using helm:
helm install helm-postgres helm-postgres/ --namespace team1-tenant1

To package:
helm package helm-postgres


To create helm chart:
To convert your Kubernetes manifests into a Helm chart, you'll create a directory structure for the Helm chart and use templating for dynamic values in the Kubernetes resources. Below, I’ll guide you through creating the necessary files for the Helm chart, including the values.yaml file.

Directory Structure
plaintext
Copy code
my-postgres-chart/
├── Chart.yaml
├── templates/
│   ├── deployment.yaml
│   ├── pvc.yaml
│   ├── secret.yaml
│   ├── service.yaml
│   └── route.yaml
└── values.yaml