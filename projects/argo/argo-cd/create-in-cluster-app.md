
CLI
```
argocd app create --name test \
--repo https://github.com/Ainfosecsss/website.git \
--dest-server https://kubernetes.default.svc \
--dest-namespace andre --path kubernetes
```

YAML

```
apiVersion: argoproj.io/v1alpha1
kind: Application
metadata:
  name: test
  namespace: andre
spec:
  project: default
  source:
    repoURL: https://github.com/Ainfosecsss/website.git 
    targetRevision: HEAD
    path: projecte/argo/example-app
  destination:
    server: https://kubernetes.default.svc
    namespace: andre
```

