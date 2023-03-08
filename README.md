# Nestjs Tutorial

<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

<p align="center"><i>A progressive <a href="http://nodejs.org">Node.js</a> framework for building efficient, reliable and scalable server-side applications.</i></p>

## Introduction

Nest (NestJS) is a framework for building efficient, scalable [**Node.js**](https://nodejs.org) server-side applications. It uses progressive JavaScript, is built with and fully supports [**TypeScript**](http://www.typescriptlang.org) (yet still enables developers to code in pure JavaScript) and combines elements of OOP (Object Oriented Programming), FP (Functional Programming), and FRP (Functional Reactive Programming).

Under the hood, Nest makes use of robust HTTP Server frameworks like [**Express**](https://expressjs.com) (the default) and optionally can be configured to use [**Fastify**](https://github.com/fastify/fastify) as well!

Nest provides a level of abstraction above these common Node.js frameworks (Express/Fastify), but also exposes their APIs directly to the developer. This gives developers the freedom to use the myriad of third-party modules which are available for the underlying platform.

### Installation

To get started, you need to install the [**Nest CLI**](https://docs.nestjs.com/cli/overview) once if your local machine doesn't exist.

```shell
# install Nest CLI as global dependency
$ npm i -g @nestjs/cli
# then create a project using `nest` command
$ nest new project-name
```

> To create a new project with TypeScript's `strict` mode enabled, pass the `--strict` flag to the `nest new` command.

### Alternatives

Alternatively, to install the TypeScript starter project with Git:

```shell
# clone the project
$ git clone https://github.com/nestjs/typescript-starter.git project
# go into project folder
$ cd project
# install dependencies
$ npm install
# run application
$ npm run start
```

> If you'd like to clone the repository without the git history, you can use [**degit**](https://github.com/Rich-Harris/degit).

Open your browser and navigate to `http://localhost:3000/`.

To install the JavaScript flavor of the starter project, use `javascript-starter.git` in the command sequence above.

You can also manually create a new project from scratch by installing the core and supporting files with **npm** (or **yarn**). In this case, of course, you'll be responsible for creating the project boilerplate files yourself.

```shell
$ npm i --save @nestjs/core @nestjs/common rxjs reflect-metadata
```

[🔼 Back to top](#nestjs-tutorial)

### 📜 References

- [Nestjs Documentation](https://docs.nestjs.com)

### 🤝 Contributors

- Mengsreang-Chhoeung [@mengsreang_dev](https://twitter.com/mengsreang_dev)
