# Jira Board Plugin

**Description:** The plugin will show jira Tasks and Progress for the same on the JIRA Board and pull the same from altassian accounts

- The ability to plan agile work from project backlog to sprints

- Customizable workflows to fit your frameworks

- Fully customizable Kanban and Scrum boards

- The ability to estimate time for issues as you prioritize your backlog

**Business Value:**  The Business Value of the plugin is it makes it possible to manage JIRA workflows and integrate them into your RearPortal instance

## Plugin Deep-Dive
Plugin Allows to make it manage JIRA workflows and show them in backstage without logging into official jira 
account.
### Developer Docs

Developer Docs are mentioned here: https://github.com/RoadieHQ/roadie-backstage-plugins/tree/main/plugins/frontend/backstage-plugin-github-insights

### User Docs

The plugin if integrated requires no special attention from End users to enable it.

The GitHub Annotation will do the job automatically for catalog entities

```yaml
metadata:
  annotations:
    jira/project-key: <example-jira-project-key>
    jira/component: <example-component> # optional, you might skip this value to fetch data for all components
    jira/token-type: Bearer # optional, used for Activity stream feed. If you are using Basic auth you can skip this.
```

### Owner of the Package

[Roadie](https://roadie.io/backstage/plugins/jira/?utm_source=backstage.io&utm_medium=marketplace&utm_campaign=jira)

## Decision

**The plugin seems useful and will be part of RearPortal out-of-the-box offerings.**


This Plugin is extremely useful to manage JIRA board in  RearPortal instance.

