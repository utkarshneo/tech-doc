# Gitlab Plugin

**Description:** The Gitlab plugin provides access to the features of the repository hosted on Gitlab .



- List top 20 builds for a project
- List top 20 Merge Requests for a project
- List top 20 Issues for a project
- View Contributors for a project
- View Languages used for a project
- View Pipeline status for a project
- Works for both project and personal tokens
- Pagination for builds
- Pagination for Merge Requests
- Merge Requests Statistics

**Business Value:** The Business Value that it derives to our Plugins 

## Plugin Deep-Dive

### Developer Docs

Developer Docs are mentioned here: https://github.com/loblaw-sre/backstage-plugin-gitlab

### User Docs

The plugin if integrated requires no special attention from End users to enable it.

The Gitlab Annotation will do the job automatically for catalog entities

```yaml
apiVersion: backstage.io/v1alpha1
kind: Component
metadata:
  # ...
  annotations:
      gitlab.com/project-id: 'project-id' #1234. This must be in quotes and can be found under Settings --> General
      or
      gitlab.com/project-slug: 'project-slug' # group_name/project_name
spec:
  type: service
```

### Owner of the Package

[LobLaw](https://github.com/loblaw-sre/backstage-plugin-gitlab)

## Decision

**The plugin seems useful and will be part of RearPortal out-of-the-box offerings.**

If changes will be required by any of our customer to customize this plugin - we can either:

- Fork the upstream plugin and build on top of it.

- Contribute the changes to the plugin owner.

