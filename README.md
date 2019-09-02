# Colyseus + PixiJS <a href="https://patreon.com/endel" title="Donate to this project using Patreon"><img src="https://img.shields.io/badge/endpoint.svg?url=https%3A%2F%2Fshieldsio-patreon.herokuapp.com%2Fendel&style=for-the-badge" alt="Donate on Patreon"/></a>

A simple boilerplate using Colyseus + PixiJS. It implements a simplistic version of the classical [agar.io](http://agar.io/) game.

[View live demo](https://colyseus-pixijs-boilerplate.herokuapp.com)

## Running locally

This demo uses `@colyseus/social`, that requires [MongoDB](https://www.mongodb.com/download-center#community) to be installed on your machine. Alternatively, you can remove [this line](https://github.com/endel/colyseus-pixijs-boilerplate/blob/76c4879597faafb4f2450a03d8017c75c251ab32/src/client/Application.ts#L61) if you don't want to use it.

```
git clone https://github.com/endel/colyseus-pixijs-boilerplate.git
cd colyseus-pixijs-boilerplate
npm install
npm run dev
```

Open [http://localhost:8080](http://localhost:8080) in your browser.

## Directory structure

```
├── nodemon.json
├── package.json
├── src
│   ├── client
│   │   ├── Application.ts
│   │   ├── index.html
│   │   └── index.ts
│   └── server
│       ├── index.ts
│       └── rooms
│           ├── ArenaRoom.ts
│           ├── Entity.ts
│           └── State.ts
├── tsconfig-client.json
├── tsconfig.json
└── webpack.config.js
```

- All frontend dependencies should be included as `devDependencies` on `package.json`.
- All backend dependencies should be included as `dependencies` on `package.json`.

## TODO:
- [ ] Enter name before starting the game
- [ ] Re-spawn button after dead
- [ ] Leaderboard

## License

MIT
