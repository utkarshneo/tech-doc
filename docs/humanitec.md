# Humanitec Plugin

**Description:** 
Show workloads, environments and resources deployed by Humanitec Platform Orchestrator. Plugin includes an Entity ComponentCard, Backend API route and scaffolder actions

The Plugin has following features:

- Definition of baseline configurations

- Role Based Access Control 

- Infrastructure orchestration

- Definition of resource dependencies (e.g., which kind of environments should be equipped with which kind of infrastructure)

**Business Value:** The notion of surfacing relevant metadata in the single pane of glass is exemplied here.

We can see some useful insights without searching for the repository in Humanitec

## Plugin Deep-Dive

### Developer Docs

Developer Docs are mentioned here: (https://github.com/thefrontside/backstage/tree/main/plugins/humanitec)

### User Docs

The plugin if integrated requires no special attention from End users to enable it.

The GitHub Annotation will do the job automatically for catalog entities

```yaml
humanitec:
  orgId: my-humanitec-organization
  token: ${HUMANITEC_TOKEN} # without Bearer
```

```yaml
# ./catalog-humanitec-workloads.yaml
apiVersion: backstage.io/v1alpha1
kind: Component
metadata:
  name: name-of-application-workload # 🚨 CHANGE
  description: Humanitec Workload Environments
  annotations:
    "humanitec.com/orgId": "my-humanitec-organization" # 🚨 CHANGE
    "humanitec.com/appId": "my-humanitec-application" # 🚨 CHANGE
spec:
  type: service
  owner: john@example.com
  lifecycle: experimental

```



### Owner of the Package

[FrontSide]https://frontside.com)

## Decision

**The plugin seems useful and will be part of RearPortal out-of-the-box offerings.**

If changes will be required by any of our customer to customize this plugin - we can either:

- Fork the upstream plugin and build on top of it.

- Contribute the changes to the plugin owner.

