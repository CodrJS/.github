# CodrJS

Codr is an open-sourced customizable annotation tool for researchers and industry being developed by the [PERC_Lab](https://github.com/PERC-Lab).

This is the start to a improved version of Codr which can be found on [Github](https://github.com/PERC-Lab/Codr) and hosted at https://codr.dylanbulmer.com.

## Repositories

- **CodrJS/API** • [[repo](https://github.com/CodrJS/API)] • _This contains the code for our RESTful API built on the @CodrJS/Core module_
- **CodrJS/config** • [[repo](https://github.com/CodrJS/config)] (**to be changed**) • _Current state: k8s and service configuration documentation_
- **CodrJS/docs** • [[repo](https://github.com/CodrJS/docs)] (**private repo**) • _End user documentation for Codr_
- **CodrJS/WebUI** • [[repo](https://github.com/CodrJS/WebUI)] • _This is the fround-end web client that interacts with the RESTful API_

## NPM modules
View all packages on [npmjs.org](https://www.npmjs.com/org/codrjs)!

- ![npm version](https://img.shields.io/npm/v/@codrjs/core) `@codrjs/core` • [[repo](https://github.com/CodrJS/core)] [[npmjs.org](https://www.npmjs.com/package/@codrjs/core)] -- *being deprecated*
- ![npm version](https://img.shields.io/npm/v/@codrjs/design-library) `@codrjs/design-library` • [[repo](https://github.com/CodrJS/design-library)] [[npmjs.org](https://www.npmjs.com/package/@codrjs/design-library)]
- ![npm version](https://img.shields.io/npm/v/@codrjs/health) `@codrjs/health` • [[repo](https://github.com/CodrJS/health)] [[npmjs.org](https://www.npmjs.com/package/@codrjs/health)]
- ![npm version](https://img.shields.io/npm/v/@codrjs/kafka) `@codrjs/kafka` • [[repo](https://github.com/CodrJS/kafka)] [[npmjs.org](https://www.npmjs.com/package/@codrjs/kafka)]
- ![npm version](https://img.shields.io/npm/v/@codrjs/logger) `@codrjs/logger` • [[repo](https://github.com/CodrJS/logger)] [[npmjs.org](https://www.npmjs.com/package/@codrjs/logger)]
- ![npm version](https://img.shields.io/npm/v/@codrjs/models) `@codrjs/models` • [[repo](https://github.com/CodrJS/models)] [[npmjs.org](https://www.npmjs.com/package/@codrjs/models)] -- *in progress*

## Templates

- `ts-npm-template` • [[repo](https://github.com/CodrJS/ts-npm-template)]
- `ts-microservice-template` • [[repo](https://github.com/CodrJS/ts-microservice-template)]

## Microservices

**Core Domain**
- `codr-core-controller` • [[repo](https://github.com/CodrJS/codr-core-controller)] • Core domain, traffic proxy
- `codr-core-config` • [[repo](https://github.com/CodrJS/codr-core-config)] • Core domain, configuration manager for all microservices
- `codr-core-audit` • [[repo](https://github.com/CodrJS/codr-core-audit)] • To be built
- `codr-core-email` • [[repo](https://github.com/CodrJS/codr-core-email)] • To be built
- `codr-core-email-template` • [[repo](https://github.com/CodrJS/codr-core-email)] • To be built

**User Domain**
- `codr-user-controller` • [[repo](https://github.com/CodrJS/codr-user-controller)] • To be built
- `codr-user-user` • [[repo](https://github.com/CodrJS/codr-user-config)] • To be built
- `codr-user-profile` • [[repo](https://github.com/CodrJS/codr-user-profile)] • To be built
- `codr-user-session` • [[repo](https://github.com/CodrJS/codr-user-session)] • To be built

**Project Domain**
- `codr-project-controller` • [[repo](https://github.com/CodrJS/codr-project-controller)] • To be built
- `codr-project-project` • [[repo](https://github.com/CodrJS/codr-project-project)] • To be built
- `codr-project-dataset` • [[repo](https://github.com/CodrJS/codr-project-dataset)] • To be built
- `codr-project-sample` • [[repo](https://github.com/CodrJS/codr-project-sample)] • To be built
- `codr-project-annotation` • [[repo](https://github.com/CodrJS/codr-project-annotation)] • To be built
