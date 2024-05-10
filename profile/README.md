# CodrJS

Codr is an open-sourced customizable annotation tool for researchers and industry being developed by the [PERC_Lab](https://github.com/PERC-Lab).

This is the start to a improved version of Codr which can be found on [Github](https://github.com/PERC-Lab/Codr) and hosted at https://codr.dylanbulmer.com.

## Repositories

- **CodrJS/API** • [[repo](https://github.com/CodrJS/API)] • _This contains the code for our RESTful API built on the @CodrJS/Core module_
- **CodrJS/setup** • [[repo](https://github.com/CodrJS/setup)] • k8s and service configuration documentation
- **CodrJS/docs** • [[repo](https://github.com/CodrJS/docs)] (**private repo**) • _End user documentation for Codr_
- **CodrJS/WebUI** • [[repo](https://github.com/CodrJS/WebUI)] • _This is the fround-end web client that interacts with the RESTful API_

## NPM modules
View all packages on [npmjs.org](https://www.npmjs.com/org/codrjs)!

| Version | Name | Repo | Image | Purpose | Notes |
| ------- | ---- | ---- | ----- | ------- | ----- |
| ![npm version](https://img.shields.io/npm/v/@codrjs/config) | `@codrjs/config` | [Link](https://github.com/CodrJS/config) | [Link](https://www.npmjs.com/package/@codrjs/config) | Pulls environment variables into a unified JSON object. | |
| ![npm version](https://img.shields.io/npm/v/@codrjs/core) | `@codrjs/core` | [repo](https://github.com/CodrJS/core) | [npmjs.org](https://www.npmjs.com/package/@codrjs/core) |  | *being deprecated* |
| ![npm version](https://img.shields.io/npm/v/@codrjs/design-library) | `@codrjs/design-library` | [repo](https://github.com/CodrJS/design-library) | [npmjs.org](https://www.npmjs.com/package/@codrjs/design-library) | Storybook UI/UX library | [docker image](https://github.com/CodrJS/design-library/pkgs/container/design-library)
| ![npm version](https://img.shields.io/npm/v/@codrjs/health) | `@codrjs/health` | [repo](https://github.com/CodrJS/health) | [npmjs.org](https://www.npmjs.com/package/@codrjs/health) | Monitors health data of the service. | |
| ![npm version](https://img.shields.io/npm/v/@codrjs/kafka) | `@codrjs/kafka` | [repo](https://github.com/CodrJS/kafka) | [npmjs.org](https://www.npmjs.com/package/@codrjs/kafka) | Customized kafka classes for easier integration. |
| ![npm version](https://img.shields.io/npm/v/@codrjs/logger) | `@codrjs/logger` | [repo](https://github.com/CodrJS/logger) | [npmjs.org](https://www.npmjs.com/package/@codrjs/logger) | Unifies logging output for observability | 
| ![npm version](https://img.shields.io/npm/v/@codrjs/models) | `@codrjs/models` | [repo](https://github.com/CodrJS/models) | [npmjs.org](https://www.npmjs.com/package/@codrjs/models) | Contains all data models for Codr |

## Templates

- `ts-npm-template` • [[repo](https://github.com/CodrJS/ts-npm-template)]
- `ts-microservice-template` • [[repo](https://github.com/CodrJS/ts-microservice-template)]
[[docker image](https://github.com/CodrJS/ts-microservice-template/pkgs/container/ts-microservice-template)]

## Microservices

All microservices are hidden within an internal kubernetes network. In the future, a Nginx server will be deployed on top of these services and expose the endpoints by proxying the routes to the correct location.

| Type | Name | Repo | Image | Purpose | Notes |
| ---- | ---- | ---- | ----- | ------- | ----- |
| Entity | `codr-config` | [Link](https://github.com/CodrJS/codr-core-config) | [Link](https://github.com/CodrJS/codr-core-config/pkgs/container/codr-core-config) | Config domain entity manager. | Dataset and other configs? |
| Entity | `codr-preference` | [Link](https://github.com/CodrJS/codr-preference) | | Preference domain entity manager. | User preferences for privacy, notification, etc. |
| Entity | `codr-template` | [Link](https://github.com/CodrJS/codr-template) | | Template domain entity manager. | Email, SMS, and push notification templates. |
| Entity | `codr-user` | [Link](https://github.com/CodrJS/codr-user-user) | [Link](https://github.com/CodrJS/codr-user-user/pkgs/container/codr-user-user) | User domain entity manager. | User identification, used heavily in authentication. |
| Entity | `codr-profile` | [Link](https://github.com/CodrJS/codr-user-profile) | [Link](https://github.com/CodrJS/codr-user-profile/pkgs/container/codr-user-profile) | Profile domain entity manager. | Profile information for non-anonymous users. |
| Entity | `codr-usergroup` | [Link](https://github.com/CodrJS/codr-user-group) | [Link](https://github.com/CodrJS/codr-user-group/pkgs/container/codr-user-group) | User Group domain entity manager. | Grouping users together for project collaboration. |
| Entity | `codr-project` | [Link](https://github.com/CodrJS/codr-project-project) | [Link](https://github.com/CodrJS/codr-project-project/pkgs/container/codr-project-project) | Project domain entity manager. | Project configuration, e.g. display customization. |
| Entity | `codr-dataset` | [Link](https://github.com/CodrJS/codr-project-dataset) | [Link](https://github.com/CodrJS/codr-project-dataset/pkgs/container/codr-project-dataset) | Dataset domain entity manager. | Links samples together and links to a project |
| Entity | `codr-sample` | [Link](https://github.com/CodrJS/codr-project-sample) | [Link](https://github.com/CodrJS/codr-project-sample/pkgs/container/codr-project-sample) | Sample domain entity manager. | Uploaded sample for dataset |
| Entity | `codr-annotation` | [Link](https://github.com/CodrJS/codr-project-annotation) | [Link](https://github.com/CodrJS/codr-project-annotation/pkgs/container/codr-project-annotation) | Annotation domain entity manager. | Annotation provided by user for sample. |
| Service | `codr-audit-svc` | [Link](https://github.com/CodrJS/codr-audit) | | Audit domain processing service. | Consumes event streams to log actions |
| Service | `codr-notification-svc` | [Link](https://github.com/CodrJS/codr-notification-message) | [Link](https://github.com/CodrJS/codr-notification-message/pkgs/container/codr-notification-message) | Notification domain processing service. | Consumes event streams to automate notifications |
| Serivce | `codr-bff` | | | Backend-for-frontend | Intermediary between the browser and API layers for security. |

