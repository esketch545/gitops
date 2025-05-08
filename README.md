# gitops

gitops/
├── root/
│   └── app-of-apps.yaml         # Top-level ArgoCD app
├── apps/
│   ├── my-app/
│   │   ├── kustomization.yaml   # Kustomize file (or Helm chart)
│   │   └── deployment.yaml      # Optional static manifest or Helm values
│   └── other-app/
│       └── ...
└── projects/
    └── default-project.yaml     # Optional Argo CD project config