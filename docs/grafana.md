# Grafana Plugin

**Description:** The plugin will show the details of the Grafana project and Dashboard on Rearportal for Managing the Infrastructure for Grafana. **

- Dashboard templating This is one Grafana feature that’s really useful. 

- Provisioning

- Annotation

- Kiosk mode and playlists

**Business Value:** The notion of surfacing relevant metadata in the single pane of glass is exemplied here.

We can see some useful insights without searching for the repository in GitHub.

## Plugin Deep-Dive

### Developer Docs

Developer Docs are mentioned here: (https://github.com/K-Phoen/backstage-plugin-grafana)

### User Docs

The plugin if integrated requires no special attention from End users to enable it.

The GitHub Annotation will do the job automatically for catalog entities

```yaml
annotations:
  grafana/tag-selector: "my-grafana-tag"
  
```

### Owner of the Package

[Roadie](https://github.com/K-Phoen/backstage-plugin-grafana)

## Decision

**The plugin seems useful and will be part of RearPortal out-of-the-box offerings.**

If changes will be required by any of our customer to customize this plugin - we can either:

- Fork the upstream plugin and build on top of it.

- Contribute the changes to the plugin owner.

