# StackOverFlow  Plugin

**Description:** A plugin that provides stack overflow specific functionality that can be used in different ways (e.g. for homepage and search) to compose your Backstage App.


Before we begin, make sure:

You have created your own standalone Backstage app using @backstage/create-app and not using a fork of the backstage repository. If you haven't setup Backstage already, start here.
To use any of the functionality this plugin provides, you need to start by configuring your App with the following 


**Business Value:** The idea for the stackoverflow plugin is to to allow developers to search for questions on stackoverflow.com/questions and index in any Search Engine instance .

## Plugin Deep-Dive

### Developer Docs

Developer Docs are mentioned here: https://github.com/backstage/backstage/tree/master/plugins/stack-overflow


### User Docs

The Plugin Consists of StackOverflow frontend and backend plugins to enable   Stackoveflow 

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

