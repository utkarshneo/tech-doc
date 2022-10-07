# Argo CD Plugin

**Description:** View Argo CD status for your projects in Backstage.

- Build Pipeline

- Automated deployment of applications to specified target environments

- Continuous monitoring of deployed applications


- Rollbacks should be as simple as deploying a different configuration.

- Application deployments should be fast, reliable, and idempotent.

**Business Value:**  Argo CD empowers organizations to declaratively build and run cloud native applications and workflows on Kubernetes using GitOps. It is a pull-based, declarative, GitOps continuous delivery tool for Kubernetes with a fully loaded UI.

.

## Plugin Deep-Dive

### Developer Docs

Developer Docs are mentioned here: (https://roadie.io/backstage/plugins/argo-cd/?utm_source=backstage.io&utm_medium=marketplace&utm_campaign=argo-cd)

### User Docs

The plugin is already added to the RearPortal instance and 

The plugin if integrated requires no special attention from End users to enable it.

The ArgoCD Annotation will do the job automatically for catalog entities

```yaml
# app-config.yaml

proxy:
  'metadata:
  annotations:
    argocd/app-name: <your-app-name>
```

### Owner of the Package

[Roadie](https://roadie.io/backstage/plugins/argo-cd/?utm_source=backstage.io&utm_medium=marketplace&utm_campaign=argo-cd)

## Decision

**The plugin seems useful and will be part of RearPortal out-of-the-box offerings.**

The plugins are useful for clients who want to see  ArgoCd Pipline in their developer Portal.
Allows the developer to look for the ArgoCd Pipline Data in their rearPortal instance and work with it accordingly  without having to worry about logging into ArgoCd.

