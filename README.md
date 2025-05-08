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



Purpose
- Setup argocd
- Break-out k8s manifests from app code
- Separate resonsibility
    - gitops = platform engineers
    - app code = developers
- Single place of management for platform engineers
- Argocd will auto-sync the new version of app code