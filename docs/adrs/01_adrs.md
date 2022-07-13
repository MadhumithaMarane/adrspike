# Muziris

## What is  Muziris  ?

***Muziris*** is the M&S Engineering portal for APIs, events  and reusable assets in M&S to enhance developer experience. 

Muziris is powered by *Backstage*, with few enhancements and additional plugins built for M&S. 

[Backstage](https://backstage.io/) is an open platform for building developer portals. Backstage unifies all infrastructure tooling, services, and documentation to create a streamlined development environment from end to end.

## Documentation

Documentation, How-tos and samples for the portal are available [here](https://muziris.azurewebsites.net/catalog/default/component/Muziris/docs). Muziris documention is markdown documentation as code referred to from [the repo](https://github.com/DigitalInnovation/Muziris/docs)

Out of the box, Muziris portal includes:

- [Software Catalogue](https://muziris.azurewebsites.net/catalog/default/component/Muziris/docs/features/software-catalog/) for managing all software (microservices, libraries, data pipelines, websites, infrastrcutre templates etc.)
- [Software Templates](https://muziris.azurewebsites.net/catalog/default/component/Muziris/docs/features/software-templates/) for quickly spinning up new projects and standardizing your tooling with your organization’s best practices
- [TechDocs](https://muziris.azurewebsites.net/catalog/default/component/Muziris/docs/features/techdocs/) for making it easy to create, maintain, find, and use technical documentation, using a "docs like code" approach
- Plus, a growing ecosystem of [open source plugins](https://github.com/backstage/backstage/tree/master/plugins) that further expand customizability and functionality

The detailed upstream documentation is available at [backstage.io/docs](https://backstage.io/docs)

## Project roadmap

A project roadmap, including already delivered milestones, is available [here](https://github.com/DigitalInnovation/Muziris/projects) in Github.

## Discussions

Please join the discussions for Muziris over [here](https://github.com/DigitalInnovation/Muziris/discussions) in Github.


## Running backstage for local development

### Prerequisites

A Backstage App is a monorepo setup with `lerna` that includes everything you
need to run Backstage in your environment.

- [Node.js](https://nodejs.org/en/download/) Active LTS Release installed
  (currently v14)
- [Yarn](https://classic.yarnpkg.com/en/docs/install)
- [Python](https://www.python.org/downloads/) (although you likely have it
  already).
- [Docker](https://docs.docker.com/engine/install/) installed to use some features
  like Software Templates and TechDocs

### Build and Run Muziris in Local

To get up and running with a local app run an initial build.

```bash

# Fetch our dependencies and run an initial build
yarn install
yarn tsc
yarn build

```
Download the pre-populated app-confg.local.yaml using below [this link](https://mnscorp-my.sharepoint.com/personal/sai_gandikota_mnscorp_net/_layouts/15/download.aspx?SourceUrl=%2Fpersonal%2Fsai%5Fgandikota%5Fmnscorp%5Fnet%2FDocuments%2Fapp%2Dconfig%2Elocal%2Eyaml)

Open the downloaded file and fill github PAT token  

Phew! Now you have a local repository that's ready to run.

```bash
yarn dev
```
