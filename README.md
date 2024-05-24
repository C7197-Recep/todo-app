# todo-app

This application is generated using [LoopBack 4 CLI](https://loopback.io/doc/en/lb4/Command-line-interface.html) with the
[initial project layout](https://loopback.io/doc/en/lb4/Loopback-application-layout.html).

## Install dependencies

By default, dependencies were installed when this application was generated.
Whenever dependencies in `package.json` are changed, run the following command:

```sh
npm install
```

To only install resolved dependencies in `package-lock.json`:

```sh
npm ci
```

## Run the application

```sh
npm start
```

You can also run `node .` to skip the build step.

Open http://127.0.0.1:3000 in your browser.

## Rebuild the project

To incrementally build the project:

```sh
npm run build
```

To force a full build by cleaning up cached artifacts:

```sh
npm run rebuild
```

## Fix code style and formatting issues

```sh
npm run lint
```

To automatically fix such issues:

```sh
npm run lint:fix
```

## Other useful commands

- `npm run migrate`: Migrate database schemas for models
- `npm run openapi-spec`: Generate OpenAPI spec into a file
- `npm run docker:build`: Build a Docker image for this application
- `npm run docker:run`: Run this application inside a Docker container

## Tests

```sh
npm test
```

## What's next

Please check out [LoopBack 4 documentation](https://loopback.io/doc/en/lb4/) to
understand how you can continue to add features to this application.

[![LoopBack](https://github.com/loopbackio/loopback-next/raw/master/docs/site/imgs/branding/Powered-by-LoopBack-Badge-(blue)-@2x.png)](http://loopback.io/)

# Extra Info

You can find database usage alternatives in src/datasources.ts file

You have three options there:

1. You can use FAKE DB, which is already set.

2. You can use ONLINE DB. To use this option:

    a.  First, set up an online MONGO DB
    b.  Update "host: 'user:password@cluster0.lopa7ph.mongodb.net'" part in the datasources.ts file
    c.  Run this loopback app (npm start)
    d.  Go to Api Explorer from your browser (http://localhost:3000/explorer/)
    e.  Post a new todo there

    When you go to your MONGO DB, you will see the new todo added.

3.  You can use LOCAL DB. To use this option:

    a.  Download MongoDB and set it up (https://www.mongodb.com/try/download/community)
    b.  When the MongoDB Compass opens, create a collection
    c.  Run this loopback app (npm start)
    d.  Go to Api Explorer from your browser (http://localhost:3000/explorer/)
    e.  Post a new todo there

    When you go to your MONGO DB Compass, you will see the new todo added.