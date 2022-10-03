# Security Insights Plugin

**Description:** The plugin will showcase a new tab with the following insights about the GitHub repository catalog in RearPortal:

- Contributor List

- Code Language Distribution

- The root Readme

- Release List (optional)

**Business Value:** The notion of surfacing relevant metadata in the single pane of glass is exemplied here.

We can see some useful insights without searching for the repository in GitHub.

## Plugin Deep-Dive

### Developer Docs

Developer Docs are mentioned here: https://github.com/RoadieHQ/roadie-backstage-plugins/tree/main/plugins/frontend/backstage-plugin-github-insights

### User Docs

The plugin if integrated requires no special attention from End users to enable it.

The GitHub Annotation will do the job automatically for catalog entities

```yaml
metadata:
  annotations:
    github.com/project-slug: [organization name]/[repository name]
```

### Owner of the Package

[Roadie](https://github.com/RoadieHQ/roadie-backstage-plugins/tree/main/plugins/frontend/backstage-plugin-github-insights)

## Decision

**The plugin seems useful and will be part of RearPortal out-of-the-box offerings.**

If changes will be required by any of our customer to customize this plugin - we can either:

- Fork the upstream plugin and build on top of it.

- Contribute the changes to the plugin owner.

