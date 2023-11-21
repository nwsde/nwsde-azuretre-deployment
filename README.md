# nwsde-azuretre-deployment repo

> Created from template [`microsoft/AzureTRE-Deployment`](https://www.github.com/microsoft/AzureTRE-Deployment)

This project is intended to assist the deployment of the Azure TRE project in real world environments. This includes deploying using a dev container from your local machine, deploying using GitHub Actions, and publishing custom templates.

See the [Azure TRE documentation](https://microsoft.github.io/AzureTRE/) which includes detailed documentation and best practices to ensure a successful deployment and to assist you with customizing your own templates using this repository.

## Contents

In this project you will find:

- Github Actions implementing AzureTRE automation, including running deployments to Azure
- Configuration specific to deployment
- Workspace template definitions
- User resource template definitions
- Devcontainer setup


### Prerequisites

To work with devcontainers you will need:

- [Visual Studio Code](https://code.visualstudio.com)
- [Remote containers extension for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)


## Current environment pipelines

The following environment pipelines are configured via GitHub Actions & Environment protection rules:


| Branch or tag  | *deploys* Azure TRE | *to* Environment | Env status | TRE name |
|-------------|------------|--|---|---|
| release tag |     | `PROD` |  *(not yet in use)* |
| release tag |  | `STAGE` | *(not yet in use)*
| `main`        | `microsoft/AzureTRE:v0.15.2`  | `TEST` | *(not yet in use)*
| `develop`     | `nwsde/nwsde-azuretre:develop`  | `DEV` | active |`nwsdedev`