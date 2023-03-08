# Nestjs Tutorial

<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

<p align="center"><i>A progressive <b><a href="http://nodejs.org">Node.js</a></b> framework for building efficient, reliable and scalable server-side applications.</i></p>

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

The `project-name` directory will be created, node modules and a few other boilerplate files will be installed, and a `src/` directory will be created and populated with several core files.

<img src="./doc-images/project-structure.jpeg" width="100%" alt="project-structure">

Here's a brief overview of those core files:

- `app.controller.ts`: A basic controller witha single route.
- `app.controller.spec.ts`: The unit tests for the controller.
- `app.module.ts`: The root module of the application.
- `app.service.ts`: A basic service with a single method.
- `main.ts`: The entry file of the application which uses the core function `NestFactory` to create a Nest application instance.

The `main.ts` includes an async function, which will **bootstrap** our application:

```ts
main.ts;

import { NestFactory } from "@nestjs/core";
import { AppModule } from "./app.module";

async function bootstrap() {
  const app = await NestFactory.create(AppModule);
  await app.listen(3000);
}
bootstrap();
```

To create a Nest application instance, we use the core `NestFactory` class. `NestFactory` exposes a few static methods that allow creating an application instance. The `create()` method returns an application object, which fulfills the `INestApplication` interface. This object provides a set of methods which are described in the coming chapters. In the `main.ts` example above, we simply start up our HTTP listener, which lets the application await inbound HTTP requests.

### Running the application

Once the installation process is complete, you can run the follwing command at your OS command prompt to start the application listening for inbound HTTP requests:

```shell
$ npm run start
```

This command starts the app with the HTTP server listening on the port defined in the `src/main.ts` file. Once the application is running, open your browser and navigate to `http://localhost:3000/`. You should see the `Hello World!` message.

To watch for changes in your files, you can run the following command to start the application:

```shell
$ npm run start:dev
```

This command will watch your files, automatically recompiling and reloading the server.

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

[🔼 Back to top](#nestjs-tutorial)

### 📜 References

- [Nestjs Documentation](https://docs.nestjs.com)

### 🤝 Contributors

- Mengsreang-Chhoeung [@mengsreang_dev](https://twitter.com/mengsreang_dev)
